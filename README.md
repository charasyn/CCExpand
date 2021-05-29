# CCExpand
This project aims to allow users to easily implement their own assembly-code
control codes into an EarthBound ROM hack.

## Usage
1. Write assembly functions to implement your custom functionality
  (see the documentation in `ccexpand.ccs` and the examples)
1. Add your assembly routine to `CodeTable` in `ccexpand.ccs`
1. Use your new control code in a script!
1. Recommended: Add commands that wrap your control code to make it
  easier to use (see `cc_asmcall.ccs` for a good example)

## Examples
Some examples of custom control codes can be seen in the `example/` directory:
- `cc_asmcall.ccs`: Provides a method to call an assembly function from
  CCScript and read the return value. Provided by Catador.
- `cc_text_speed.ccs`: Allows the user to get and set the current text speed.
  Provided by jtolmar.
- `cc_example_simple.ccs`: Simple functions that show how to return values to
  the script. Provided by cooprocks123e.

## Thanks
- jtolmar for providing a WIP which this was based on
- phoenixbound and Catador for their support during development
- All of the randomizer developers for inspiring me to get involved with PK Hacking
- Everyone else on the PK Hack Discord for being awesome
- The [EarthBound ROM Explorer](https://earthbound-rom-explorerr.herokuapp.com/)
- The [Data Crystal page](https://datacrystal.romhacking.net/wiki/EarthBound) for EarthBound
- [CoilSnake wiki](https://github.com/pk-hack/CoilSnake/wiki)
- [Starmen.net CCScript Reference](https://starmen.net/pkhack/ccscript/) (An oldie but a goodie)
- Saving the best for last, [ebsrc](https://github.com/Herringway/ebsrc), without which this would
  have taken 3 weeks instead of 3 days
