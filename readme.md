1. A builds as x64 and B builds as anycpu
2. A passes Platform=x64 because same plat
3. B gets platform=x86
4. Q: What does compiler do if given no plat?
5. B gets anycpu as most compatible
6. B should get win32 from the default lookup table
7. B gets whatever you build with that's compatible with A