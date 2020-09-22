---
title: 使用 Microsoft Graph 工具包生成 SharePoint web 部件
description: 开始使用 Microsoft Graph 工具包生成 SharePoint web 部件。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: bdc2d6679c145f3f50d908bbf0e4e417234c4dc9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059648"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="4918b-103">使用 Microsoft Graph 工具包生成 SharePoint web 部件</span><span class="sxs-lookup"><span data-stu-id="4918b-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4918b-104">本主题介绍如何在 [SharePoint 客户端 web 部件](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)中使用 Microsoft Graph 工具包组件。</span><span class="sxs-lookup"><span data-stu-id="4918b-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="4918b-105">入门涉及以下步骤：</span><span class="sxs-lookup"><span data-stu-id="4918b-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="4918b-106">设置开发环境并创建 web 部件。</span><span class="sxs-lookup"><span data-stu-id="4918b-106">Set up your development environment and create a web part.</span></span>
2. <span data-ttu-id="4918b-107">更新项目中的 TypeScript。</span><span class="sxs-lookup"><span data-stu-id="4918b-107">Update TypeScript in your project.</span></span>
3. <span data-ttu-id="4918b-108">添加 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="4918b-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="4918b-109">添加 SharePoint 提供程序。</span><span class="sxs-lookup"><span data-stu-id="4918b-109">Add the SharePoint Provider.</span></span>
5. <span data-ttu-id="4918b-110">添加组件。</span><span class="sxs-lookup"><span data-stu-id="4918b-110">Add components.</span></span>
6. <span data-ttu-id="4918b-111">配置权限。</span><span class="sxs-lookup"><span data-stu-id="4918b-111">Configure permissions.</span></span>
7. <span data-ttu-id="4918b-112">生成和部署 web 部件。</span><span class="sxs-lookup"><span data-stu-id="4918b-112">Build and deploy your web part.</span></span>
8. <span data-ttu-id="4918b-113">测试 web 部件。</span><span class="sxs-lookup"><span data-stu-id="4918b-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="4918b-114">设置 SharePoint 框架开发环境并创建新的 web 部件</span><span class="sxs-lookup"><span data-stu-id="4918b-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="4918b-115">按照 [设置 SharePoint 框架开发环境](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-development-environment) 的步骤操作，然后 [创建一个新的 web 部件](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。</span><span class="sxs-lookup"><span data-stu-id="4918b-115">Follow the steps to [Set up your SharePoint Framework development environment](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="update-typescript-in-your-project"></a><span data-ttu-id="4918b-116">更新项目中的 TypeScript</span><span class="sxs-lookup"><span data-stu-id="4918b-116">Update TypeScript in your project</span></span>

<span data-ttu-id="4918b-117">Microsoft Graph 工具包需要 Typescript 3. x。</span><span class="sxs-lookup"><span data-stu-id="4918b-117">The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="4918b-118">将工具包添加到项目之前，请确保使用 [的是受支持的 Typescript 版本](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。</span><span class="sxs-lookup"><span data-stu-id="4918b-118">Before adding the Toolkit to your project, make sure you're using a [supported version of Typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span> <span data-ttu-id="4918b-119">例如，若要添加 Typescript 3.7，请使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="4918b-119">For example, to add Typescript 3.7, use the following command:</span></span>

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
<span data-ttu-id="4918b-120">然后， `tsconfig.json` 在项目文件夹中找到该文件，打开该文件，然后查找此行：</span><span class="sxs-lookup"><span data-stu-id="4918b-120">Then, locate the `tsconfig.json` file in your project folder, open the file, and look for this line:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
<span data-ttu-id="4918b-121">将此行替换为：</span><span class="sxs-lookup"><span data-stu-id="4918b-121">Replace the line with:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="4918b-122">添加 Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="4918b-122">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4918b-123">使用以下命令安装 Microsoft Graph 工具包 npm 包和 polyfills.ts：</span><span class="sxs-lookup"><span data-stu-id="4918b-123">Install the Microsoft Graph Toolkit npm package and polyfills with the following command:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="4918b-124">如果您计划在 web 部件中支持 IE11，则需要执行其他步骤以确保跨浏览器的兼容性：</span><span class="sxs-lookup"><span data-stu-id="4918b-124">If you plan to support IE11 in your web parts, you'll need to follow additional steps to ensure cross-browser compatibility:</span></span>

1. <span data-ttu-id="4918b-125">安装以下程序包：</span><span class="sxs-lookup"><span data-stu-id="4918b-125">Install the following packages:</span></span>
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. <span data-ttu-id="4918b-126">将以下代码添加到 `gulpfile.js` 中，请在上面添加 `build.initialize(gulp)` ：</span><span class="sxs-lookup"><span data-stu-id="4918b-126">Add the following code to `gulpfile.js`, right above `build.initialize(gulp)`:</span></span>
```ts
build.configureWebpack.mergeConfig({
  additionalConfiguration: (generatedConfiguration) => {
    generatedConfiguration.module.rules.push(
      {
        test: /\.m?js$/, use:
        {
          loader: "babel-loader",
          options:
          {
            presets: [["@babel/preset-env",
              {
                targets: {
                  "ie": "11"
                }
              }]]
          }
        }
      }
    );

    return generatedConfiguration;
  }
});
```
3. <span data-ttu-id="4918b-127">在您的 `src\webparts\<your-project>\<your-web-part>.ts` 文件中，在下一步中将以下 polyfills.ts 导入到 SharePoint 提供程序之前。</span><span class="sxs-lookup"><span data-stu-id="4918b-127">In your `src\webparts\<your-project>\<your-web-part>.ts` file, import the following polyfills before the SharePoint provider in the next step.</span></span>

```ts
import 'regenerator-runtime/runtime';
import 'core-js/es/number';
import 'core-js/es/math';
import 'core-js/es/string';
import 'core-js/es/date';
import 'core-js/es/array';
import 'core-js/es/regexp';
import '@webcomponents/webcomponentsjs/webcomponents-bundle.js';
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="4918b-128">添加 SharePoint 提供程序</span><span class="sxs-lookup"><span data-stu-id="4918b-128">Add the SharePoint Provider</span></span>

<span data-ttu-id="4918b-129">Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="4918b-129">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="4918b-130">若要了解详细信息，请参阅 [使用提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="4918b-130">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="4918b-131">SharePoint web 部件始终存在于已验证的上下文中，因为用户已必须登录才能转到承载 web 部件的页面。</span><span class="sxs-lookup"><span data-stu-id="4918b-131">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="4918b-132">使用此上下文初始化 [SharePoint 提供程序](../providers/sharepoint.md)。</span><span class="sxs-lookup"><span data-stu-id="4918b-132">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="4918b-133">首先，将提供程序添加到 web 部件中。</span><span class="sxs-lookup"><span data-stu-id="4918b-133">First, add the provider to your web part.</span></span> <span data-ttu-id="4918b-134">`src\webparts\<your-project>\<your-web-part>.ts`在项目文件夹中找到该文件，并将以下行添加到文件顶部，并在现有语句的正下方 `import` ：</span><span class="sxs-lookup"><span data-stu-id="4918b-134">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

<span data-ttu-id="4918b-135">接下来，您需要使用 web 部件的方法内的经过身份验证的上下文初始化提供程序 `onInit()` 。</span><span class="sxs-lookup"><span data-stu-id="4918b-135">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="4918b-136">在同一文件中，将以下代码添加到行的前面 `public render(): void {` ：</span><span class="sxs-lookup"><span data-stu-id="4918b-136">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a><span data-ttu-id="4918b-137">添加组件</span><span class="sxs-lookup"><span data-stu-id="4918b-137">Add components</span></span>

<span data-ttu-id="4918b-138">现在，您可以开始向 web 部件中添加组件。</span><span class="sxs-lookup"><span data-stu-id="4918b-138">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="4918b-139">只需将组件添加到方法内的 HTML `render()` ，组件将使用 SharePoint 上下文来访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="4918b-139">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="4918b-140">例如，若要添加 " [人员" 组件](../components/person.md)，您的代码将如下所示：</span><span class="sxs-lookup"><span data-stu-id="4918b-140">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a><span data-ttu-id="4918b-141">配置权限</span><span class="sxs-lookup"><span data-stu-id="4918b-141">Configure permissions</span></span>

<span data-ttu-id="4918b-142">若要从 SharePoint 框架应用程序调用 Microsoft Graph，需要在解决方案包中请求所需的权限，并且 Microsoft 365 租户管理员需要批准请求的权限。</span><span class="sxs-lookup"><span data-stu-id="4918b-142">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="4918b-143">若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 文件并设置以下内容：</span><span class="sxs-lookup"><span data-stu-id="4918b-143">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="4918b-144">在该行的正下方，添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="4918b-144">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="4918b-145">根据所使用的组件，确定所需的 Microsoft Graph API 权限。</span><span class="sxs-lookup"><span data-stu-id="4918b-145">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="4918b-146">每个组件的文档页面提供组件所需权限的列表。</span><span class="sxs-lookup"><span data-stu-id="4918b-146">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="4918b-147">您需要将所需的每个权限添加到 `webApiPermissionRequests` 。</span><span class="sxs-lookup"><span data-stu-id="4918b-147">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="4918b-148">例如，如果您使用的是 "人员" 组件和 "议程" 组件， `webApiPermissionRequests` 可能如下所示：</span><span class="sxs-lookup"><span data-stu-id="4918b-148">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

```json
"webApiPermissionRequests": [
  {
    "resource": "Microsoft Graph",
    "scope": "User.Read"
  },
  {
    "resource": "Microsoft Graph",
    "scope": "Calendars.Read"
  }
]
```
## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="4918b-149">生成和部署 web 部件</span><span class="sxs-lookup"><span data-stu-id="4918b-149">Build and deploy your web part</span></span>

<span data-ttu-id="4918b-150">现在，将生成应用程序并将其部署到 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="4918b-150">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="4918b-151">通过运行以下命令生成应用程序：</span><span class="sxs-lookup"><span data-stu-id="4918b-151">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="4918b-152">在 `sharepoint/solution` 文件夹中，将会有一个新 `.sppkg` 文件。</span><span class="sxs-lookup"><span data-stu-id="4918b-152">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="4918b-153">您需要将此文件上载到您的 SharePoint Online 应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="4918b-153">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="4918b-154">转到 [SharePoint 管理中心的 "更多功能" 页](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。</span><span class="sxs-lookup"><span data-stu-id="4918b-154">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="4918b-155">依次选择 "在**应用程序**下**打开**"、"**应用程序目录**" 和 "**分发 SharePoint 相关应用程序**"。</span><span class="sxs-lookup"><span data-stu-id="4918b-155">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="4918b-156">上传 `.sppkg` 文件，然后单击 " **部署**"。</span><span class="sxs-lookup"><span data-stu-id="4918b-156">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="4918b-157">接下来，您需要以管理员身份批准权限。</span><span class="sxs-lookup"><span data-stu-id="4918b-157">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="4918b-158">转到您的 **SharePoint 管理中心**。</span><span class="sxs-lookup"><span data-stu-id="4918b-158">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="4918b-159">在左侧导航栏中，选择 " **高级** "，然后选择 " **API 访问**"。</span><span class="sxs-lookup"><span data-stu-id="4918b-159">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="4918b-160">您应查看您在文件中添加的每个权限的挂起请求 `config\package-solution.json` 。</span><span class="sxs-lookup"><span data-stu-id="4918b-160">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="4918b-161">选择并批准每个权限。</span><span class="sxs-lookup"><span data-stu-id="4918b-161">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="4918b-162">测试 web 部件</span><span class="sxs-lookup"><span data-stu-id="4918b-162">Test your web part</span></span>

<span data-ttu-id="4918b-163">现在，您可以将 web 部件添加到 SharePoint 页面并将其测试出来。您需要使用托管的工作台测试使用 Microsoft Graph 工具包的 web 部件，因为这些组件需要经过身份验证的上下文才能调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="4918b-163">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="4918b-164">您可以在 **https://<YOUR_TENANT sharepoint.com/_layouts/15/workbench.aspx>** 找到托管的工作台。</span><span class="sxs-lookup"><span data-stu-id="4918b-164">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="4918b-165">`config\serve.json`在项目中打开文件，并将 "" 的值替换为 `initialPage` 托管的工作台的 url：</span><span class="sxs-lookup"><span data-stu-id="4918b-165">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="4918b-166">保存该文件，然后在控制台中运行以下命令，以生成并预览 web 部件：</span><span class="sxs-lookup"><span data-stu-id="4918b-166">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="4918b-167">托管的工作台将自动在浏览器中打开。</span><span class="sxs-lookup"><span data-stu-id="4918b-167">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="4918b-168">将 web 部件添加到页面中，并应在操作中看到包含 Microsoft Graph 工具包组件的 web 部件！</span><span class="sxs-lookup"><span data-stu-id="4918b-168">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="4918b-169">只要 gulp 服务命令仍在控制台中运行，您就可以继续对代码进行编辑，然后刷新浏览器以查看所做的更改。</span><span class="sxs-lookup"><span data-stu-id="4918b-169">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4918b-170">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4918b-170">Next Steps</span></span>
- <span data-ttu-id="4918b-171">请参阅本分步教程，了解如何 [生成 SharePoint web 部件](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。</span><span class="sxs-lookup"><span data-stu-id="4918b-171">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="4918b-172">尝试 [样本](https://mgt.dev)中的组件。</span><span class="sxs-lookup"><span data-stu-id="4918b-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="4918b-173">在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。</span><span class="sxs-lookup"><span data-stu-id="4918b-173">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="4918b-174">在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。</span><span class="sxs-lookup"><span data-stu-id="4918b-174">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>


