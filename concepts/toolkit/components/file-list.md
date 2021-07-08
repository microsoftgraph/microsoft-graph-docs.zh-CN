---
title: Microsoft 服务中的文件列表Graph Toolkit
description: 文件列表组件用于通过显示文件图标和名称来显示文件列表
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 816ea4b76a08d089e419aad2a126b7b39c2727b1
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334778"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="bcc76-103">Microsoft 服务中的文件列表Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bcc76-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bcc76-104">文件列表 [组件使用您](/graph/api/resources/onedrive) 指定的文件/文件夹名称、图标和其他属性显示多个文件夹和文件的列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="bcc76-105">此组件使用 [mgt 文件](./file.md) 组件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="bcc76-106">您可以指定特定驱动器或网站、根据见解类型显示文件列表 (趋势、使用或共享) ，或者提供对自定义文件列表的查询。</span><span class="sxs-lookup"><span data-stu-id="bcc76-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="bcc76-107">示例</span><span class="sxs-lookup"><span data-stu-id="bcc76-107">Example</span></span>

<span data-ttu-id="bcc76-108">以下示例使用 组件显示 `mgt-file-list` 文件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="bcc76-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="bcc76-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="bcc76-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="bcc76-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="bcc76-111">属性</span><span class="sxs-lookup"><span data-stu-id="bcc76-111">Properties</span></span>

<span data-ttu-id="bcc76-112">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="bcc76-113">属性</span><span class="sxs-lookup"><span data-stu-id="bcc76-113">Attribute</span></span> | <span data-ttu-id="bcc76-114">属性</span><span class="sxs-lookup"><span data-stu-id="bcc76-114">Property</span></span> | <span data-ttu-id="bcc76-115">说明</span><span class="sxs-lookup"><span data-stu-id="bcc76-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="bcc76-116">file-list-query</span><span class="sxs-lookup"><span data-stu-id="bcc76-116">file-list-query</span></span> | <span data-ttu-id="bcc76-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="bcc76-117">fileListQuery</span></span> | <span data-ttu-id="bcc76-118">包含要呈现的文件列表的驱动器或站点的完整查询或路径。</span><span class="sxs-lookup"><span data-stu-id="bcc76-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="bcc76-119">文件查询</span><span class="sxs-lookup"><span data-stu-id="bcc76-119">file-queries</span></span> | <span data-ttu-id="bcc76-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="bcc76-120">fileQueries</span></span> | <span data-ttu-id="bcc76-121">由组件呈现的文件查询数组。</span><span class="sxs-lookup"><span data-stu-id="bcc76-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="bcc76-122">无</span><span class="sxs-lookup"><span data-stu-id="bcc76-122">none</span></span> | <span data-ttu-id="bcc76-123">files</span><span class="sxs-lookup"><span data-stu-id="bcc76-123">files</span></span> | <span data-ttu-id="bcc76-124">用于获取或设置组件呈现的文件列表的文件数组。</span><span class="sxs-lookup"><span data-stu-id="bcc76-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="bcc76-125">使用它来访问组件加载的文件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="bcc76-126">设置此值以加载您自己的文件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="bcc76-127">insight-type</span><span class="sxs-lookup"><span data-stu-id="bcc76-127">insight-type</span></span> | <span data-ttu-id="bcc76-128">insightType</span><span class="sxs-lookup"><span data-stu-id="bcc76-128">insightType</span></span> | <span data-ttu-id="bcc76-129">设置为显示用户的趋势、使用的文件或共享文件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="bcc76-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="bcc76-130">drive-id</span></span> | <span data-ttu-id="bcc76-131">driveId</span><span class="sxs-lookup"><span data-stu-id="bcc76-131">driveId</span></span> | <span data-ttu-id="bcc76-132">文件夹所属驱动器的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcc76-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="bcc76-133">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="bcc76-134">group-id</span><span class="sxs-lookup"><span data-stu-id="bcc76-134">group-id</span></span> | <span data-ttu-id="bcc76-135">groupId</span><span class="sxs-lookup"><span data-stu-id="bcc76-135">groupId</span></span> | <span data-ttu-id="bcc76-136">文件夹所属组的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcc76-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="bcc76-137">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="bcc76-138">site-id</span><span class="sxs-lookup"><span data-stu-id="bcc76-138">site-id</span></span> | <span data-ttu-id="bcc76-139">siteId</span><span class="sxs-lookup"><span data-stu-id="bcc76-139">siteId</span></span> | <span data-ttu-id="bcc76-140">文件夹所属网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcc76-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="bcc76-141">还必须提供 或 `{item-id}` `{item-path}` 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="bcc76-142">`{list-id}`如果从特定列表引用文件，则提供 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="bcc76-143">item-id</span><span class="sxs-lookup"><span data-stu-id="bcc76-143">item-id</span></span> | <span data-ttu-id="bcc76-144">itemId</span><span class="sxs-lookup"><span data-stu-id="bcc76-144">itemId</span></span> | <span data-ttu-id="bcc76-145">文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcc76-145">ID of the folder.</span></span> <span data-ttu-id="bcc76-146">默认查询为 `/me/drive/items` 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="bcc76-147">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="bcc76-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="bcc76-148">item-path</span><span class="sxs-lookup"><span data-stu-id="bcc76-148">item-path</span></span> | <span data-ttu-id="bcc76-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="bcc76-149">itemPath</span></span> | <span data-ttu-id="bcc76-150">文件夹的项目路径 (根文件夹) 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="bcc76-151">默认查询为 `/me/drive/root` 。</span><span class="sxs-lookup"><span data-stu-id="bcc76-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="bcc76-152">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="bcc76-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="bcc76-153">页面大小</span><span class="sxs-lookup"><span data-stu-id="bcc76-153">page-size</span></span> | <span data-ttu-id="bcc76-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="bcc76-154">pageSize</span></span> | <span data-ttu-id="bcc76-155">一个数字值，指示每个页面上要呈现的最大文件数。</span><span class="sxs-lookup"><span data-stu-id="bcc76-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="bcc76-156">文件扩展名</span><span class="sxs-lookup"><span data-stu-id="bcc76-156">file-extensions</span></span> | <span data-ttu-id="bcc76-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="bcc76-157">fileExtensions</span></span> | <span data-ttu-id="bcc76-158">用于筛选要显示的文件的文件扩展名数组。</span><span class="sxs-lookup"><span data-stu-id="bcc76-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="bcc76-159">hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="bcc76-159">hide-more-files-button</span></span> | <span data-ttu-id="bcc76-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="bcc76-160">hideMoreFilesButton</span></span> | <span data-ttu-id="bcc76-161">用于指示是否显示按钮以呈现更多文件的布尔值。</span><span class="sxs-lookup"><span data-stu-id="bcc76-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="bcc76-162">下面的示例更改组件的行为，以从特定查询获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="bcc76-163">以下示例通过提供文件夹 ID，更改组件的行为，以从文件夹获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="bcc76-164">以下示例通过提供组 ID 和文件夹路径，更改组件的行为以从组提取文件列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="bcc76-165">以下示例通过提供用户 ID 和文件夹 ID，更改组件的行为以从用户获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="bcc76-166">以下示例通过提供见解类型，更改组件的行为以提取文件列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a><span data-ttu-id="bcc76-167">方法</span><span class="sxs-lookup"><span data-stu-id="bcc76-167">Methods</span></span>
| <span data-ttu-id="bcc76-168">方法</span><span class="sxs-lookup"><span data-stu-id="bcc76-168">Method</span></span> | <span data-ttu-id="bcc76-169">说明</span><span class="sxs-lookup"><span data-stu-id="bcc76-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="bcc76-170">reload (clearCache = false) </span><span class="sxs-lookup"><span data-stu-id="bcc76-170">reload(clearCache = false)</span></span> | <span data-ttu-id="bcc76-171">调用 方法，根据组件的属性使用潜在的新数据重新加载组件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-171">Call the method to reload the component with potential new data based on its properties.</span></span> <span data-ttu-id="bcc76-172">传递 `true` 以在重新加载之前清除缓存。</span><span class="sxs-lookup"><span data-stu-id="bcc76-172">Pass `true` to clear the cache before reloading.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="bcc76-173">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="bcc76-173">CSS custom properties</span></span>

<span data-ttu-id="bcc76-174">组件 `mgt-file-list` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="bcc76-174">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

```css
mgt-file-list {
  --font-family: 'Segoe UI';
  --font-size: 14px;

  --file-list-background-color: #ffffff;
  --file-list-border: none;
  --file-list-box-shadow: none;
  --file-list-padding: 4px 0;
  --file-list-margin: 0;

  --file-item-background-color--hover: rgba(0, 0, 0, 0.1);
  --file-item-background-color--active: rgba(0, 0, 0, 0.05);
  --file-item-border-radius: 2px;
  --file-item-margin: 0 4px;

  --file-item-border-top: none;
  --file-item-border-left: none;
  --file-item-border-right: none;
  --file-item-border-bottom: none;

  --show-more-button-background-color: #f3f2f1;
  --show-more-button-background-color--hover: rgba(0, 0, 0, 0.1);
  --show-more-button-font-size: 12px;
  --show-more-button-padding: 6px;
  --show-more-button-border-bottom-right-radius: 4px;
  --show-more-button-border-bottom-left-radius: 4px;
}
```

<span data-ttu-id="bcc76-175">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="bcc76-175">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="bcc76-176">Microsoft Graph API 和权限</span><span class="sxs-lookup"><span data-stu-id="bcc76-176">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="bcc76-177">配置</span><span class="sxs-lookup"><span data-stu-id="bcc76-177">Configuration</span></span> | <span data-ttu-id="bcc76-178">权限</span><span class="sxs-lookup"><span data-stu-id="bcc76-178">Permissions</span></span> | <span data-ttu-id="bcc76-179">API</span><span class="sxs-lookup"><span data-stu-id="bcc76-179">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="bcc76-180">默认 (未提供标识符或) </span><span class="sxs-lookup"><span data-stu-id="bcc76-180">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="bcc76-181">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children` |
| <span data-ttu-id="bcc76-182">提供 `{drive-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-182">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="bcc76-183">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="bcc76-184">提供 `{group-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-184">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="bcc76-185">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="bcc76-186">仅提供 `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-186">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="bcc76-187">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` |
| <span data-ttu-id="bcc76-188">提供 `{site-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-188">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="bcc76-189">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="bcc76-190">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-190">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="bcc76-191">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="bcc76-192">提供 `{drive-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-192">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="bcc76-193">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="bcc76-194">提供 `{group-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-194">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="bcc76-195">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="bcc76-196">提供 `{site-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-196">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="bcc76-197">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-197">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="bcc76-198">提供 `{user-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-198">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="bcc76-199">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-199">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="bcc76-200">仅提供 `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="bcc76-200">Provide only `{item-path}`</span></span> | <span data-ttu-id="bcc76-201">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-201">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="bcc76-202">`insight-type` 设置为趋势</span><span class="sxs-lookup"><span data-stu-id="bcc76-202">`insight-type` is set to trending</span></span> | <span data-ttu-id="bcc76-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-203">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="bcc76-204">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `trending`</span><span class="sxs-lookup"><span data-stu-id="bcc76-204">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="bcc76-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-205">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` |
| <span data-ttu-id="bcc76-206">`insight-type` 设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="bcc76-206">`insight-type` is set to `used`</span></span> | <span data-ttu-id="bcc76-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-207">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="bcc76-208">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="bcc76-208">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="bcc76-209">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-209">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="bcc76-210">`insight-type` 设置为共享</span><span class="sxs-lookup"><span data-stu-id="bcc76-210">`insight-type` is set to shared</span></span> | <span data-ttu-id="bcc76-211">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-211">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="bcc76-212">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `shared`</span><span class="sxs-lookup"><span data-stu-id="bcc76-212">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="bcc76-213">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcc76-213">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="bcc76-214">活动</span><span class="sxs-lookup"><span data-stu-id="bcc76-214">Events</span></span>

<span data-ttu-id="bcc76-215">事件</span><span class="sxs-lookup"><span data-stu-id="bcc76-215">Event</span></span> | <span data-ttu-id="bcc76-216">何时发出</span><span class="sxs-lookup"><span data-stu-id="bcc76-216">When is it emitted</span></span> | <span data-ttu-id="bcc76-217">自定义数据</span><span class="sxs-lookup"><span data-stu-id="bcc76-217">Custom data</span></span> | <span data-ttu-id="bcc76-218">Cancelable</span><span class="sxs-lookup"><span data-stu-id="bcc76-218">Cancelable</span></span> | <span data-ttu-id="bcc76-219">气泡</span><span class="sxs-lookup"><span data-stu-id="bcc76-219">Bubbles</span></span> | <span data-ttu-id="bcc76-220">使用自定义模板</span><span class="sxs-lookup"><span data-stu-id="bcc76-220">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`itemClick` | <span data-ttu-id="bcc76-221">在用户单击文件时触发。</span><span class="sxs-lookup"><span data-stu-id="bcc76-221">Fired when the user clicks a file.</span></span> | <span data-ttu-id="bcc76-222">所选 [文件](/graph/api/resources/driveItem)</span><span class="sxs-lookup"><span data-stu-id="bcc76-222">Selected [file](/graph/api/resources/driveItem)</span></span> | <span data-ttu-id="bcc76-223">否</span><span class="sxs-lookup"><span data-stu-id="bcc76-223">No</span></span> | <span data-ttu-id="bcc76-224">否</span><span class="sxs-lookup"><span data-stu-id="bcc76-224">No</span></span> | <span data-ttu-id="bcc76-225">是，使用自定义 **文件** 模板</span><span class="sxs-lookup"><span data-stu-id="bcc76-225">Yes, with custom **file** template</span></span>

<span data-ttu-id="bcc76-226">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="bcc76-226">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="bcc76-227">模板</span><span class="sxs-lookup"><span data-stu-id="bcc76-227">Templates</span></span>

<span data-ttu-id="bcc76-228">组件 `mgt-file-list` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="bcc76-228">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="bcc76-229">若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的数据类型之一。</span><span class="sxs-lookup"><span data-stu-id="bcc76-229">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="bcc76-230">数据类型</span><span class="sxs-lookup"><span data-stu-id="bcc76-230">Data type</span></span> | <span data-ttu-id="bcc76-231">数据上下文</span><span class="sxs-lookup"><span data-stu-id="bcc76-231">Data context</span></span> | <span data-ttu-id="bcc76-232">说明</span><span class="sxs-lookup"><span data-stu-id="bcc76-232">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="bcc76-233">default</span><span class="sxs-lookup"><span data-stu-id="bcc76-233">default</span></span> | <span data-ttu-id="bcc76-234">`files`：文件对象列表</span><span class="sxs-lookup"><span data-stu-id="bcc76-234">`files`: list of file objects</span></span> | <span data-ttu-id="bcc76-235">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-235">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="bcc76-236">file</span><span class="sxs-lookup"><span data-stu-id="bcc76-236">file</span></span> | <span data-ttu-id="bcc76-237">`file`：file 对象</span><span class="sxs-lookup"><span data-stu-id="bcc76-237">`file`: file object</span></span> | <span data-ttu-id="bcc76-238">用于呈现每个文件的模板。</span><span class="sxs-lookup"><span data-stu-id="bcc76-238">The template used to render each file.</span></span> |
| <span data-ttu-id="bcc76-239">no-data</span><span class="sxs-lookup"><span data-stu-id="bcc76-239">no-data</span></span> | <span data-ttu-id="bcc76-240">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="bcc76-240">No data context is passed</span></span> | <span data-ttu-id="bcc76-241">没有可用数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="bcc76-241">The template used when no data is available.</span></span> |
| <span data-ttu-id="bcc76-242">loading</span><span class="sxs-lookup"><span data-stu-id="bcc76-242">loading</span></span> | <span data-ttu-id="bcc76-243">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="bcc76-243">No data context is passed</span></span> | <span data-ttu-id="bcc76-244">组件加载状态时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="bcc76-244">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="bcc76-245">身份验证</span><span class="sxs-lookup"><span data-stu-id="bcc76-245">Authentication</span></span>

<span data-ttu-id="bcc76-246">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="bcc76-246">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="bcc76-247">缓存</span><span class="sxs-lookup"><span data-stu-id="bcc76-247">Cache</span></span>

|<span data-ttu-id="bcc76-248">对象存储</span><span class="sxs-lookup"><span data-stu-id="bcc76-248">Object store</span></span>|<span data-ttu-id="bcc76-249">缓存数据</span><span class="sxs-lookup"><span data-stu-id="bcc76-249">Cached data</span></span>|<span data-ttu-id="bcc76-250">备注</span><span class="sxs-lookup"><span data-stu-id="bcc76-250">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="bcc76-251">文件列表列表</span><span class="sxs-lookup"><span data-stu-id="bcc76-251">List of file lists</span></span>|<span data-ttu-id="bcc76-252">用于存储文件列表的默认缓存列表。</span><span class="sxs-lookup"><span data-stu-id="bcc76-252">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="bcc76-253">见解文件列表列表</span><span class="sxs-lookup"><span data-stu-id="bcc76-253">List of insight file lists</span></span>|<span data-ttu-id="bcc76-254">提供时 `insightType` 使用。</span><span class="sxs-lookup"><span data-stu-id="bcc76-254">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="bcc76-255">组件 `mgt-file-list` 在提供时 `fileQueries` 还使用 `mgt-file` IndexedDB 中的对象存储来 `fileQueries` 缓存文件。</span><span class="sxs-lookup"><span data-stu-id="bcc76-255">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="bcc76-256">若要详细了解如何配置缓存[，请参阅](../customize-components/cache.md)Caching。</span><span class="sxs-lookup"><span data-stu-id="bcc76-256">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>