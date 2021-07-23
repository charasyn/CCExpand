# So you want to add ASM into your script?
Easiest way:
1. Add all `.ccs` files in this directory to your project.
2. In your file where you want to call the ASM, do `import cc_asmcall`.
3. To actually call an ASM function, do `cc_asmcall(<asm label name>, RET_NONE)`.

Example:
```
import asm65816
import cc_asmcall
test_text: {
    "@Hello! This is text." next
    "@Let's call some ASM." next
    cc_asmcall(test_asm, RET_NONE)
    "@...That was easy!" next
    eob
}
test_asm: {
    // Put your ASM here!
    RTL
}
```
