---
order: 0
title: Ant Design of Blazor
---

Following the Ant Design specification, we developed a Blazor Components library `ant-design-blazor` that contains a set of high quality components and demos for building rich, interactive user interfaces.

<div class="pic-plus">
  <img width="150" src="https://gw.alipayobjects.com/zos/rmsportal/KDpgvguMpGfqaHPjicRK.svg">
  <span>+</span>
  <img height="150" src="https://raw.githubusercontent.com/ant-design-blazor/ant-design-blazor/master/docs/assets/blazor.svg">
</div>

<style>
.pic-plus > * {
  display: inline-block !important;
  vertical-align: middle;
}
.pic-plus span {
  font-size: 30px;
  color: #aaa;
  margin: 0 20px;
}
</style>

## ✨ Features

- 🌈 Enterprise-class UI interactive language and visual style.
- 📦 A set of high-quality Blazor components out of the box.
- 💕 Supports WebAssembly-based client-side and SignalR-based server-side UI event interaction.
- 🎨 Supports Progressive Web Applications (PWA).
- 🛡 Build with C#, a multi-paradigm static language for an efficient development experience.
- 🌍 Internationalization support for dozens of languages.
- 🎁 Seamless integration with existing ASP.NET Core MVC and Razor Pages projects.

## 🌈 Online Examples

WebAssembly static hosting examples:

- [Azure Static WebApp](https://antblazor.com/)

## 🖥 Environment Support

- Supports .NET Core 3.1 / .NET 5 / .NET 6 / .Net 7 / .NET 8.
- Supports WebAssembly static file deployment.
- Supports 4 major browsers engines, and Internet Explorer 11+ ([Blazor Server](https://docs.microsoft.com/en-us/aspnet/core/blazor/supported-platforms?view=aspnetcore-6.0&WT.mc_id=DT-MVP-5003987) only)
- Supports [.NET MAUI](https://dotnet.microsoft.com/zh-cn/apps/maui?WT.mc_id=DT-MVP-5003987) / [WPF](https://docs.microsoft.com/en-us/aspnet/core/blazor/hybrid/tutorials/wpf?view=aspnetcore-6.0&WT.mc_id=DT-MVP-5003987) / [Windows Forms](https://docs.microsoft.com/en-us/aspnet/core/blazor/hybrid/tutorials/windows-forms?view=aspnetcore-6.0) and other Blazor Hybrid workloads.
- Supports [Electron](http://electron.atom.io/) and other Web standards-based environments.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br> Edge / IE | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/opera/opera_48x48.png" alt="Opera" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Opera | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/electron/electron_48x48.png" alt="Electron" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Electron |
| :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                                                                                                 Edge 16 / IE 11†                                                                                                 |                                                                                                        522                                                                                                        |                                                                                                      57                                                                                                       |                                                                                                      11                                                                                                       |                                                                                                    44                                                                                                     |                                                                                                      Chromium 57                                                                                                      |

> Due to [WebAssembly](https://webassembly.org) restriction, Blazor WebAssembly doesn't support IE browser, but Blazor Server supports IE 11† with additional polyfills. See [official documentation](https://docs.microsoft.com/en-us/aspnet/core/blazor/supported-platforms?view=aspnetcore-3.1&WT.mc_id=DT-MVP-5003987).

> From .NET 5, IE 11 is no longer officially supported. See [Blazor: Updated browser support](https://docs.microsoft.com/en-us/dotnet/core/compatibility/aspnet-core/5.0/blazor-browser-support-updated). Unofficial support is provided by [Blazor.Polyfill](https://github.com/Daddoon/Blazor.Polyfill) community project.

## 💿 Current Version

- Release: [![AntDesign](https://img.shields.io/nuget/v/AntDesign.svg?color=red&style=flat-square)](https://www.nuget.org/packages/AntDesign/)
- Development: [![AntDesign](https://img.shields.io/nuget/vpre/AntDesign.svg?color=red&style=flat-square)](https://www.nuget.org/packages/AntDesign/)

## 🎨 Design Specification

Regularly synchronize with Official Ant Design specifications, you can check the [sync logs](https://github.com/ant-design-blazor/ant-design-blazor/actions?query=workflow%3A%22Style+sync+Bot%22) online.

**Before the 1.0 release, we will only sync antd 4.x styles.**

## 📦 Installation Guide

- Install [.NET Core SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1?WT.mc_id=DT-MVP-5003987) 3.1.300 or later, .NET 8 is even better.

### Create a new project from the dotnet new template

We have provided the `dotnet new` template to create a [Boilerplate](https://github.com/ant-design-blazor/ant-design-pro-blazor) project out of the box：

- Install the template

  ```bash
  $ dotnet new --install AntDesign.Templates
  ```

- Create the Boilerplate project with the template

  ```bash
  $ dotnet new antdesign -o MyAntDesignApp
  ```

Options for the template：

| Options          | Description                                         | Type     | Default    |
| ---------------- | -------------------------------------------- | ------ |  --------- |
| `-f` \| `--full`  | If specified, generates all pages of ant design pro | bool  |  false    |
| `-ho` \| `--host`   | Specify the hosting model  | 'wasm' \| 'server' \| 'hosted'    |'wasm'      |
| `--no-restore` |  If specified, skips the automatic restore of the project on create  | bool    | false |



### Import Ant Design Blazor into an existing project

- Go to the project folder of the application and install the Nuget package reference

  ```bash
  $ dotnet add package AntDesign
  ```

- Register the services

  ```csharp
  services.AddAntDesign();
  ```

- Link the static files in `wwwroot/index.html` (WebAssembly) or `Pages/_Host.cshtml` (Server)

  ```html
  <link href="_content/AntDesign/css/ant-design-blazor.css" rel="stylesheet" />
  <script src="_content/AntDesign/js/ant-design-blazor.js"></script>
  ```

- Add namespace in `_Imports.razor`

  ```csharp
  @using AntDesign
  ```

- To display the pop-up component dynamically, you need to add the `<AntContainer />` component in `App.razor`. 

  ```
  <Router AppAssembly="@typeof(MainLayout).Assembly">
      <Found Context="routeData">
          <RouteView RouteData="routeData" DefaultLayout="@typeof(MainLayout)" />
      </Found>
      <NotFound>
          <LayoutView Layout="@typeof(MainLayout)">
              <Result Status="404" />
          </LayoutView>
      </NotFound>
  </Router>

  <AntContainer />   <-- add this component ✨
  ```

- Finally, it can be referenced in the `.razor' component!

  ```html
  <Button Type="primary">Hello World!</Button>
  ```

## 🔨 Local Development

- Install [.NET Core SDK](https://dotnet.microsoft.com/download/dotnet/8.0?WT.mc_id=DT-MVP-5003987) 8.0.x or later.
- Install Node.js (only for building style files and interoperable TypeScript files)
- Clone to local development

  ```bash
  $ git clone git@github.com:ant-design-blazor/ant-design-blazor.git
  $ cd ant-design-blazor
  $ npm install
  $ dotnet build ./site/AntDesign.Docs.Build/AntDesign.Docs.Build.csproj
  $ npm start
  ```

- Visit https://localhost:5001 in your supported browser and check [local development documentation](https://github.com/ant-design-blazor/ant-design-blazor/wiki) for details.

  > Visual Studio 2022 is recommended for development.

## 🔗 Links

- [Official Blazor Documentation](https://docs.microsoft.com/en-us/aspnet/core/blazor/?WT.mc_id=DT-MVP-5003987)
- [MS Learn for Blazor Tutorial](https://docs.microsoft.com/en-us/learn/modules/build-blazor-webassembly-visual-studio-code/?WT.mc_id=DT-MVP-5003987)

## 🤝 Contributing

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/ant-design-blazor/ant-design-blazor/pulls)

If you would like to contribute, feel free to create a [Pull Request](https://github.com/ant-design-blazor/ant-design-blazor/pulls), or give us [Bug Report](https://github.com/ant-design-blazor/ant-design-blazor/issues/new).

## ❓ Community Support

If you encounter any problems in the process, feel free to ask for help via following channels. We also encourage experienced users to help newcomers.

- [![Discord Server](https://img.shields.io/discord/753358910341251182?color=%237289DA&label=AntBlazor&logo=discord&logoColor=white&style=flat-square)](https://discord.com/invite/jqu3Xeq)

## ☀️ License

[![AntDesign](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](https://github.com/ant-design-blazor/ant-design-blazor/blob/master/LICENSE)
