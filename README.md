## Comfy-Sentry
This "custom node" repository is actually nodeless, but provides a ComfyUI integration to a 
[Sentry](https://sentry.io/welcome/) error reporting 
backend. This way, you can have full code and error reporting, performance monitoring and metrics, etc. in your 
ComfyUI interface reported to a Sentry backend.

---

In your Python environment for ComfyUI (it may be a `venv` and you will need to activate it), run 
`pip install sentry-sdk` to install the requisite components for the repository.

To use this, simply clone the repository into the `custom_nodes` folder of your ComfyUI root directory. Then, copy 
`sentry_config.example.json` to `sentry_config.json` within the cloned directory, and adjust your settings accordingly 
to configure your Sentry instance settings.

Then simply start ComfyUI. It will then attempt your Sentry connection and integrations automatically on startup 
before even the main UI is loaded.

**Note that any and all errors generated by your ComfyUI will be reported to this Sentry instance you've configured.**

---

This repository, unless otherwise specified, is licensed under GPL-3.0.


<a href="https://scan.coverity.com/projects/teward-comfy-sentry">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/30552/badge.svg"/>
</a>
