# for লুপ

লুপিং এর কাজে সবছেয়ে বেশি ব্যবহৃত হয় for loop. এ for loop এর তিনটি অংশ রয়েছে। তার আগে আমরা দেখেনি for loop সাধারন ব্যবহার নিয়ম।

## for\(exprission1;Exprission2;Expression3\)Statement

বিদ্রঃ এখানে প্রত্যেকটি Expression ; \(সেমিকোলন\) দিয়ে আলাদা করে দিতে হবে।

এখানে প্রথম exprission1 হচ্ছে for loop এর প্রথম অংশ। এটি দ্বারা একটি প্রাথমিক মান দেওয়া হয় । যাকে বলা হয় initial অংশ। এটি পুরো লুপিং প্রক্রিয়াকে নিয়ন্ত্রন করে।

দ্বিতীয় অংশটি অর্থাৎ Exprission2 দ্বারা একটি শর্ত দেওয়া হয়। লুপটি কতক্ষন পর্যন্ত চলবে তা এটি নির্নয় করে। Exprission2 তে সাধারনত একটি logical expression থাকে যা শুধু সত্য মিথ্যে বুঝতে পারে। যদি সত্য হয় তাহলে 1 রিটার্ন করে আর যদি মিথ্যে হয় তাহলে 0 রিটার্ন করে। এটি যদি 0 ছাড়া অন্য কোন মান রিটার্ন করে তাহলে লুপটি চলবে, আর যদি 0 রিটার্ন করে তাহলে লুপটি আর চলবে না।

Expression3 কাজ হচ্ছে আমারা প্রথমে যে প্রাথমিক মান নিলাম তাকে আমাদের ইচ্ছে মত মডিফাই করা। এটি প্রত্যেক লুপের শেষ ধাপে কাজ করে।

আর আগেই বলছি লুপটি ততক্ষনই চলবে যতক্ষন পর্যন্ত Exprission2 মিথ্যে বা 0 রিটার্ন না করে।

For loop সম্পর্কে আমরা এতক্ষন অনেক কিছু জানলাম, এবার প্রোগ্রামে এটাকে কিভাবে ব্যবহার করব তা দেখি। তার জন্য একটি প্রোগ্রাম লিখি যা 1 থেকে 10 পর্যন্ত সংখা গুলো প্রিন্ট করবে। আপনাদের জন্য নিচের প্রোগ্রামটি। এটার আউটপুট কি হবে কিভাবে হবে তা বের করুন।

এর আউট পুট হচ্ছেঃ `০ 1 2 3 4 5 6 7 8 9 10` এখানে আমরা একটি integer variable নিয়েছি। for loop এর প্রথম Expression এ আমরা এর প্রাথমিক মান নিলাম ০. প্রাথমিক মানটি for loop এর দ্বিতীয় অংশ অর্থাৎ logical অংশ দ্বারা যাচাই না হয়েই for লুপের ভেতরে থাকা স্টেটমেন্টটি এক্সিকিউট করবে। এবং প্রথম Expression কাজ শেষ হয়ে যাবে। এর আর কোন কাজ নেই। Print করার পর এবার তৃতীয় অংশ অর্থাৎ Exprission3 এখানে i++ অংশ দ্বারা মডিফাই হবে। আমরা জানি i++ এর মানে হচ্ছে i = i+1 সুতরাং এখানে i এর মান এক বাড়বে এবং ০ থেকে 1 হবে। এবার দ্বিতীয় অংশ Expression2 এখানে এসে i&lt;=10 অংশ দ্বারা লজিক্যাল যাচাই হবে। এখানে যাচাই করবে যে i এর মান 10 বা 10 থেকে ছোট কিনা। যেহেতু এখন i এর মান ১০ থেকে ছোট তাই লুপটা আবার চলবে। এবং দ্বিতীয় বার এসে 1 প্রিন্ট করবে। আবার Exprission3 তে এসে মডিফাই হবে। আগের লুপ থেকে i এর মান পেয়েছি 1 এখন আবার 1 এর সাথে এক বেড়ে 2 হবে \( এ অংশ i++ দ্বারা\) । আবার দ্বিতীয় অংশ i&lt;=10 অংশ দ্বারা লজিক্যাল যাচাই হবে। যেহেতু 2, 10 থেকে ছোট তাই আবার 2 প্রিন্ট করবে। এভাবে প্রত্যেক ধাপ শেষ করবে। যখন i এর মান বেড়ে 11 হয়ে যাবে তখন আর লুপ চলবে না। এবং আমাদের প্রোগ্রামটি শেষ হবে। আচ্ছা, আরেকটা প্রোগ্রাম লিখি। ছোট কালে কোন দুষ্টুমি করলে যে আমাদের শাস্তি দেওয়া হতো একশ বার লিখতে, আমি আর দুষ্টুমি করব না। আমরা এবার তা লিখব প্রোগ্রাম লিখে। এবং for লুপ ব্যবহার করে।

এখানে আগের প্রোগ্রামের থেকে একটু পার্থক্য হচ্ছে আগে আমরা i এর মান প্রিন্ট করেছি। এখানে আমরা একটা লাইন প্রিন্ট করেছি "ami r dustumi korbo na." for লুপ এর ভেতরের Exprission2 তে লিখেছি i&lt;=100। মানে i এর মান যতক্ষণ না পর্যন্ত ১০০ হচ্ছে, ততক্ষণ পর্যন্ত এই লুপটি চলবে। Exprission3 তে i এর মান আমরা প্রতিবার ১ করে বাড়িয়ে দিয়েছি। এবার আমরা আরেকটি প্রোগ্রাম লিখি। এবার এক থেকে ৫০ পর্যন্ত বেজোড় সংখ্যা গুলো বের করার একটা প্রোগ্রাম লিখি।

আগের প্রথম প্রোগ্রামের মতই i এর মান আমরা প্রিন্ট করেছি। তবে একটা কন্ডিশন দিয়েছি এখানে। for লুপের ভেতর প্রতিবার ঢুকবে। ঢুকার পর if দিয়ে একটা কন্ডিশন চেক করবে। if\(i%2==1\) মানে হচ্চে i কে দুই দ্বারা ভাগ করলে ভাগ শেষ যদি ১ থাকে, তাহলে if কন্ডিশনের ভেতরের স্টেটমেন্ট printf\("%dn",i\); দিয়ে i এর মান প্রিন্ট হবে। আর না হলে কিছুই হবে না। এখানে কি করছি কি, একটা লুপের ভেতর আরেকটা লুপ ব্যবহার করেছি। আমরা ইচ্ছে করলে এমন একটা লুপের ভেতর আরেকটা, আরেকটা ভেতর আরেকটা এমন ইচ্ছে মত ব্যবহার করতে পারি। যেমন আমরা এবার একটা for লুপের ভেতর আরেকটা for লুপ ব্যবহার করব। তবে তার আগে উপরের প্রোগ্রামটি আরো সহজে কিভাবে লেখা যায়, তা দেখি। আমরা ইচ্ছে করলে ১ থেকে ৫০ পর্যন বেজোড় সংখ্যা গুলো নিচের মত করেও বের করতে পারিঃ এখানে করছি কি i এর প্রথম মান ধরে নিয়েছি ১। এক একটা বিজোড় সংখ্যা। তা প্রিন্ট করবে। এরপর ১ এর সাথে ২ যোগ করে দিলেই তো হবে ৩, তা বিজোড় সংখ্যা। তা প্রিন্ট করবে। এরপর ৩ এর সাথে ২ যোগ করে দিলে হবে ৫, তা বিজোড় সংখ্যা। তা প্রিন্ট করবে। আমরা লুপের Expression3 তে লিখছি i=i+2। লুপের Expression2 তে কন্ডিশন দিয়েছি i&lt;=50। মানে যতক্ষণ না পর্যন্ত i এর মান ৫০ এর বেশি হবে, ততক্ষন পর্যন্ত লুপটি চলবে।। এবার একটা for লুপের ভেতরে আরেকটা for লুপ ব্যবহার করে একটা প্রোগ্রাম লিখিঃএখানে আমরা দুইটা ভ্যারিয়েবল নিয়েছি। i এবং j. প্রথম for লুপের ভেতর i এর ইনিশিয়াল মান দিয়েছি ০, কন্ডিশন দিয়েছি i&lt;=5 এবং i এর মান 1 করে বাড়িয়েছি। মানে হচ্ছে প্রথম for লুপটি ৫ বার এক্সিকিউট হবে। প্রোগ্রামটি আউটপুট দিবঃ \`\`\`c 0 0 1 0 1 2 0 1 2 3 0 1 2 3 4 0 1 2 3 4 5 \`\`\` দ্বিতীয় ফর লুপে j=0 দিয়ে ইনিশিয়াল মান দিয়েছি ০, এরপর j&lt;=i দিয়ে কন্ডিশন দিয়েছি। এবং শেষে j++ দিয়ে j এর মান বাড়িয়েছি। কন্ডিশন অনুযায়ী দ্বিতীয় ফরলুপটি কতবার এক্সিকিউট হবে তা নির্ভর করবে প্রথম ফর লুপের উপর। যেমন প্রথম বার i এর মান ০। তাই প্রথমবার দ্বিতীয় ফর লুপ চলবে একবার। দ্বিতীয় বার i এর মান ১, তাই দ্বিতীয় বার দ্বিতীয় লুপ চলবে দুই বার। তৃতীয় বার দ্বিতীয় ফর লুপ চলবে ৩ বার। এবার পঞ্চম বার দ্বিতীয় লুপ চলবে ৫বার। প্রথম বার দ্বিতীয় লুপ প্রিন্ট করবে ০, দ্বিতীয়বার প্রিন্ট করবে 0 1. তৃতীয় বার 0 1 2. এভাবে পঞ্চম বার প্রিন্ট করবে 0 1 2 3 4 5. এখন আমরা যদি প্রথম ফর লুপের কন্ডিশন পরিবর্তন করে দশ করে দি, তাহলে আউটপুট দিবেঃ [![nested for demo](http://jakir.me/wp-content/uploads/2015/03/nested-for-demo.png)](http://jakir.me/wp-content/uploads/2015/03/nested-for-demo.png) [do while](http://jakir.me/c-do-while/) দিয়ে আমরা কয়েকটা সংখ্যার গড় বের করার প্রোগ্রাম লিখেছি এর আগে। এবার আমরা তা for লুপ ব্যবহার করে লিখবঃ
