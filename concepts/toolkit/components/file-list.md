---
title: Microsoft 服务中的文件列表Graph Toolkit
description: 文件列表组件用于通过显示文件图标和名称来显示文件列表
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 89f60020fb1db75ed4e79a7402b0aa0518146130
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082172"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9bc03-103">Microsoft 服务中的文件列表Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="9bc03-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9bc03-104">文件列表 [组件使用您](/graph/api/resources/onedrive) 指定的文件/文件夹名称、图标和其他属性显示多个文件夹和文件的列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="9bc03-105">此组件使用 [mgt 文件](./file.md) 组件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="9bc03-106">您可以指定特定驱动器或网站、根据见解类型显示文件列表 (趋势、使用或共享) ，或者提供对自定义文件列表的查询。</span><span class="sxs-lookup"><span data-stu-id="9bc03-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="9bc03-107">示例</span><span class="sxs-lookup"><span data-stu-id="9bc03-107">Example</span></span>

<span data-ttu-id="9bc03-108">以下示例使用 组件显示 `mgt-file-list` 文件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="9bc03-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="9bc03-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="9bc03-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="9bc03-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="9bc03-111">属性</span><span class="sxs-lookup"><span data-stu-id="9bc03-111">Properties</span></span>

<span data-ttu-id="9bc03-112">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="9bc03-113">属性</span><span class="sxs-lookup"><span data-stu-id="9bc03-113">Attribute</span></span> | <span data-ttu-id="9bc03-114">属性</span><span class="sxs-lookup"><span data-stu-id="9bc03-114">Property</span></span> | <span data-ttu-id="9bc03-115">说明</span><span class="sxs-lookup"><span data-stu-id="9bc03-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="9bc03-116">file-list-query</span><span class="sxs-lookup"><span data-stu-id="9bc03-116">file-list-query</span></span> | <span data-ttu-id="9bc03-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="9bc03-117">fileListQuery</span></span> | <span data-ttu-id="9bc03-118">包含要呈现的文件列表的驱动器或站点的完整查询或路径。</span><span class="sxs-lookup"><span data-stu-id="9bc03-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="9bc03-119">文件查询</span><span class="sxs-lookup"><span data-stu-id="9bc03-119">file-queries</span></span> | <span data-ttu-id="9bc03-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="9bc03-120">fileQueries</span></span> | <span data-ttu-id="9bc03-121">由组件呈现的文件查询数组。</span><span class="sxs-lookup"><span data-stu-id="9bc03-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="9bc03-122">无</span><span class="sxs-lookup"><span data-stu-id="9bc03-122">none</span></span> | <span data-ttu-id="9bc03-123">files</span><span class="sxs-lookup"><span data-stu-id="9bc03-123">files</span></span> | <span data-ttu-id="9bc03-124">用于获取或设置组件呈现的文件列表的文件数组。</span><span class="sxs-lookup"><span data-stu-id="9bc03-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="9bc03-125">使用它来访问组件加载的文件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="9bc03-126">设置此值以加载您自己的文件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="9bc03-127">insight-type</span><span class="sxs-lookup"><span data-stu-id="9bc03-127">insight-type</span></span> | <span data-ttu-id="9bc03-128">insightType</span><span class="sxs-lookup"><span data-stu-id="9bc03-128">insightType</span></span> | <span data-ttu-id="9bc03-129">设置为显示用户的趋势、使用的文件或共享文件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="9bc03-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="9bc03-130">drive-id</span></span> | <span data-ttu-id="9bc03-131">driveId</span><span class="sxs-lookup"><span data-stu-id="9bc03-131">driveId</span></span> | <span data-ttu-id="9bc03-132">文件夹所属驱动器的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bc03-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="9bc03-133">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="9bc03-134">group-id</span><span class="sxs-lookup"><span data-stu-id="9bc03-134">group-id</span></span> | <span data-ttu-id="9bc03-135">groupId</span><span class="sxs-lookup"><span data-stu-id="9bc03-135">groupId</span></span> | <span data-ttu-id="9bc03-136">文件夹所属组的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bc03-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="9bc03-137">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="9bc03-138">site-id</span><span class="sxs-lookup"><span data-stu-id="9bc03-138">site-id</span></span> | <span data-ttu-id="9bc03-139">siteId</span><span class="sxs-lookup"><span data-stu-id="9bc03-139">siteId</span></span> | <span data-ttu-id="9bc03-140">文件夹所属网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bc03-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="9bc03-141">还必须提供 或 `{item-id}` `{item-path}` 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="9bc03-142">`{list-id}`如果从特定列表引用文件，则提供 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="9bc03-143">item-id</span><span class="sxs-lookup"><span data-stu-id="9bc03-143">item-id</span></span> | <span data-ttu-id="9bc03-144">itemId</span><span class="sxs-lookup"><span data-stu-id="9bc03-144">itemId</span></span> | <span data-ttu-id="9bc03-145">文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bc03-145">ID of the folder.</span></span> <span data-ttu-id="9bc03-146">默认查询为 `/me/drive/items` 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="9bc03-147">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="9bc03-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="9bc03-148">item-path</span><span class="sxs-lookup"><span data-stu-id="9bc03-148">item-path</span></span> | <span data-ttu-id="9bc03-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="9bc03-149">itemPath</span></span> | <span data-ttu-id="9bc03-150">文件夹的项目路径 (根文件夹) 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="9bc03-151">默认查询为 `/me/drive/root` 。</span><span class="sxs-lookup"><span data-stu-id="9bc03-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="9bc03-152">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="9bc03-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="9bc03-153">页面大小</span><span class="sxs-lookup"><span data-stu-id="9bc03-153">page-size</span></span> | <span data-ttu-id="9bc03-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="9bc03-154">pageSize</span></span> | <span data-ttu-id="9bc03-155">一个数字值，指示每个页面上要呈现的最大文件数。</span><span class="sxs-lookup"><span data-stu-id="9bc03-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="9bc03-156">文件扩展名</span><span class="sxs-lookup"><span data-stu-id="9bc03-156">file-extensions</span></span> | <span data-ttu-id="9bc03-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="9bc03-157">fileExtensions</span></span> | <span data-ttu-id="9bc03-158">用于筛选要显示的文件的文件扩展名数组。</span><span class="sxs-lookup"><span data-stu-id="9bc03-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="9bc03-159">hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="9bc03-159">hide-more-files-button</span></span> | <span data-ttu-id="9bc03-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="9bc03-160">hideMoreFilesButton</span></span> | <span data-ttu-id="9bc03-161">用于指示是否显示按钮以呈现更多文件的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9bc03-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="9bc03-162">下面的示例更改组件的行为，以从特定查询获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="9bc03-163">以下示例通过提供文件夹 ID，更改组件的行为，以从文件夹获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="9bc03-164">以下示例通过提供组 ID 和文件夹路径，更改组件的行为以从组提取文件列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="9bc03-165">以下示例通过提供用户 ID 和文件夹 ID，更改组件的行为以从用户获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="9bc03-166">以下示例通过提供见解类型，更改组件的行为以提取文件列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="methods"></a><span data-ttu-id="9bc03-167">方法</span><span class="sxs-lookup"><span data-stu-id="9bc03-167">Methods</span></span>
| <span data-ttu-id="9bc03-168">方法</span><span class="sxs-lookup"><span data-stu-id="9bc03-168">Method</span></span> | <span data-ttu-id="9bc03-169">说明</span><span class="sxs-lookup"><span data-stu-id="9bc03-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="9bc03-170">reload (clearCache = false) </span><span class="sxs-lookup"><span data-stu-id="9bc03-170">reload(clearCache = false)</span></span> | <span data-ttu-id="9bc03-171">调用 方法，根据组件的属性使用潜在的新数据重新加载组件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-171">Call the method to reload the component with potential new data based on its properties.</span></span> <span data-ttu-id="9bc03-172">传递 `true` 以在重新加载之前清除缓存。</span><span class="sxs-lookup"><span data-stu-id="9bc03-172">Pass `true` to clear the cache before reloading.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="9bc03-173">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="9bc03-173">CSS custom properties</span></span>

<span data-ttu-id="9bc03-174">组件 `mgt-file-list` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="9bc03-174">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="9bc03-175">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="9bc03-175">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="9bc03-176">Microsoft Graph API 和权限</span><span class="sxs-lookup"><span data-stu-id="9bc03-176">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="9bc03-177">配置</span><span class="sxs-lookup"><span data-stu-id="9bc03-177">Configuration</span></span> | <span data-ttu-id="9bc03-178">权限</span><span class="sxs-lookup"><span data-stu-id="9bc03-178">Permissions</span></span> | <span data-ttu-id="9bc03-179">API</span><span class="sxs-lookup"><span data-stu-id="9bc03-179">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="9bc03-180">默认 (未提供标识符或) </span><span class="sxs-lookup"><span data-stu-id="9bc03-180">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="9bc03-181">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children` |
| <span data-ttu-id="9bc03-182">提供 `{drive-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-182">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="9bc03-183">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="9bc03-184">提供 `{group-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-184">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="9bc03-185">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="9bc03-186">仅提供 `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-186">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="9bc03-187">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` |
| <span data-ttu-id="9bc03-188">提供 `{site-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-188">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="9bc03-189">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="9bc03-190">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-190">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="9bc03-191">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="9bc03-192">提供 `{drive-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-192">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="9bc03-193">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="9bc03-194">提供 `{group-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-194">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="9bc03-195">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="9bc03-196">提供 `{site-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-196">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="9bc03-197">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-197">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="9bc03-198">提供 `{user-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-198">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="9bc03-199">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-199">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="9bc03-200">仅提供 `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="9bc03-200">Provide only `{item-path}`</span></span> | <span data-ttu-id="9bc03-201">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-201">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="9bc03-202">`insight-type` 设置为趋势</span><span class="sxs-lookup"><span data-stu-id="9bc03-202">`insight-type` is set to trending</span></span> | <span data-ttu-id="9bc03-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-203">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="9bc03-204">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `trending`</span><span class="sxs-lookup"><span data-stu-id="9bc03-204">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="9bc03-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-205">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` |
| <span data-ttu-id="9bc03-206">`insight-type` 设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="9bc03-206">`insight-type` is set to `used`</span></span> | <span data-ttu-id="9bc03-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-207">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="9bc03-208">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="9bc03-208">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="9bc03-209">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-209">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="9bc03-210">`insight-type` 设置为共享</span><span class="sxs-lookup"><span data-stu-id="9bc03-210">`insight-type` is set to shared</span></span> | <span data-ttu-id="9bc03-211">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-211">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="9bc03-212">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `shared`</span><span class="sxs-lookup"><span data-stu-id="9bc03-212">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="9bc03-213">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc03-213">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="9bc03-214">活动</span><span class="sxs-lookup"><span data-stu-id="9bc03-214">Events</span></span>

| <span data-ttu-id="9bc03-215">事件</span><span class="sxs-lookup"><span data-stu-id="9bc03-215">Event</span></span> | <span data-ttu-id="9bc03-216">说明</span><span class="sxs-lookup"><span data-stu-id="9bc03-216">Description</span></span> |
| ----- | ----------- |
| `itemClick` | <span data-ttu-id="9bc03-217">在用户单击文件时触发。</span><span class="sxs-lookup"><span data-stu-id="9bc03-217">Fired when the user clicks a file.</span></span> <span data-ttu-id="9bc03-218">返回文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="9bc03-218">Returns the file details.</span></span> |

<span data-ttu-id="9bc03-219">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="9bc03-219">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="9bc03-220">模板</span><span class="sxs-lookup"><span data-stu-id="9bc03-220">Templates</span></span>

<span data-ttu-id="9bc03-221">组件 `mgt-file-list` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="9bc03-221">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="9bc03-222">若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的数据类型之一。</span><span class="sxs-lookup"><span data-stu-id="9bc03-222">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="9bc03-223">数据类型</span><span class="sxs-lookup"><span data-stu-id="9bc03-223">Data type</span></span> | <span data-ttu-id="9bc03-224">数据上下文</span><span class="sxs-lookup"><span data-stu-id="9bc03-224">Data context</span></span> | <span data-ttu-id="9bc03-225">说明</span><span class="sxs-lookup"><span data-stu-id="9bc03-225">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="9bc03-226">default</span><span class="sxs-lookup"><span data-stu-id="9bc03-226">default</span></span> | <span data-ttu-id="9bc03-227">`files`：文件对象列表</span><span class="sxs-lookup"><span data-stu-id="9bc03-227">`files`: list of file objects</span></span> | <span data-ttu-id="9bc03-228">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-228">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="9bc03-229">file</span><span class="sxs-lookup"><span data-stu-id="9bc03-229">file</span></span> | <span data-ttu-id="9bc03-230">`file`：file 对象</span><span class="sxs-lookup"><span data-stu-id="9bc03-230">`file`: file object</span></span> | <span data-ttu-id="9bc03-231">用于呈现每个文件的模板。</span><span class="sxs-lookup"><span data-stu-id="9bc03-231">The template used to render each file.</span></span> |
| <span data-ttu-id="9bc03-232">no-data</span><span class="sxs-lookup"><span data-stu-id="9bc03-232">no-data</span></span> | <span data-ttu-id="9bc03-233">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="9bc03-233">No data context is passed</span></span> | <span data-ttu-id="9bc03-234">没有可用数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="9bc03-234">The template used when no data is available.</span></span> |
| <span data-ttu-id="9bc03-235">loading</span><span class="sxs-lookup"><span data-stu-id="9bc03-235">loading</span></span> | <span data-ttu-id="9bc03-236">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="9bc03-236">No data context is passed</span></span> | <span data-ttu-id="9bc03-237">组件加载状态时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="9bc03-237">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="9bc03-238">身份验证</span><span class="sxs-lookup"><span data-stu-id="9bc03-238">Authentication</span></span>

<span data-ttu-id="9bc03-239">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="9bc03-239">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="9bc03-240">缓存</span><span class="sxs-lookup"><span data-stu-id="9bc03-240">Cache</span></span>

|<span data-ttu-id="9bc03-241">对象存储</span><span class="sxs-lookup"><span data-stu-id="9bc03-241">Object store</span></span>|<span data-ttu-id="9bc03-242">缓存数据</span><span class="sxs-lookup"><span data-stu-id="9bc03-242">Cached data</span></span>|<span data-ttu-id="9bc03-243">备注</span><span class="sxs-lookup"><span data-stu-id="9bc03-243">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="9bc03-244">文件列表列表</span><span class="sxs-lookup"><span data-stu-id="9bc03-244">List of file lists</span></span>|<span data-ttu-id="9bc03-245">用于存储文件列表的默认缓存列表。</span><span class="sxs-lookup"><span data-stu-id="9bc03-245">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="9bc03-246">见解文件列表列表</span><span class="sxs-lookup"><span data-stu-id="9bc03-246">List of insight file lists</span></span>|<span data-ttu-id="9bc03-247">提供时 `insightType` 使用。</span><span class="sxs-lookup"><span data-stu-id="9bc03-247">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="9bc03-248">组件 `mgt-file-list` 在提供时 `fileQueries` 还使用 `mgt-file` IndexedDB 中的对象存储来 `fileQueries` 缓存文件。</span><span class="sxs-lookup"><span data-stu-id="9bc03-248">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="9bc03-249">若要详细了解如何配置缓存[，请参阅](../customize-components/cache.md)Caching。</span><span class="sxs-lookup"><span data-stu-id="9bc03-249">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>