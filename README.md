import { useState } from "react"; import { Button } from "@/components/ui/button"; import { Input } from "@/components/ui/input"; import { Textarea } from "@/components/ui/textarea"; import { Card, CardContent } from "@/components/ui/card"; import { MessageCircle } from "lucide-react";

export default function PinkySoftGothic() { const [messages, setMessages] = useState([]); const [input, setInput] = useState("");

const handleSend = () => { if (input.trim()) { setMessages([...messages, { text: input, fromUser: true }]); setInput(""); } };

return ( <div className="min-h-screen bg-pink-100 text-gray-800 p-4"> <div className="max-w-

