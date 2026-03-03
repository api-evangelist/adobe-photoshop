# Adobe Photoshop (adobe-photoshop)
Adobe Photoshop is the industry-standard image editing and digital design application. Its developer platform offers a cloud-based REST API for programmatic image processing via Firefly Services, the UXP plugin framework for building desktop extensions with modern JavaScript, a C++ plugin SDK for native filters and file formats, and scripting interfaces for workflow automation.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Image Editing, Creative Cloud, Photoshop, REST API, Plugins, Scripting, AI/ML

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-02-28

## APIs

### Adobe Photoshop API
A cloud-based REST API that provides programmatic access to Photoshop's image editing capabilities without requiring a local installation. Part of Adobe Firefly Services, the API supports PSD document operations including layer editing, Smart Object replacement, text layer editing, and artboard creation. It also provides AI-powered features such as background removal, mask creation, product crop, and depth blur. All operations are asynchronous, returning a polling URL to check job status, and support webhooks via Adobe I/O Events for completion notifications.

**Human URL:** [https://developer.adobe.com/firefly-services/docs/photoshop/](https://developer.adobe.com/firefly-services/docs/photoshop/)


#### Tags:

 - REST API, Cloud, Image Processing, PSD Editing, Background Removal, AI/ML, Asynchronous

#### Properties

- [Documentation](https://developer.adobe.com/firefly-services/docs/photoshop/)
- [OpenAPI](openapi/adobe-photoshop-api-openapi-original.yml)
- [AsyncAPI](asyncapi/adobe-photoshop-api-asyncapi-original.yml)
- [APIReference](https://developer.adobe.com/firefly-services/docs/photoshop/api/)
- [GettingStarted](https://developer.adobe.com/firefly-services/docs/photoshop/getting_started/)

### Adobe Firefly Services SDK for JavaScript
A unified Node.js and TypeScript SDK that provides typed client libraries for accessing the Photoshop API and other Firefly Services. The PhotoshopClient class offers methods for background removal, mask creation, PSD rendition generation, document creation and modification, Smart Object replacement, text layer editing, Photoshop Actions execution, auto crop, and depth blur. The SDK simplifies authentication with ClientCredentials passed during initialization and provides full TypeScript type definitions for static type-checking and IDE autocompletion.

**Human URL:** [https://developer.adobe.com/firefly-services/docs/guides/sdks/](https://developer.adobe.com/firefly-services/docs/guides/sdks/)


#### Tags:

 - SDK, Node.js, TypeScript, NPM, Client Library

#### Properties

- [Documentation](https://developer.adobe.com/firefly-services/docs/guides/sdks/)
- [GitHubRepository](https://github.com/Firefly-Services/firefly-services-sdk-js)
- [NPMPackage](https://www.npmjs.com/package/@adobe/photoshop-apis)

### Adobe Photoshop UXP Plugin API
The modern plugin development platform for Photoshop, replacing the legacy CEP framework. UXP (Unified Extensibility Platform) is powered by a V8 JavaScript engine supporting ES6+ and provides Spectrum design components for building panels and dialogs using HTML, CSS, and modern JavaScript. Plugins access a rich Photoshop DOM API for interacting with documents, layers, and actions, along with platform APIs for file system access, network I/O, clipboard operations, and more. The batchPlay interface enables sending action descriptors directly to Photoshop's event queue for advanced automation.

**Human URL:** [https://developer.adobe.com/photoshop/uxp/2022/](https://developer.adobe.com/photoshop/uxp/2022/)


#### Tags:

 - Plugin Platform, JavaScript, HTML/CSS, DOM API, Desktop, Spectrum UI

#### Properties

- [Documentation](https://developer.adobe.com/photoshop/uxp/2022/)
- [APIReference](https://developer.adobe.com/photoshop/uxp/2022/ps_reference/)
- [APIReference](https://developer.adobe.com/photoshop/uxp/2022/uxp-api/)
- [GettingStarted](https://developer.adobe.com/photoshop/uxp/2022/guides/)
- [JSONSchema](json-schema/adobe-photoshop-uxp-plugin-manifest-schema.json)

### Adobe Photoshop UXP Scripting
A modern scripting system for Photoshop that allows developers to execute standalone JavaScript files with the .psjs extension to automate tasks. Unlike full UXP plugins, scripts are single files that run once and complete, similar to the legacy ExtendScript workflow but using modern JavaScript powered by the V8 engine. UXP scripts access the same Photoshop DOM API and platform APIs as UXP plugins, enabling document manipulation, layer management, and batch processing without building a full plugin UI. Available since Photoshop 23.5.

**Human URL:** [https://developer.adobe.com/photoshop/uxp/2022/scripting/](https://developer.adobe.com/photoshop/uxp/2022/scripting/)


#### Tags:

 - Scripting, JavaScript, Automation, Modern JS

#### Properties

- [Documentation](https://developer.adobe.com/photoshop/uxp/2022/scripting/)
- [APIReference](https://developer.adobe.com/photoshop/uxp/2022/ps_reference/media/uxpscripting/)

### Adobe Photoshop UXP Hybrid Plugins
A specialized plugin type that combines UXP's JavaScript, HTML, and CSS plugin framework with native C++ code compiled as a .uxpaddon. This allows developers to write performance-critical code in C++ such as pixel-level image processing while using UXP for the user interface layer. Hybrid plugins can integrate with the traditional Photoshop C++ SDK to create filters that appear in Photoshop's Filter menu or implement new file format support. Requires Photoshop v24.2.0 or later.

**Human URL:** [https://developer.adobe.com/photoshop/uxp/2022/guides/hybrid-plugins/](https://developer.adobe.com/photoshop/uxp/2022/guides/hybrid-plugins/)


#### Tags:

 - Plugin, C++, Hybrid, Native Code, Performance, Filters

#### Properties

- [Documentation](https://developer.adobe.com/photoshop/uxp/2022/guides/hybrid-plugins/)
- [GettingStarted](https://developer.adobe.com/photoshop/uxp/2022/guides/hybrid-plugins/getting-started/)
- [APIReference](https://developer.adobe.com/photoshop/uxp/2022/ps_reference/media/cpp-pluginsdk/)

### Adobe Photoshop C++ Plugin SDK
A C++ based SDK for building low-level native Photoshop plugins. The SDK enables developers to extend Photoshop in seven categories including filters appearing under the Filter menu, file format import and export support, selection tools, color pickers, automation plugins, measurement tools, and 3D import and export. It provides direct access to Photoshop's internal pixel data and rendering pipeline for maximum performance. While still supported, Adobe recommends UXP Hybrid Plugins for new development that requires native C++ capabilities.

**Human URL:** [https://developer.adobe.com/photoshop/](https://developer.adobe.com/photoshop/)


#### Tags:

 - C++, Native SDK, Filters, File Formats, Desktop

#### Properties

- [Documentation](https://developer.adobe.com/photoshop/)
- [GitHubRepository](https://github.com/AdobeDocs/photoshop-cpp-sdk)

### Adobe Photoshop ExtendScript Scripting API
The legacy scripting system based on ExtendScript, Adobe's implementation of ECMAScript 3. ExtendScript scripts use the .jsx file extension and can automate nearly all Photoshop operations through a comprehensive Application, Document, and Layer object model. Scripts can also be written in AppleScript on macOS or VBScript on Windows. While ExtendScript scripts still function in current Photoshop versions, Adobe recommends migrating to UXP scripting for modern JavaScript support and provides a conversion utility to help transform ExtendScript code to batchPlay-based UXP code.

**Human URL:** [https://extendscript.docsforadobe.dev/](https://extendscript.docsforadobe.dev/)


#### Tags:

 - Legacy, Scripting, ExtendScript, JSX, Automation

#### Properties

- [Documentation](https://extendscript.docsforadobe.dev/)
- [Documentation](https://developer.adobe.com/photoshop/uxp/2022/guides/uxp_for_you/uxp_for_extendscript_devs/)
- [GitHubRepository](https://github.com/adobe-uxp/ps-es-to-uxp)

## Common Properties

- [Portal](https://developer.adobe.com/photoshop/)
- [Documentation](https://developer.adobe.com/firefly-services/docs/photoshop/)
- [Documentation](https://developer.adobe.com/photoshop/uxp/2022/)
- [GettingStarted](https://developer.adobe.com/firefly-services/docs/photoshop/getting_started/)
- [Portal](https://developer.adobe.com/developer-console/)
- [APIReference](https://developer.adobe.com/firefly-services/docs/photoshop/api/)
- [Documentation](https://developer.adobe.com/firefly-services/docs/guides/sdks/)
- [GitHubRepository](https://github.com/Firefly-Services/firefly-services-sdk-js)
- [GitHubRepository](https://github.com/AdobeDocs/photoshop-cpp-sdk)
- [Website](https://www.adobe.com/products/photoshop.html)
- [Blog](https://blog.developer.adobe.com/)
- [Forum](https://community.adobe.com/t5/photoshop-ecosystem-discussions/bd-p/photoshop)
- [Forum](https://forums.creativeclouddeveloper.com)
- [Status](https://status.adobe.com/)
- [Security](https://helpx.adobe.com/security/products/photoshop.html)
- [X](https://x.com/Photoshop)
- [YouTube](https://www.youtube.com/@AdobeCreativeCloud)
- [TermsOfService](https://www.adobe.com/legal/terms.html)
- [PrivacyPolicy](https://www.adobe.com/privacy/policy.html)
- [License](https://www.adobe.com/legal/licenses-terms.html)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
