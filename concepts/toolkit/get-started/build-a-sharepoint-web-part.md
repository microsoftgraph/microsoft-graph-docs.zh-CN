---
title: 使用 Microsoft Graph 部件生成 SharePoint Toolkit
description: 开始使用 Microsoft Graph Toolkit生成 SharePoint Web 部件。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d07a597c69ae998c75e3d4698cb0513cff056e56
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659748"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="6ccf6-103">使用 Microsoft Graph 部件生成 SharePoint Toolkit</span><span class="sxs-lookup"><span data-stu-id="6ccf6-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="6ccf6-104">本主题介绍如何使用 Microsoft Graph Toolkit SharePoint 客户端 Web [部件中的组件](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="6ccf6-105">入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="6ccf6-106">设置开发环境并创建 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-106">Set up your development environment and create a web part.</span></span>
2. <span data-ttu-id="6ccf6-107">更新项目中的 TypeScript。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-107">Update TypeScript in your project.</span></span>
3. <span data-ttu-id="6ccf6-108">添加 Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="6ccf6-109">添加 SharePoint 提供程序。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-109">Add the SharePoint Provider.</span></span>
5. <span data-ttu-id="6ccf6-110">添加组件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-110">Add components.</span></span>
6. <span data-ttu-id="6ccf6-111">配置权限。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-111">Configure permissions.</span></span>
7. <span data-ttu-id="6ccf6-112">生成和部署 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-112">Build and deploy your web part.</span></span>
8. <span data-ttu-id="6ccf6-113">测试 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="6ccf6-114">设置 SharePoint 框架开发环境并创建新的 Web 部件</span><span class="sxs-lookup"><span data-stu-id="6ccf6-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="6ccf6-115">按照步骤设置[SharePoint 框架开发环境，](/sharepoint/dev/spfx/set-up-your-development-environment)[然后创建新的 Web 部件](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="update-typescript-in-your-project"></a><span data-ttu-id="6ccf6-116">更新项目中的 TypeScript</span><span class="sxs-lookup"><span data-stu-id="6ccf6-116">Update TypeScript in your project</span></span>

<span data-ttu-id="6ccf6-117">Microsoft Graph Toolkit Typescript 3.x。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-117">The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="6ccf6-118">在将Toolkit项目之前，请确保你使用的是支持的 [Typescript 版本](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-118">Before adding the Toolkit to your project, make sure you're using a [supported version of Typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span> <span data-ttu-id="6ccf6-119">例如，若要添加 Typescript 3.7，请使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-119">For example, to add Typescript 3.7, use the following command:</span></span>

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
<span data-ttu-id="6ccf6-120">然后，在 `tsconfig.json` 项目文件夹中找到该文件，打开该文件，然后查找以下行：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-120">Then, locate the `tsconfig.json` file in your project folder, open the file, and look for this line:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
<span data-ttu-id="6ccf6-121">将该行替换为：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-121">Replace the line with:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="6ccf6-122">添加 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="6ccf6-122">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="6ccf6-123">通过以下Toolkit安装 Microsoft Graph Toolkit npm 包和填充：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-123">Install the Microsoft Graph Toolkit npm package and polyfills with the following command:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="6ccf6-124">如果计划在 Web 部件中支持 IE11，则需要执行其他步骤以确保跨浏览器兼容性：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-124">If you plan to support IE11 in your web parts, you'll need to follow additional steps to ensure cross-browser compatibility:</span></span>

1. <span data-ttu-id="6ccf6-125">安装以下程序包：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-125">Install the following packages:</span></span>
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. <span data-ttu-id="6ccf6-126">将以下代码添加到 `gulpfile.js` 正上方 `build.initialize(gulp)` ：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-126">Add the following code to `gulpfile.js`, right above `build.initialize(gulp)`:</span></span>
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
3. <span data-ttu-id="6ccf6-127">在文件中，在 SharePoint 提供程序下一步 `src\webparts\<your-project>\<your-web-part>.ts` 中导入以下填充。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-127">In your `src\webparts\<your-project>\<your-web-part>.ts` file, import the following polyfills before the SharePoint provider in the next step.</span></span>

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

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="6ccf6-128">添加 SharePoint 提供程序</span><span class="sxs-lookup"><span data-stu-id="6ccf6-128">Add the SharePoint Provider</span></span>

<span data-ttu-id="6ccf6-129">Microsoft Graph Toolkit提供程序为组件启用身份验证并访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-129">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="6ccf6-130">若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="6ccf6-130">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="6ccf6-131">SharePoint Web 部件始终存在于经过身份验证的上下文中，因为用户已经必须登录才能访问承载 Web 部件的页面。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-131">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="6ccf6-132">使用此上下文初始化 [SharePoint 提供程序](../providers/sharepoint.md)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-132">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="6ccf6-133">首先，将提供程序添加到 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-133">First, add the provider to your web part.</span></span> <span data-ttu-id="6ccf6-134">在项目文件夹中找到该文件，将以下行添加到文件顶部，位于现有语句 `src\webparts\<your-project>\<your-web-part>.ts` `import` 的正下方：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-134">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

<span data-ttu-id="6ccf6-135">接下来，您需要在 Web 部件的方法内使用经过身份验证的上下文初始化 `onInit()` 提供程序。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-135">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="6ccf6-136">在同一文件中，将以下代码添加到该行 `public render(): void {` 的正前：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-136">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a><span data-ttu-id="6ccf6-137">添加组件</span><span class="sxs-lookup"><span data-stu-id="6ccf6-137">Add components</span></span>

<span data-ttu-id="6ccf6-138">现在，你可以开始向 Web 部件添加组件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-138">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="6ccf6-139">只需将组件添加到方法内的 HTML，组件将使用 `render()` SharePoint 上下文访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-139">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="6ccf6-140">例如，若要添加 [Person 组件](../components/person.md)，代码将如下所示：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-140">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a><span data-ttu-id="6ccf6-141">配置权限</span><span class="sxs-lookup"><span data-stu-id="6ccf6-141">Configure permissions</span></span>

<span data-ttu-id="6ccf6-142">若要从 SharePoint 框架应用程序调用 Microsoft Graph，需要在解决方案包中请求所需的权限，并且 Microsoft 365 租户管理员需要批准请求的权限。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-142">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="6ccf6-143">若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 该文件并设置：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-143">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="6ccf6-144">在该行正下方，添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-144">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="6ccf6-145">根据你使用的组件确定你需要哪些 Microsoft Graph API 权限。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-145">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="6ccf6-146">每个组件的文档页都提供组件所需的权限列表。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-146">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="6ccf6-147">您需要将所需的每个权限添加到 `webApiPermissionRequests` 。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-147">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="6ccf6-148">例如，如果你使用的是"人员"组件和"议程"组件，可能 `webApiPermissionRequests` 如下所示：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-148">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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
## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="6ccf6-149">生成和部署 Web 部件</span><span class="sxs-lookup"><span data-stu-id="6ccf6-149">Build and deploy your web part</span></span>

<span data-ttu-id="6ccf6-150">现在，将生成应用程序，并部署到 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-150">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="6ccf6-151">通过运行以下命令生成应用程序：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-151">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="6ccf6-152">该 `sharepoint/solution` 文件夹中有一个新 `.sppkg` 文件。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-152">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="6ccf6-153">您需要将此文件上载到 SharePoint Online 应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-153">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="6ccf6-154">转到 [SharePoint 管理中心的"更多功能"页](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-154">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="6ccf6-155">选择 **"应用程序\*\*\*\*"下的"打开"，** 然后单击 **"应用程序目录\*\*\*\*"，然后分发 SharePoint 应用程序**。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-155">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="6ccf6-156">上载文件 `.sppkg` ，然后单击"部署 **"。**</span><span class="sxs-lookup"><span data-stu-id="6ccf6-156">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="6ccf6-157">接下来，您需要以管理员角色批准权限。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-157">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="6ccf6-158">转到 **SharePoint 管理中心**。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-158">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="6ccf6-159">在左侧导航栏中，选择 **"高级**"，然后选择 **"API Access"。**</span><span class="sxs-lookup"><span data-stu-id="6ccf6-159">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="6ccf6-160">应看到针对在文件中添加的每个权限的挂起 `config\package-solution.json` 请求。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-160">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="6ccf6-161">选择并批准每个权限。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-161">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="6ccf6-162">测试 Web 部件</span><span class="sxs-lookup"><span data-stu-id="6ccf6-162">Test your web part</span></span>

<span data-ttu-id="6ccf6-163">现在可以将 Web 部件添加到 SharePoint 页面并进行测试。你将需要使用托管的工作台来测试使用 Microsoft Graph Toolkit因为组件需要经过身份验证的上下文才能调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-163">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="6ccf6-164">您可以在 **https：//<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx** 找到托管的工作台。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-164">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="6ccf6-165">打开项目中的文件，将值替换为托管工作台的 `config\serve.json` `initialPage` URL：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-165">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="6ccf6-166">保存该文件，然后在控制台中运行以下命令以生成和预览 Web 部件：</span><span class="sxs-lookup"><span data-stu-id="6ccf6-166">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="6ccf6-167">托管的工作台将自动在浏览器中打开。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-167">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="6ccf6-168">将 Web 部件添加到页面，你应该会看到你的 Web 部件与 Microsoft Graph Toolkit组件在操作！</span><span class="sxs-lookup"><span data-stu-id="6ccf6-168">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="6ccf6-169">只要 gulp serve 命令仍在控制台中运行，就可以继续编辑代码，然后刷新浏览器以查看更改。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-169">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6ccf6-170">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6ccf6-170">Next Steps</span></span>
- <span data-ttu-id="6ccf6-171">请查看此有关生成 SharePoint Web 部件 [分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-171">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="6ccf6-172">尝试在运动场 [中的组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="6ccf6-173">在 Stack [Overflow](https://aka.ms/mgt-question)上提问。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-173">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="6ccf6-174">在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="6ccf6-174">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>