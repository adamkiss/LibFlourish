# Flourish for ProcessWire v0.9.0

ProcessWire wrapper around the great [unframework Flourish](http://flourishlib.com). Makes tracking of correct lib, and updating it in PW a breeze (when using with [Modules Manager](http://modules.processwire.com/modules/modules-manager/)). The module version mirrors the included Flourish version, so whenever Flourish is updated, this module is updated as well and voillá – you may use the new version.

---

# Installation

* via [Modules Manager](http://modules.processwire.com/modules/modules-manager/) (recommended)
* Download into `/site/modules/` and install

# Usage

Anywhere you need to use Flourish library, make following call:

```
  // in templates
  $modules->get('LibFlourish');

  // in modules
  $this->modules->get('LibFlourish');

  // anywhere else
  wire('modules')->get('LibFlourish');
```

This inits the sole function of this wrapper – `spl_autoloader` for Flourish – so you now can freely use your Flourish powered code.

# License

Wrapper – the module itself are licensed under [WTFPL](http://www.wtfpl.net/) and were created by [Adam Kiss](http://adamkiss.com). Flourish classes are licensed under MIT License and created by [Will Bond](http://wbond.net/). Thanks Will.