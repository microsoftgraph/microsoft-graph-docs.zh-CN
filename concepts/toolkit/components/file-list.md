---
title: Microsoft 服务中的文件列表Graph Toolkit
description: 文件列表组件用于通过显示文件图标和名称来显示文件列表
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 77eb93bc17d9c684ac61fc6a7dc2f263e406bba8
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579805"
---
# <a name="file-list-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f7775-103">Microsoft 服务中的文件列表Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f7775-103">File list component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f7775-104">文件列表 [组件使用您](/graph/api/resources/onedrive) 指定的文件/文件夹名称、图标和其他属性显示多个文件夹和文件的列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-104">The File List component displays [a list of multiple folders and files](/graph/api/resources/onedrive) by using the file/folder name, an icon, and other properties that you specify.</span></span> <span data-ttu-id="f7775-105">此组件使用 [mgt 文件](./file.md) 组件。</span><span class="sxs-lookup"><span data-stu-id="f7775-105">This component uses the [mgt-file](./file.md) component.</span></span> <span data-ttu-id="f7775-106">您可以指定特定驱动器或网站、根据见解类型显示文件列表 (趋势、使用或共享) ，或者提供对自定义文件列表的查询。</span><span class="sxs-lookup"><span data-stu-id="f7775-106">You can specify a specific drive or site, display a list of files based on insight type (trending, used, or shared), or provide queries to a custom list of files.</span></span>

## <a name="example"></a><span data-ttu-id="f7775-107">示例</span><span class="sxs-lookup"><span data-stu-id="f7775-107">Example</span></span>

<span data-ttu-id="f7775-108">以下示例使用 组件显示 `mgt-file-list` 文件。</span><span class="sxs-lookup"><span data-stu-id="f7775-108">The following example displays a file using the `mgt-file-list` component.</span></span> <span data-ttu-id="f7775-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="f7775-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file-list--file-list&source=docs" height="250"></iframe>

[<span data-ttu-id="f7775-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="f7775-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file-list--file-list&source=docs)

## <a name="properties"></a><span data-ttu-id="f7775-111">属性</span><span class="sxs-lookup"><span data-stu-id="f7775-111">Properties</span></span>

<span data-ttu-id="f7775-112">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="f7775-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="f7775-113">属性</span><span class="sxs-lookup"><span data-stu-id="f7775-113">Attribute</span></span> | <span data-ttu-id="f7775-114">属性</span><span class="sxs-lookup"><span data-stu-id="f7775-114">Property</span></span> | <span data-ttu-id="f7775-115">说明</span><span class="sxs-lookup"><span data-stu-id="f7775-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="f7775-116">file-list-query</span><span class="sxs-lookup"><span data-stu-id="f7775-116">file-list-query</span></span> | <span data-ttu-id="f7775-117">fileListQuery</span><span class="sxs-lookup"><span data-stu-id="f7775-117">fileListQuery</span></span> | <span data-ttu-id="f7775-118">包含要呈现的文件列表的驱动器或站点的完整查询或路径。</span><span class="sxs-lookup"><span data-stu-id="f7775-118">The full query or path to the drive or site that contains the list of files to render.</span></span> |
| <span data-ttu-id="f7775-119">文件查询</span><span class="sxs-lookup"><span data-stu-id="f7775-119">file-queries</span></span> | <span data-ttu-id="f7775-120">fileQueries</span><span class="sxs-lookup"><span data-stu-id="f7775-120">fileQueries</span></span> | <span data-ttu-id="f7775-121">由组件呈现的文件查询数组。</span><span class="sxs-lookup"><span data-stu-id="f7775-121">An array of file queries to be rendered by the component.</span></span> |
| <span data-ttu-id="f7775-122">无</span><span class="sxs-lookup"><span data-stu-id="f7775-122">none</span></span> | <span data-ttu-id="f7775-123">files</span><span class="sxs-lookup"><span data-stu-id="f7775-123">files</span></span> | <span data-ttu-id="f7775-124">用于获取或设置组件呈现的文件列表的文件数组。</span><span class="sxs-lookup"><span data-stu-id="f7775-124">An array of files to get or set the list of files rendered by the component.</span></span> <span data-ttu-id="f7775-125">使用它来访问组件加载的文件。</span><span class="sxs-lookup"><span data-stu-id="f7775-125">Use this to access the files loaded by the component.</span></span> <span data-ttu-id="f7775-126">设置此值以加载您自己的文件。</span><span class="sxs-lookup"><span data-stu-id="f7775-126">Set this value to load your own files.</span></span> |
| <span data-ttu-id="f7775-127">insight-type</span><span class="sxs-lookup"><span data-stu-id="f7775-127">insight-type</span></span> | <span data-ttu-id="f7775-128">insightType</span><span class="sxs-lookup"><span data-stu-id="f7775-128">insightType</span></span> | <span data-ttu-id="f7775-129">设置为显示用户的趋势、使用的文件或共享文件。</span><span class="sxs-lookup"><span data-stu-id="f7775-129">Set to show the user’s trending, used, or shared files.</span></span> |
| <span data-ttu-id="f7775-130">drive-id</span><span class="sxs-lookup"><span data-stu-id="f7775-130">drive-id</span></span> | <span data-ttu-id="f7775-131">driveId</span><span class="sxs-lookup"><span data-stu-id="f7775-131">driveId</span></span> | <span data-ttu-id="f7775-132">文件夹所属驱动器的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7775-132">ID of the drive the folder belongs to.</span></span> <span data-ttu-id="f7775-133">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="f7775-133">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="f7775-134">group-id</span><span class="sxs-lookup"><span data-stu-id="f7775-134">group-id</span></span> | <span data-ttu-id="f7775-135">groupId</span><span class="sxs-lookup"><span data-stu-id="f7775-135">groupId</span></span> | <span data-ttu-id="f7775-136">文件夹所属组的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7775-136">ID of the group the folder belongs to.</span></span> <span data-ttu-id="f7775-137">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="f7775-137">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="f7775-138">site-id</span><span class="sxs-lookup"><span data-stu-id="f7775-138">site-id</span></span> | <span data-ttu-id="f7775-139">siteId</span><span class="sxs-lookup"><span data-stu-id="f7775-139">siteId</span></span> | <span data-ttu-id="f7775-140">文件夹所属网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7775-140">ID of the site the folder belongs to.</span></span> <span data-ttu-id="f7775-141">还必须提供 或 `{item-id}` `{item-path}` 。</span><span class="sxs-lookup"><span data-stu-id="f7775-141">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="f7775-142">`{list-id}`如果从特定列表引用文件，则提供 。</span><span class="sxs-lookup"><span data-stu-id="f7775-142">Provide `{list-id}` if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="f7775-143">item-id</span><span class="sxs-lookup"><span data-stu-id="f7775-143">item-id</span></span> | <span data-ttu-id="f7775-144">itemId</span><span class="sxs-lookup"><span data-stu-id="f7775-144">itemId</span></span> | <span data-ttu-id="f7775-145">文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7775-145">ID of the folder.</span></span> <span data-ttu-id="f7775-146">默认查询为 `/me/drive/items` 。</span><span class="sxs-lookup"><span data-stu-id="f7775-146">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="f7775-147">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="f7775-147">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="f7775-148">item-path</span><span class="sxs-lookup"><span data-stu-id="f7775-148">item-path</span></span> | <span data-ttu-id="f7775-149">itemPath</span><span class="sxs-lookup"><span data-stu-id="f7775-149">itemPath</span></span> | <span data-ttu-id="f7775-150">文件夹的项目路径 (根文件夹) 。</span><span class="sxs-lookup"><span data-stu-id="f7775-150">Item path of the folder (relative to the root).</span></span> <span data-ttu-id="f7775-151">默认查询为 `/me/drive/root` 。</span><span class="sxs-lookup"><span data-stu-id="f7775-151">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="f7775-152">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="f7775-152">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="f7775-153">页面大小</span><span class="sxs-lookup"><span data-stu-id="f7775-153">page-size</span></span> | <span data-ttu-id="f7775-154">pageSize</span><span class="sxs-lookup"><span data-stu-id="f7775-154">pageSize</span></span> | <span data-ttu-id="f7775-155">一个数字值，指示每个页面上要呈现的最大文件数。</span><span class="sxs-lookup"><span data-stu-id="f7775-155">A number value to indicate the maximum number of files to render on each page.</span></span> |
| <span data-ttu-id="f7775-156">文件扩展名</span><span class="sxs-lookup"><span data-stu-id="f7775-156">file-extensions</span></span> | <span data-ttu-id="f7775-157">fileExtensions</span><span class="sxs-lookup"><span data-stu-id="f7775-157">fileExtensions</span></span> | <span data-ttu-id="f7775-158">用于筛选要显示的文件的文件扩展名数组。</span><span class="sxs-lookup"><span data-stu-id="f7775-158">An array of file extensions used to filter files to show.</span></span> |
| <span data-ttu-id="f7775-159">hide-more-files-button</span><span class="sxs-lookup"><span data-stu-id="f7775-159">hide-more-files-button</span></span> | <span data-ttu-id="f7775-160">hideMoreFilesButton</span><span class="sxs-lookup"><span data-stu-id="f7775-160">hideMoreFilesButton</span></span> | <span data-ttu-id="f7775-161">用于指示是否显示按钮以呈现更多文件的布尔值。</span><span class="sxs-lookup"><span data-stu-id="f7775-161">A boolean to indicate whether to show a button to render more files.</span></span> |

<span data-ttu-id="f7775-162">下面的示例更改组件的行为，以从特定查询获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-162">The following example changes the behavior of the component to fetch a file list from a specific query.</span></span>

```html
<mgt-file-list file-list-query="/me/drive/items/01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY/children"></mgt-file-list>
```

<span data-ttu-id="f7775-163">以下示例通过提供文件夹 ID，更改组件的行为，以从文件夹获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-163">The following example changes the behavior of the component to fetch a file list from a folder by providing the folder id.</span></span>

```html
<mgt-file-list item-id="01BYE5RZYJ43UXGBP23BBIFPISHHMCDTOY"></mgt-file-list>
```

<span data-ttu-id="f7775-164">以下示例通过提供组 ID 和文件夹路径，更改组件的行为以从组提取文件列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-164">The following example changes the behavior of the component to fetch file list from a group by providing the group id and folder path.</span></span>

```html
<mgt-file-list group-id="8090c93e-ba7c-433e-9f39-08c7ba07c0b3" item-path="/Design"></mgt-file-list>
```

<span data-ttu-id="f7775-165">以下示例通过提供用户 ID 和文件夹 ID，更改组件的行为以从用户获取文件列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-165">The following example changes the behavior of the component to fetch file list from a user by providing the user id and folder id.</span></span>

```html
<mgt-file-list user-id="48d31887-5fad-4d73-a9f5-3c356e68a038" item-id="01BYE5RZYFPM65IDVARFELFLNTXR4ZKABD"></mgt-file-list>
```

<span data-ttu-id="f7775-166">以下示例通过提供见解类型，更改组件的行为以提取文件列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-166">The following example changes the behavior of the component to fetch file list by providing the insight type.</span></span>

```html
<mgt-file-list insight-type="shared"></mgt-file-list>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f7775-167">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="f7775-167">CSS custom properties</span></span>

<span data-ttu-id="f7775-168">组件 `mgt-file-list` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="f7775-168">The `mgt-file-list` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="f7775-169">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="f7775-169">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="f7775-170">Microsoft Graph API 和权限</span><span class="sxs-lookup"><span data-stu-id="f7775-170">Microsoft Graph APIs and permissions</span></span>

| <span data-ttu-id="f7775-171">配置</span><span class="sxs-lookup"><span data-stu-id="f7775-171">Configuration</span></span> | <span data-ttu-id="f7775-172">权限</span><span class="sxs-lookup"><span data-stu-id="f7775-172">Permissions</span></span> | <span data-ttu-id="f7775-173">API</span><span class="sxs-lookup"><span data-stu-id="f7775-173">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="f7775-174">默认 (未提供标识符或) </span><span class="sxs-lookup"><span data-stu-id="f7775-174">Default (no identifiers or query provided)</span></span> | <span data-ttu-id="f7775-175">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-175">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root/children`   |
| <span data-ttu-id="f7775-176">提供 `{drive-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="f7775-176">Provide `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="f7775-177">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-177">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}/children` |
| <span data-ttu-id="f7775-178">提供 `{group-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="f7775-178">Provide `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="f7775-179">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-179">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="f7775-180">仅提供 `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="f7775-180">Provide ONLY `{item-id}`</span></span> | <span data-ttu-id="f7775-181">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-181">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}/children` | 
| <span data-ttu-id="f7775-182">提供 `{site-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="f7775-182">Provide `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="f7775-183">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-183">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="f7775-184">Pprovide `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="f7775-184">Pprovide `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="f7775-185">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-185">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}/children` |
| <span data-ttu-id="f7775-186">提供 `{drive-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="f7775-186">Provide `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="f7775-187">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-187">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}:/children` |
| <span data-ttu-id="f7775-188">提供 `{group-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="f7775-188">Provide `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="f7775-189">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-189">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/root:/{item-path}:/children` |
| <span data-ttu-id="f7775-190">提供 `{site-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="f7775-190">Provide `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="f7775-191">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-191">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/root:/{item-path}:/children` |
| <span data-ttu-id="f7775-192">提供 `{user-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="f7775-192">Provide `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="f7775-193">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/root:/{item-path}:/children` |
| <span data-ttu-id="f7775-194">仅提供 `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="f7775-194">Provide only `{item-path}`</span></span> | <span data-ttu-id="f7775-195">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}:/children` |
| <span data-ttu-id="f7775-196">`insight-type` 设置为趋势</span><span class="sxs-lookup"><span data-stu-id="f7775-196">`insight-type` is set to trending</span></span> | <span data-ttu-id="f7775-197">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-197">Sites.Read.All</span></span> | `GET /me/insights/trending` |
| <span data-ttu-id="f7775-198">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `trending`</span><span class="sxs-lookup"><span data-stu-id="f7775-198">Provide `{user-id or upn}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="f7775-199">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-199">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending` | 
| <span data-ttu-id="f7775-200">`insight-type` 设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="f7775-200">`insight-type` is set to `used`</span></span> | <span data-ttu-id="f7775-201">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-201">Sites.Read.All</span></span> | `GET /me/insights/used` |
| <span data-ttu-id="f7775-202">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="f7775-202">Provide `{user-id or upn}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="f7775-203">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-203">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used` |
| <span data-ttu-id="f7775-204">`insight-type` 设置为共享</span><span class="sxs-lookup"><span data-stu-id="f7775-204">`insight-type` is set to shared</span></span> | <span data-ttu-id="f7775-205">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-205">Sites.Read.All</span></span> | `GET /me/insights/shared` |
| <span data-ttu-id="f7775-206">" `{user-id or upn}` `insight-type` 提供 AND"设置为 `shared`</span><span class="sxs-lookup"><span data-stu-id="f7775-206">Provide `{user-id or upn}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="f7775-207">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7775-207">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared?$filter=((lastshared/sharedby/id eq '${user-id}') and (resourceReference/type eq 'microsoft.graph.driveItem'))` |

## <a name="events"></a><span data-ttu-id="f7775-208">活动</span><span class="sxs-lookup"><span data-stu-id="f7775-208">Events</span></span>

| <span data-ttu-id="f7775-209">事件</span><span class="sxs-lookup"><span data-stu-id="f7775-209">Event</span></span> | <span data-ttu-id="f7775-210">说明</span><span class="sxs-lookup"><span data-stu-id="f7775-210">Description</span></span> |
| ----- | ----------- |
| <span data-ttu-id="f7775-211">itemClick</span><span class="sxs-lookup"><span data-stu-id="f7775-211">itemClick</span></span> | <span data-ttu-id="f7775-212">在用户单击文件时触发。</span><span class="sxs-lookup"><span data-stu-id="f7775-212">Fired when the user clicks a file.</span></span> <span data-ttu-id="f7775-213">返回文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="f7775-213">Returns the file details.</span></span> |

## <a name="templates"></a><span data-ttu-id="f7775-214">模板</span><span class="sxs-lookup"><span data-stu-id="f7775-214">Templates</span></span>

<span data-ttu-id="f7775-215">组件 `mgt-file-list` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="f7775-215">The `mgt-file-list` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="f7775-216">若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的数据类型之一。</span><span class="sxs-lookup"><span data-stu-id="f7775-216">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the data types listed in the following table.</span></span>

| <span data-ttu-id="f7775-217">数据类型</span><span class="sxs-lookup"><span data-stu-id="f7775-217">Data type</span></span> | <span data-ttu-id="f7775-218">数据上下文</span><span class="sxs-lookup"><span data-stu-id="f7775-218">Data context</span></span> | <span data-ttu-id="f7775-219">说明</span><span class="sxs-lookup"><span data-stu-id="f7775-219">Description</span></span> |
| ----------- | -------------- | ------------ |
| <span data-ttu-id="f7775-220">default</span><span class="sxs-lookup"><span data-stu-id="f7775-220">default</span></span> | <span data-ttu-id="f7775-221">`files`：文件对象列表</span><span class="sxs-lookup"><span data-stu-id="f7775-221">`files`: list of file objects</span></span> | <span data-ttu-id="f7775-222">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="f7775-222">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="f7775-223">file</span><span class="sxs-lookup"><span data-stu-id="f7775-223">file</span></span> | <span data-ttu-id="f7775-224">`file`：file 对象</span><span class="sxs-lookup"><span data-stu-id="f7775-224">`file`: file object</span></span> | <span data-ttu-id="f7775-225">用于呈现每个文件的模板。</span><span class="sxs-lookup"><span data-stu-id="f7775-225">The template used to render each file.</span></span> |
| <span data-ttu-id="f7775-226">no-data</span><span class="sxs-lookup"><span data-stu-id="f7775-226">no-data</span></span> | <span data-ttu-id="f7775-227">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="f7775-227">No data context is passed</span></span> | <span data-ttu-id="f7775-228">没有可用数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f7775-228">The template used when no data is available.</span></span> |
| <span data-ttu-id="f7775-229">loading</span><span class="sxs-lookup"><span data-stu-id="f7775-229">loading</span></span> | <span data-ttu-id="f7775-230">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="f7775-230">No data context is passed</span></span> | <span data-ttu-id="f7775-231">组件加载状态时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f7775-231">The template used while the component loads state.</span></span> |

## <a name="authentication"></a><span data-ttu-id="f7775-232">身份验证</span><span class="sxs-lookup"><span data-stu-id="f7775-232">Authentication</span></span>

<span data-ttu-id="f7775-233">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="f7775-233">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="f7775-234">缓存</span><span class="sxs-lookup"><span data-stu-id="f7775-234">Cache</span></span>

|<span data-ttu-id="f7775-235">对象存储</span><span class="sxs-lookup"><span data-stu-id="f7775-235">Object store</span></span>|<span data-ttu-id="f7775-236">缓存数据</span><span class="sxs-lookup"><span data-stu-id="f7775-236">Cached data</span></span>|<span data-ttu-id="f7775-237">备注</span><span class="sxs-lookup"><span data-stu-id="f7775-237">Remarks</span></span>|
|---------|-----------|-------|
|`fileLists`|<span data-ttu-id="f7775-238">文件列表列表</span><span class="sxs-lookup"><span data-stu-id="f7775-238">List of file lists</span></span>|<span data-ttu-id="f7775-239">用于存储文件列表的默认缓存列表。</span><span class="sxs-lookup"><span data-stu-id="f7775-239">Default cache list to store file lists.</span></span>|
|`insightfileLists`|<span data-ttu-id="f7775-240">见解文件列表列表</span><span class="sxs-lookup"><span data-stu-id="f7775-240">List of insight file lists</span></span>|<span data-ttu-id="f7775-241">提供时 `insightType` 使用。</span><span class="sxs-lookup"><span data-stu-id="f7775-241">Used when `insightType` is provided.</span></span>|

> [!NOTE]
> <span data-ttu-id="f7775-242">组件 `mgt-file-list` 在提供时 `fileQueries` 还使用 `mgt-file` IndexedDB 中的对象存储来 `fileQueries` 缓存文件。</span><span class="sxs-lookup"><span data-stu-id="f7775-242">The `mgt-file-list` component also uses the `fileQueries` object store in `mgt-file` IndexedDB to cache files when `fileQueries` is provided.</span></span>

<span data-ttu-id="f7775-243">若要详细了解如何配置缓存[，请参阅](../customize-components/cache.md)Caching。</span><span class="sxs-lookup"><span data-stu-id="f7775-243">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>