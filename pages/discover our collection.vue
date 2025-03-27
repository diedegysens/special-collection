import Image from "next/image";

export default function Collection() {
  const images = [
    "/images/book1.jpg",
    "/images/book2.jpg",
    "/images/book3.jpg",
    "/images/book4.jpg",
    "/images/book5.jpg",
    "/images/book6.jpg",
  ];

  return (
    <div className="min-h-screen bg-white px-10 py-6">
      {/* Header */}``

    
        <h1 className="text-5xl font-bold text-orange-500">our collection</h1>
        <div className="space-x-4">
          <button className="text-black text-lg font-medium">menu</button>
          <button className="text-black text-lg font-medium">search</button>
        </div>
 

      {/* Image Grid */}
       className="mt-8 grid grid-cols-3 gap-6">
        images.map(src, index) => 
          <div key={index} className="relative w-full h-60">
            <Image src={src} alt={`Book ${index}`} layout="fill" objectFit="cover" className="rounded-lg" />
          </div>
        )}
      
    
  ;

