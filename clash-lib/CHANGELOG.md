# Changelog for the [`clash-lib`](http://hackage.haskell.org/package/clash-lib) package

## 0.5 *March 11th 2015*
* New features:
  * Simplify BlackBox handling, and improve VHDL generation. [#47](https://github.com/clash-lang/clash-compiler/issues/47)
  * Use unbound-generics. [#48](https://github.com/clash-lang/clash-compiler/issues/48)

* Fixes bugs:
  * VHDL generation error: wrapper for sum-of-products type. [#44](https://github.com/clash-lang/clash-compiler/issues/44)

## 0.4.1 *February 4th 2015*
* Fixes bugs:
  * Treat BlackBox expressions as declarations when DC args. [#37](https://github.com/christiaanb/clash2/issues/33)
  * Don't inline recursive closed bindings

## 0.4 *November 17th 2014*
* New features:
  * Support for clash-prelude 0.6

* Fixes bugs:
  * Ambiguous type: 'std_logic_vector' or 'std_ulogic_vector' [#33](https://github.com/christiaanb/clash2/issues/33)

## 0.3.2 *June 5th 2014*

* Fixes bugs:
  * VHDL array constant ambiguous [#18](https://github.com/christiaanb/clash2/issues/18)
  * Exception: can't create selector [#24](https://github.com/christiaanb/clash2/issues/24)
  * Calls to `vhdlTypeMark` don't result to inclusion of VHDL type in types.vhdl [#28](https://github.com/christiaanb/clash2/issues/28)

## 0.3.1 *May 15th 2014*

* New features:
  * Make ANF lift non-representable values [#7](https://github.com/christiaanb/clash2/issues/7)
  * Hardcode `fromInteger` for `Signed` and `Unsigned` [#9](https://github.com/christiaanb/clash2/issues/9)
  * Replace VHDL default hole by error hole [#13](https://github.com/christiaanb/clash2/issues/13)

* Fixes bugs:
  * Type families are not expanded [#3](https://github.com/christiaanb/clash2/issues/3)
  * Exception: CLaSH.Netlist.VHDL(512): fromSLV: Vector 13 Bool [#5](https://github.com/christiaanb/clash2/issues/5)
  * Incorrect vhdl generation for default value in blackbox [#6](https://github.com/christiaanb/clash2/issues/6)
  * Duplicate type names when multiple ADTs need the same amount of bits [#8](https://github.com/christiaanb/clash2/issues/8)
  * Circuit testbench generation with MAC example fails[#15](https://github.com/christiaanb/clash2/issues/15)

* Code improvements:
  * Refactor Netlist/BlackBox [#10](https://github.com/christiaanb/clash2/issues/10)
  * CPP special-case conversion of `Control.Exception.Base.irrefutPatError` [#11](https://github.com/christiaanb/clash2/issues/11)

