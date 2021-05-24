---
title: 使用 Microsoft SharePoint生成 web Graph Toolkit
description: 开始使用 Microsoft Graph Toolkit生成 SharePoint Web 部件。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c1f4be864c9e762e164980bc20abb4195df5c9f7
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629131"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="cd5f9-103">使用 Microsoft SharePoint生成 web Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="cd5f9-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cd5f9-104">本主题介绍如何使用 Microsoft Graph Toolkit客户端 Web SharePoint[中的组件](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="cd5f9-105">入门包括以下步骤：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="cd5f9-106">设置开发环境并创建 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-106">Set up your development environment and create a web part.</span></span>
1. <span data-ttu-id="cd5f9-107">添加 Microsoft Graph Toolkit SharePoint 框架程序包。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-107">Add the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="cd5f9-108">添加SharePoint提供程序。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-108">Add the SharePoint Provider.</span></span>
1. <span data-ttu-id="cd5f9-109">添加组件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-109">Add components.</span></span>
1. <span data-ttu-id="cd5f9-110">配置权限。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-110">Configure permissions.</span></span>
1. <span data-ttu-id="cd5f9-111">部署 Microsoft Graph Toolkit SharePoint 框架程序包。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-111">Deploy the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="cd5f9-112">生成和部署 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-112">Build and deploy your web part.</span></span>
1. <span data-ttu-id="cd5f9-113">测试 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="cd5f9-114">设置开发SharePoint 框架并创建新的 Web 部件</span><span class="sxs-lookup"><span data-stu-id="cd5f9-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="cd5f9-115">按照步骤设置[开发SharePoint 框架，](/sharepoint/dev/spfx/set-up-your-development-environment)然后[创建新的 Web 部件](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="cd5f9-116">添加 Microsoft Graph Toolkit SharePoint 框架包</span><span class="sxs-lookup"><span data-stu-id="cd5f9-116">Add the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="cd5f9-117">若要防止多个 SharePoint 框架 组件在页面上注册自己的一组 Microsoft Graph Toolkit 组件，您应将 Microsoft Graph Toolkit SharePoint 框架 程序包部署到租户，并引用在此程序包的解决方案中使用的 Microsoft Graph Toolkit 组件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-117">To prevent multiple SharePoint Framework components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this package.</span></span>

<span data-ttu-id="cd5f9-118">Microsoft Graph Toolkit SharePoint 框架 包包含一个SharePoint 框架库，该库在 SharePoint 中注册 Microsoft Graph Toolkit 组件的单个实例。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-118">The Microsoft Graph Toolkit SharePoint Framework package contains a SharePoint Framework library that registers a single instance of Microsoft Graph Toolkit components in SharePoint.</span></span>

<span data-ttu-id="cd5f9-119">使用下列Graph Toolkit SharePoint 框架安装 Microsoft Graph Toolkit SharePoint 框架 npm 包：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-119">Install the Microsoft Graph Toolkit SharePoint Framework npm package using the following command:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="cd5f9-120">添加SharePoint提供程序</span><span class="sxs-lookup"><span data-stu-id="cd5f9-120">Add the SharePoint Provider</span></span>

<span data-ttu-id="cd5f9-121">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="cd5f9-122">若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="cd5f9-123">SharePoint Web 部件始终存在于经过身份验证的上下文中，因为用户已经必须登录才能访问托管 Web 部件的页面。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-123">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="cd5f9-124">使用此上下文初始化SharePoint[提供程序](../providers/sharepoint.md)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-124">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="cd5f9-125">首先，将提供程序添加到 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-125">First, add the provider to your web part.</span></span> <span data-ttu-id="cd5f9-126">在项目文件夹中找到文件，将以下行添加到文件顶部，位于现有语句 `src\webparts\<your-project>\<your-web-part>.ts` `import` 的正下方：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-126">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

<span data-ttu-id="cd5f9-127">接下来，你需要在 Web 部件的方法内使用经过身份验证的上下文初始化 `onInit()` 提供程序。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-127">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="cd5f9-128">在同一文件中，将以下代码添加到 行 `public render(): void {` 的正前：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-128">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a><span data-ttu-id="cd5f9-129">添加组件</span><span class="sxs-lookup"><span data-stu-id="cd5f9-129">Add components</span></span>

<span data-ttu-id="cd5f9-130">现在，你可以开始向 Web 部件添加组件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-130">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="cd5f9-131">只需将组件添加到 方法内的 HTML，组件将使用 SharePoint 上下文访问 `render()` Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-131">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="cd5f9-132">例如，若要添加 [Person 组件](../components/person.md)，代码将如下所示：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-132">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> <span data-ttu-id="cd5f9-133">如果要使用 web 部件生成 web React，请参阅[@microsoft/mgt-spfx](./mgt-spfx.md#react)文档，了解如何使用 `@microsoft/mgt-react` 。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-133">If you're building a web part using React, see the [@microsoft/mgt-spfx docs](./mgt-spfx.md#react) to learn how to use `@microsoft/mgt-react`.</span></span>

## <a name="configure-permissions"></a><span data-ttu-id="cd5f9-134">配置权限</span><span class="sxs-lookup"><span data-stu-id="cd5f9-134">Configure permissions</span></span>

<span data-ttu-id="cd5f9-135">若要从 Graph 应用程序调用 Microsoft SharePoint 框架，您需要在解决方案包中请求所需的权限，Microsoft 365租户管理员需要批准请求的权限。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-135">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="cd5f9-136">若要将权限添加到解决方案包，请找到并打开 `config\package-solution.json` 文件并设置：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-136">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="cd5f9-137">在该行正下方，添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-137">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="cd5f9-138">根据你Graph，确定你需要哪些 Microsoft 应用 API 权限。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-138">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="cd5f9-139">每个组件的文档页都提供组件所需的权限列表。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-139">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="cd5f9-140">你需要将所需的每个权限添加到 `webApiPermissionRequests` 。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-140">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="cd5f9-141">例如，如果你使用的是人员组件和议程组件，你可能 `webApiPermissionRequests` 如下所示：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-141">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="cd5f9-142">部署 Microsoft Graph Toolkit SharePoint 框架 程序包</span><span class="sxs-lookup"><span data-stu-id="cd5f9-142">Deploy the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="cd5f9-143">在将SharePoint 框架包部署到租户之前，你需要将 Microsoft Graph Toolkit SharePoint 框架包部署到租户。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-143">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="cd5f9-144">可以从项目上的"发布"部分下载与Graph Toolkit Microsoft GitHub 版本相对应的程序包。 [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases)</span><span class="sxs-lookup"><span data-stu-id="cd5f9-144">You can download the package corresponding to the version of Microsoft Graph Toolkit that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="cd5f9-145">由于租户中只能安装 Microsoft Graph Toolkit 的 SharePoint 框架 库的一个版本，因此在解决方案中使用 Microsoft Graph Toolkit 之前，请确定组织或客户是否已部署并使用相同的版本的 SharePoint 框架 库。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-145">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

<span data-ttu-id="cd5f9-146">下载 Microsoft Graph Toolkit SharePoint 框架 .sppkg 程序包后，将其上传到 SharePoint Online 应用目录。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-146">After downloading the Microsoft Graph Toolkit SharePoint Framework .sppkg package, upload it to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="cd5f9-147">转到管理[中心的更多功能SharePoint页面](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-147">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="cd5f9-148">选择 **"应用程序**"下的"打开 **"，** 然后单击"**应用程序** 目录"，然后分配 **SharePoint。**</span><span class="sxs-lookup"><span data-stu-id="cd5f9-148">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="cd5f9-149">Upload文件 `.sppkg` ，然后单击"部署 **"。**</span><span class="sxs-lookup"><span data-stu-id="cd5f9-149">Upload your `.sppkg` file, and click **Deploy**.</span></span>

## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="cd5f9-150">生成和部署 Web 部件</span><span class="sxs-lookup"><span data-stu-id="cd5f9-150">Build and deploy your web part</span></span>

<span data-ttu-id="cd5f9-151">现在，将生成应用程序并部署到SharePoint。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-151">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="cd5f9-152">通过运行以下命令构建应用程序：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-152">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="cd5f9-153">在 `sharepoint/solution` 文件夹中，将会有一个新 `.sppkg` 文件。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-153">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="cd5f9-154">你需要将此文件上载到 SharePoint Online 应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-154">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="cd5f9-155">转到管理[中心的更多功能SharePoint页面](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-155">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="cd5f9-156">选择 **"应用程序**"下的"打开 **"，** 然后单击"**应用程序** 目录"，然后分配 **SharePoint。**</span><span class="sxs-lookup"><span data-stu-id="cd5f9-156">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="cd5f9-157">Upload文件 `.sppkg` ，然后单击"部署 **"。**</span><span class="sxs-lookup"><span data-stu-id="cd5f9-157">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="cd5f9-158">接下来，您需要以管理员角色批准权限。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-158">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="cd5f9-159">转到你的SharePoint **管理中心**。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-159">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="cd5f9-160">在左侧导航栏中，选择 **"高级"，** 然后选择 **"API 访问"。**</span><span class="sxs-lookup"><span data-stu-id="cd5f9-160">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="cd5f9-161">应看到文件中添加的每个权限的挂起 `config\package-solution.json` 请求。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-161">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="cd5f9-162">选择并批准每个权限。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-162">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="cd5f9-163">测试 Web 部件</span><span class="sxs-lookup"><span data-stu-id="cd5f9-163">Test your web part</span></span>

<span data-ttu-id="cd5f9-164">现在，你已准备好将 Web 部件添加到SharePoint并进行测试。你将需要使用托管的工作台来测试使用 Microsoft Graph Toolkit因为组件需要经过身份验证的上下文才能调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-164">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="cd5f9-165">可在 **https：//<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx 找到托管的工作台**。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-165">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="cd5f9-166">打开 `config\serve.json` 项目中的文件，将 的值替换为 `initialPage` 托管工作台的 url：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-166">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="cd5f9-167">保存文件，然后在控制台中运行以下命令以生成和预览 Web 部件：</span><span class="sxs-lookup"><span data-stu-id="cd5f9-167">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="cd5f9-168">托管的工作台将自动在浏览器中打开。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-168">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="cd5f9-169">将 Web 部件添加到页面，你应该会看到 Web 部件与 Microsoft Graph Toolkit组件在操作！</span><span class="sxs-lookup"><span data-stu-id="cd5f9-169">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="cd5f9-170">只要 gulp serve 命令仍在控制台中运行，就可以继续编辑代码，然后仅刷新浏览器以查看更改。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-170">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cd5f9-171">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cd5f9-171">Next Steps</span></span>
- <span data-ttu-id="cd5f9-172">请查看此有关生成 web 部件SharePoint[分步教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-172">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="cd5f9-173">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="cd5f9-174">在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。</span><span class="sxs-lookup"><span data-stu-id="cd5f9-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="cd5f9-175">报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="cd5f9-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
