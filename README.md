# https://corekits.framer.website/
# https://rsms.me/inter/


// app/layout.tsx

import { Inter } from "next/font/google";

const inter = Inter({
  subsets: ["latin"],
  variable: "--font-inter",
});

export default function RootLayout({
  children,
}: {
  children: React.ReactNode;
}) {
  return (
    <html lang="en" className={inter.variable}>
      <body>{children}</body>
    </html>
  );
}

body {
  font-family: var(--font-inter), system-ui, sans-serif;
}
