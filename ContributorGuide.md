Templating
==========

###main.blade.php

Views ထဲမွာ Templates ဆိုတဲ folder ရယ္ pages ဆိုတဲ့ folder ရယ္ ႏွစ္ခုခြဲထားပါတယ္။ Templates folder ထဲမွာ Main Template ျဖစ္တဲ့ main.blade.php ပါ။ main template ရဲ့ body tag ထဲမွာ ပထမဆံုးေရးထားတဲ့ @if (Sentry::check()) က login ဝင္ထားခဲ့ရင္ Username ကို သိမ္းထားခဲ့တာပါ။ @if (Session::has('success')) ရယ္ error ရယ္ info ရယ္ warning ရယ္က flash message အတြက္ session ကို စစ္ျပီး Session မွာ message တစ္ခုခုရွိရင္ ျပဖို႔အတြက္ပါ။ ျပီးရင္ pages folder ထဲက header.blade.php ကို Include လုပ္ထားပါတယ္။ ေနာက္တစ္ေၾကာင္း Sentry နဲ႔စစ္ထားတာက Login ဝင္ထားမွ sidebar နဲ႔ breadcrumb ကို include လုပ္ထားတာပါ။ ေနာက္တစ္ေၾကာင္းကေတာ့ content အတြက္ yield လုပ္ထားတာပါ။ ေအာက္ဆံုးမွာပါတဲ့ script က flash message အတြက္ ေရးထားတဲ့ script ပါ။

###header.blade.php

header ကေတာ့ bootstrap ရဲ့ navbar ပါ။ အဲ့ဒီမွာ login ဝင္ထားရင္ ျမင္ရမဲ့အပိုင္းနဲ႔ login မျဖစ္ရင္ ျမင္ရမဲ့အပိုင္းကို Sentry::check() နဲ႔သံုးျပီး စစ္ထားတယ္။ 