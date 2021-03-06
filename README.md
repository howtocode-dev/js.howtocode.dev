# ভূমিকা

**প্রধান লেখক ও সমন্বয়ক**  
[নুহিল মেহেদী](https://nuhil.net/)

**অন্যান্য লেখক ও কন্ট্রিবিউটরদের তালিকা**  
[বিস্তারিত এখানে](https://github.com/howtocode-dev/js.howtocode.dev/graphs/contributors?type=a)

জাভাস্ক্রিপ্ট বা সংক্ষেপে JS হচ্ছে first-class ফাংশন এর সমন্বয়ে গঠিত একটি লাইট ওয়েট, ইন্টারপ্রেটেড \(কম্পাইল করার প্রয়োজন নেই\) প্রোগ্রামিং ভাষা।

অনেকেই মনে করে জাভাস্ক্রিপ্টের কাজ শুধুমাত্র ওয়েবপেজের ফর্ম ভ্যালিডেশন আর টুকটাক কিছু ডোম ম্যানিপুলেশনের মধ্যেই সীমাবদ্ধ। আর এটা একটা ক্লায়েন্ট সাইড ল্যাঙ্গুয়েজ অর্থাৎ শুধু ব্রাউজারের মধ্যেই রান করে পারে। কিন্তু ধারনা শতভাগ ভুল। সার্ভার সাইড ও নেটওয়ার্ক প্রোগ্রামিং, মোবাইল ও ডেস্কটপ অ্যাপ ডেভেলপমেন্ট, গেইম ডেভেলপমেন্ট থেকে শুরু করে ইন্টারনেট অব থিংস, মেশিন লার্নিং এ গিয়েও দেখা মিলবে এই জাভাস্ক্রিপ্ট এর। আর এটাকে ইন্টারমেডিয়েট ল্যাঙ্গুয়েজ ধরে এর উপর তৈরি হয়েছে বেশ কিছু সাব ল্যাঙ্গুয়েজ যেমন কফিস্ক্রিপ্ট, [TypeScript](https://www.typescriptlang.org/) ইত্যাদি।

এটা সত্য যে, এটি ওয়েব পেজের স্ক্রিপ্টিং ভাষা হিসেবে বেশি পরিচিত, কিন্তু ব্রাউজার ছাড়াও অন্যান্য জায়গায় ব্যবহার করা হয়, যেমন [Apache CouchDB](http://couchdb.apache.org/), [MongoDB](https://www.mongodb.com/) ইত্যাদি ডাটাবেইজ সার্ভিস তাদের স্ক্রিপ্টিং ল্যাঙ্গুয়েজ এবং কুয়েরী ল্যাঙ্গুয়েজ হিসেবে জাভাস্ক্রিপ্ট ব্যবহার করে। আবার, [node.js](https://nodejs.org/en/) বা সম্প্রতি রিলিজ হওয়া [Deno](https://deno.land/) এর মত প্ল্যাটফর্ম জাভাস্ক্রিপ্টকে ব্রাইজার স্কোপের বাইরে এনে এমন একটি এনভায়রনমেন্ট দিয়েছে যাতে করে জাভাস্ক্রিপ্ট এর মাধ্যমে ডেক্সটপ এবং সার্ভার প্রোগ্রামিং-ও দিন দিন জনপ্রিয় হচ্ছে। এছাড়াও জাভাস্ক্রিপ্ট এর উপর ভিত্তি করে তৈরি হাজার হাজার লাইব্রেরী এবং ফ্রেমওয়ার্ক যেমন - [AngularJS](https://angularjs.org/), [React](https://facebook.github.io/react/), [Express](https://expressjs.com/), [JQuery](https://jquery.com/) যেগুলো বদলে দিয়েছে সফটওয়্যার ডেভেলপমেন্ট এর চেহারা। এমনকি [ConvNetJS](https://github.com/karpathy/convnetjs) এর মত লাইব্রেরীর মাধ্যমে মেশিন লার্নিং নিয়ে কাজ করাও জনপ্রিয় হচ্ছে ব্রাউজারেই।

> JS হল prototype-based, মাল্টি প্যারাডাইম, ডাইনামিক স্ক্রিপ্টিং ল্যাঙ্গুয়েজ যা একাধারে object-oriented, imperative, এবং declarative তথা functional programming স্টাইল সাপোর্ট করে।
>
> ১৯৯৫ সালে তৈরি এই ল্যঙ্গুয়েজের তখনকার উদ্দেশ্য ছিল নেটস্কেপ ব্রাউজারে ওয়েব পেজের জন্য প্রোগ্রাম লেখা। পরবর্তীতে প্রায় সবগুলা আধুনিক ব্রাউজারই জাভাস্ক্রিপ্ট অন্তর্ভুক্ত করে নেয়।

জাভাস্ক্রিপ্ট স্ট্যান্ডার্ড এর নাম ECMAScript। ২০১২ সাল পর্যন্ত পাওয়া তথ্য অনুযায়ী সব নতুন ব্রাউজার ECMAScript 5.1 সমর্থন করে। পুরোনো ব্রাউজারগুলো অন্তত ECMAScript 3 সমর্থন করে। ২০১৫ সালের ১৭ জুন ECMA International তার ষষ্ঠ প্রধান সংস্করণ প্রকাশ করে, আনুষ্ঠানিক ভাবে যা ECMAScript 2015 নামে অভিহিত, এবং সাধারন ভাবে এটি ECMAScript 6 বা ES6 নামে পরিচিত। তখন থেকেই বাৎসরিক প্রকাশ চক্র অনুযায়ী ECMAScript -এর মান প্রকাশিত হচ্ছে।

**ভ্রান্ত ধারনা**  
উঠতি প্রোগ্রামারদের মধ্যে একটি সাধারণ ভ্রান্ত ধারনা আছে যে, জাভাস্ক্রিপ্ট এর সাথে জাভার অনেক অনেক মিল এবং জাভার সাথে ওতপ্রোতভাবে সম্পর্কিত।

নামের মিলের সাথে সাথে এটাও সত্যি যে, দুটো ল্যাঙ্গুয়েজের-ই সিনট্যাক্স সি এর মত। আসলে, জাভা-র সিনট্যাক্স এবং স্ট্যান্ডার্ড লাইব্রেরী গুলোর কথা মাথায় রেখেই জাভাস্ক্রিপ্ট ডিজাইন করা হয়েছে। অর্থাৎ, জাভার প্রায় সব গুলো কি-ওয়ার্ড মুল জাভাস্ক্রিপ্টেও রিজার্ভড। আবার জাভাস্ক্রিপ্ট এর স্ট্যান্ডার্ড লাইব্রেরী গুলো জাভার নেমিং কনভেনশন ফলো করে। আরও কিছু মিল যেমন, জাভা ১.০ এর ক্লাসের উপর ভিত্তি করেই জাভাস্ক্রিপ্টের ডেট এবং ম্যাথ অবজেক্ট তৈরি। এমনকি, জাভা এবং জাভস্ক্রিপ্ট দুটোই ২৩ মে ১৯৯৫ -এ প্রকাশিত। কিন্তু মিলের ব্যপারটা এখান পর্যন্তই।

জাভা ডেভেলপ করেছেন সান মাক্রসিস্টেমের জেমস গসলিং এবং জাভাস্ক্রিপ্ট ডেভেলপ করেছেন নেটস্কেপ কমিউনিকেশনস এর ব্রেন্ড্যান এইচ। জাভা স্ট্যাটিক্যালি টাইপড কিন্তু জাভাস্ক্রিপ্ট ডাইনামিক। কম্পাইল করা বাইট কোড থেকে জাভা লোড হয় কিন্তু জাভাস্ক্রিপ্ট লোড হয় আমাদের লেখা সোর্স কোড থেকেই। জাভার অবজেক্ট হচ্ছে ক্লাস ভিত্তিক কিন্তু জাভাস্ক্রিপ্ট এর অবজেক্ট প্রোটোটাইপ ভিত্তিক। জাভা ৮ এর আগ পর্যন্ত এটা ফাংশনাল প্রোগ্রামিং সাপোর্ট করতো না যেখানে, জাভাস্ক্রিপ্টে এই ফিচার অনেক আগে থেকেই ছিল। সর্বোপরি দুটো ল্যাঙ্গুয়েজ, সফটওয়্যার ডেভেলপমেন্টের পথে আলাদা আলাদা উদ্দেশ্যে ব্যবহৃত হয়।

**ওপেন সোর্স**

এই বইটি মূলত স্বেচ্ছাশ্রমে লেখা এবং বইটি সম্পূর্ন ওপেন সোর্স । এখানে তাই আপনিও অবদান রাখতে পারেন লেখক হিসেবে । আপনার কন্ট্রিবিউশান গৃহীত হলে অবদানকারীদের তালিকায় আপনার নাম যোগ করে দেওয়া হবে।

এটি মূলত একটি [গিটহাব রিপোজিটোরি](https://github.com/howtocode-dev/js.howtocode.dev) যেখানে এই বইয়ের আর্টিকেল গুলো মার্কডাউন ফরম্যাটে লেখা হচ্ছে । রিপোজটরিটি ফর্ক করে পুল রিকুয়েস্ট পাঠানোর মাধ্যমে আপনারাও অবদান রাখতে পারেন । বিস্তারিত দেখতে পারেন এই ভিডিওতে [Video](http://blog.howtocode.com.bd/?p=32)

> **বর্তমানে বইটির কন্টেন্ট বিভিন্ন কন্ট্রিবিউটর এবং নানা রকম সোর্স থেকে সংগৃহীত এবং সংকলিত।**

  
This work is licensed under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/).

