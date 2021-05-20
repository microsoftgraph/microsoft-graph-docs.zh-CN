---
title: Microsoft 服务中的文件Graph Toolkit
description: 文件组件用于通过显示图标和名称来显示文件
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 314f08d396421c3b0afe0cf049e91cca9daa03fd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579806"
---
# <a name="file-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c6ddc-103">Microsoft 服务中的文件Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="c6ddc-103">File component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c6ddc-104">File 组件用于表示 OneDrive 或 SharePoint 中的单个文件[/](/graph/onedrive-concept-overview)文件夹，具体方法为显示文件/文件夹名称、指示文件类型的图标以及其他属性（如作者、上次修改日期或其他详细信息）。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-104">The File component is used to represent an individual [file/folder from OneDrive or SharePoint](/graph/onedrive-concept-overview) by displaying information such as the file/folder name, an icon indicating the file type, and other properties such as the author, last modified date, or other details.</span></span> <span data-ttu-id="c6ddc-105">你可以提供文件的标识符，组件将生成查询以根据提供的标识符检索文件。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-105">You can provide the identifiers for a file and the component will generate the query to retrieve the file based on the identifiers provided.</span></span> <span data-ttu-id="c6ddc-106">此组件可以自己使用，也可以作为 [mgt-file-list组件的一部分](./file-list.md) 使用。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-106">This component can be used on its own or as part of the [mgt-file-list](./file-list.md) components.</span></span>

## <a name="example"></a><span data-ttu-id="c6ddc-107">示例</span><span class="sxs-lookup"><span data-stu-id="c6ddc-107">Example</span></span>

<span data-ttu-id="c6ddc-108">以下示例使用 组件显示 `mgt-file` 文件。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-108">The following example displays a file using the `mgt-file` component.</span></span> <span data-ttu-id="c6ddc-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-file--file&source=docs" height="250"></iframe>

[<span data-ttu-id="c6ddc-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="c6ddc-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-file--file&source=docs)

## <a name="properties"></a><span data-ttu-id="c6ddc-111">属性</span><span class="sxs-lookup"><span data-stu-id="c6ddc-111">Properties</span></span>

<span data-ttu-id="c6ddc-112">可以使用多个属性来自定义组件。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-112">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="c6ddc-113">属性</span><span class="sxs-lookup"><span data-stu-id="c6ddc-113">Attribute</span></span> | <span data-ttu-id="c6ddc-114">属性</span><span class="sxs-lookup"><span data-stu-id="c6ddc-114">Property</span></span> | <span data-ttu-id="c6ddc-115">说明</span><span class="sxs-lookup"><span data-stu-id="c6ddc-115">Description</span></span> |
| --------- | -------- | ----------- |
| <span data-ttu-id="c6ddc-116">文件查询</span><span class="sxs-lookup"><span data-stu-id="c6ddc-116">file-query</span></span> | <span data-ttu-id="c6ddc-117">fileQuery</span><span class="sxs-lookup"><span data-stu-id="c6ddc-117">fileQuery</span></span> | <span data-ttu-id="c6ddc-118">要检索的文件的完整查询或路径。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-118">The full query or path to the file to be retrieved.</span></span> |
| <span data-ttu-id="c6ddc-119">drive-id</span><span class="sxs-lookup"><span data-stu-id="c6ddc-119">drive-id</span></span> | <span data-ttu-id="c6ddc-120">driveId</span><span class="sxs-lookup"><span data-stu-id="c6ddc-120">driveId</span></span> | <span data-ttu-id="c6ddc-121">文件所属驱动器的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-121">The ID of the drive the file belongs to.</span></span> <span data-ttu-id="c6ddc-122">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-122">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="c6ddc-123">group-id</span><span class="sxs-lookup"><span data-stu-id="c6ddc-123">group-id</span></span> | <span data-ttu-id="c6ddc-124">groupId</span><span class="sxs-lookup"><span data-stu-id="c6ddc-124">groupId</span></span> | <span data-ttu-id="c6ddc-125">文件所属组的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-125">ID of the group the file belongs to.</span></span> <span data-ttu-id="c6ddc-126">还必须提供 或 `item-id` `item-path` 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-126">Must also provide either `item-id` or `item-path`.</span></span> |
| <span data-ttu-id="c6ddc-127">site-id</span><span class="sxs-lookup"><span data-stu-id="c6ddc-127">site-id</span></span> | <span data-ttu-id="c6ddc-128">siteId</span><span class="sxs-lookup"><span data-stu-id="c6ddc-128">siteId</span></span> | <span data-ttu-id="c6ddc-129">文件所属网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-129">ID of the site the file belongs to.</span></span> <span data-ttu-id="c6ddc-130">还必须提供 或 `{item-id}` `{item-path}` 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-130">Must also provide either `{item-id}` or `{item-path}`.</span></span> <span data-ttu-id="c6ddc-131">如果 `{list-id}` 从特定列表引用文件，则也提供 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-131">Provide the `{list-id}` too if you’re referencing a file from a specific list.</span></span> |
| <span data-ttu-id="c6ddc-132">list-id</span><span class="sxs-lookup"><span data-stu-id="c6ddc-132">list-id</span></span> | <span data-ttu-id="c6ddc-133">listId</span><span class="sxs-lookup"><span data-stu-id="c6ddc-133">listId</span></span> | <span data-ttu-id="c6ddc-134">文件所属列表的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-134">ID of the list the file belongs to.</span></span> <span data-ttu-id="c6ddc-135">还必须提供 `{site-id}` `{item-id}` 和 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-135">Must also provide `{site-id}` and `{item-id}`.</span></span> |
| <span data-ttu-id="c6ddc-136">item-id</span><span class="sxs-lookup"><span data-stu-id="c6ddc-136">item-id</span></span> | <span data-ttu-id="c6ddc-137">itemId</span><span class="sxs-lookup"><span data-stu-id="c6ddc-137">itemId</span></span> | <span data-ttu-id="c6ddc-138">文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-138">ID of the file.</span></span> <span data-ttu-id="c6ddc-139">默认查询为 `/me/drive/items` 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-139">Default query is `/me/drive/items`.</span></span> <span data-ttu-id="c6ddc-140">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-140">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="c6ddc-141">item-path</span><span class="sxs-lookup"><span data-stu-id="c6ddc-141">item-path</span></span> | <span data-ttu-id="c6ddc-142">itemPath</span><span class="sxs-lookup"><span data-stu-id="c6ddc-142">itemPath</span></span> | <span data-ttu-id="c6ddc-143">文件的项目路径。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-143">Item path of the file.</span></span> <span data-ttu-id="c6ddc-144">默认查询为 `/me/drive/root` 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-144">Default query is `/me/drive/root`.</span></span> <span data-ttu-id="c6ddc-145">提供 `{drive-id}` `{group-id}` 、 、 或 `{site-id}` `{user-id}` 以查询特定位置。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-145">Provide `{drive-id}`, `{group-id}`, `{site-id}`, or `{user-id}` to query a specific location.</span></span> |
| <span data-ttu-id="c6ddc-146">insight-type</span><span class="sxs-lookup"><span data-stu-id="c6ddc-146">insight-type</span></span> | <span data-ttu-id="c6ddc-147">insightType</span><span class="sxs-lookup"><span data-stu-id="c6ddc-147">insightType</span></span> | <span data-ttu-id="c6ddc-148">从中检索文件的见解类型。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-148">Type of insight the file is retrieved from.</span></span> <span data-ttu-id="c6ddc-149">可以是 `trending` `used` 、、 或 `shared` 。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-149">Can be `trending`, `used`, or `shared`.</span></span> |
| <span data-ttu-id="c6ddc-150">insight-id</span><span class="sxs-lookup"><span data-stu-id="c6ddc-150">insight-id</span></span> | <span data-ttu-id="c6ddc-151">insightId</span><span class="sxs-lookup"><span data-stu-id="c6ddc-151">insightId</span></span> | <span data-ttu-id="c6ddc-152">见解资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-152">ID of the insight resource.</span></span> |
| <span data-ttu-id="c6ddc-153">file-details</span><span class="sxs-lookup"><span data-stu-id="c6ddc-153">file-details</span></span> | <span data-ttu-id="c6ddc-154">fileDetails</span><span class="sxs-lookup"><span data-stu-id="c6ddc-154">fileDetails</span></span> | <span data-ttu-id="c6ddc-155">设置为表示文件的对象</span><span class="sxs-lookup"><span data-stu-id="c6ddc-155">Set to an object representing a file</span></span> |
| <span data-ttu-id="c6ddc-156">file-icon</span><span class="sxs-lookup"><span data-stu-id="c6ddc-156">file-icon</span></span> | <span data-ttu-id="c6ddc-157">fileIcon</span><span class="sxs-lookup"><span data-stu-id="c6ddc-157">fileIcon</span></span> | <span data-ttu-id="c6ddc-158">设置为要显示文件的图标</span><span class="sxs-lookup"><span data-stu-id="c6ddc-158">Set to an icon to show for the file</span></span> |
| <span data-ttu-id="c6ddc-159">view</span><span class="sxs-lookup"><span data-stu-id="c6ddc-159">view</span></span> | <span data-ttu-id="c6ddc-160">view</span><span class="sxs-lookup"><span data-stu-id="c6ddc-160">view</span></span> | <span data-ttu-id="c6ddc-161">设置为控制文件的呈现方式。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-161">Set to control how the file is rendered.</span></span> <span data-ttu-id="c6ddc-162">默认值为 `oneline`。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-162">The default is `oneline`.</span></span> <br><span data-ttu-id="c6ddc-163">`image` - 只显示图标</span><span class="sxs-lookup"><span data-stu-id="c6ddc-163">`image` - show only the icon</span></span> <br><span data-ttu-id="c6ddc-164">`oneline` - 显示图标和一行文本 (默认为文件 `name`) </span><span class="sxs-lookup"><span data-stu-id="c6ddc-164">`oneline` - show the icon and one line of text (default is file `name`)</span></span> <br><span data-ttu-id="c6ddc-165">`twolines` - 显示图标和两行文本 (`name` `lastModifiedDateTime` 默认情况下显示) </span><span class="sxs-lookup"><span data-stu-id="c6ddc-165">`twolines` - show the icon and two lines of text (`name` and `lastModifiedDateTime` by default)</span></span><br> <span data-ttu-id="c6ddc-166">`threelines` - 默认显示作者的图标 (、、和三行 `name` `lastModifiedDateTime` `displayName` 文本) </span><span class="sxs-lookup"><span data-stu-id="c6ddc-166">`threelines` - show the icon and three lines of text (`name`, `lastModifiedDateTime`, and `displayName` of the author by default)</span></span> |
| <span data-ttu-id="c6ddc-167">line1-property</span><span class="sxs-lookup"><span data-stu-id="c6ddc-167">line1-property</span></span> | <span data-ttu-id="c6ddc-168">line1Property</span><span class="sxs-lookup"><span data-stu-id="c6ddc-168">line1Property</span></span> | <span data-ttu-id="c6ddc-169">设置 要 `fileDetails` 用于第一行文本的属性。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-169">Sets the property of `fileDetails` to use for the first line of text.</span></span> <span data-ttu-id="c6ddc-170">默认值 `name` 为 文件。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-170">Default is `name` of the file.</span></span> |
| <span data-ttu-id="c6ddc-171">line2-property</span><span class="sxs-lookup"><span data-stu-id="c6ddc-171">line2-property</span></span> | <span data-ttu-id="c6ddc-172">line2Property</span><span class="sxs-lookup"><span data-stu-id="c6ddc-172">line2Property</span></span> | <span data-ttu-id="c6ddc-173">设置 要 `fileDetails` 用于第二行文本的属性。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-173">Sets the property of `fileDetails` to use for the second line of text.</span></span> <span data-ttu-id="c6ddc-174">默认值为“`lastModifiedDateTime`”。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-174">Default is `lastModifiedDateTime`.</span></span> |
| <span data-ttu-id="c6ddc-175">line3-property</span><span class="sxs-lookup"><span data-stu-id="c6ddc-175">line3-property</span></span> | <span data-ttu-id="c6ddc-176">line3Property</span><span class="sxs-lookup"><span data-stu-id="c6ddc-176">line3Property</span></span> | <span data-ttu-id="c6ddc-177">设置 要 `fileDetails` 用于第三行文本的属性。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-177">Sets the property of `fileDetails` to use for the third line of text.</span></span> <span data-ttu-id="c6ddc-178">默认值 `size` 为 文件。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-178">Default is `size` of the file.</span></span> |

<span data-ttu-id="c6ddc-179">以下示例将组件的行为更改为从特定查询提取数据。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-179">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2"></mgt-file>
```

<span data-ttu-id="c6ddc-180">以下示例更改组件的行为以从特定查询提取数据，显示三行信息（默认情况下为文件名、上次修改日期时间和文件大小）并设置文件图标。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-180">The following example changes the behavior of the component to fetch data from a specific query, show three lines of information - file name, last modified date time, and file size by default - and set the file icon.</span></span>

```html
<mgt-file file-query="/me/drive/items/01BYE5RZZFWGWWVNHHKVHYXE3OUJHGWCT2" view="threeLines" file-icon="ICON_PATH"></mgt-file>
```

<span data-ttu-id="c6ddc-181">以下示例将组件的行为更改为从特定驱动器提取数据。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-181">The following example changes the behavior of the component to fetch data from a specific drive.</span></span>

```html
<mgt-file drive-id="b!-RIj2DuyvEyV1T4NlOaMHk8XkS_I8MdFlUCq1BlcjgmhRfAj3-Z8RY2VpuvV_tpd" item-id="01BYE5RZ5MYLM2SMX75ZBIPQZIHT6OAYPB"></mgt-file>
```

<span data-ttu-id="c6ddc-182">以下示例将组件的内容更改为从网站和路径SharePoint数据。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-182">The following example changes the behabior of the component to fetch data from a SharePoint site and path.</span></span>

```html
  <mgt-file site-id="m365x214355.sharepoint.com,5a58bb09-1fba-41c1-8125-69da264370a0,9f2ec1da-0be4-4a74-9254-973f0add78fd" item-Path="/DemoDocs/AdminDemo"></mgt-file>
```

<span data-ttu-id="c6ddc-183">以下示例将组件的行为更改为按见解类型提取数据。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-183">The following example changes the behavior of the component to fetch data by insight type.</span></span>

```html
<mgt-file insight-type="shared" insight-id="AW1GxMvkOztMkJX-SCppUSRPF5EvyPDHRZVAqtQZXI4JoUXwI9_mfEWNlabr1f7aXRBWDMt2C2FDop4fP1vsUw9tRsTL5Ds7TJCV_kgqaVEkBA"></mgt-file>
```

## <a name="css-custom-properties"></a><span data-ttu-id="c6ddc-184">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="c6ddc-184">CSS custom properties</span></span>

<span data-ttu-id="c6ddc-185">组件 `mgt-file` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-185">The `mgt-file` component defines the following CSS custom properties.</span></span>

```css
mgt-file {
  --file-type-icon-size: 28px;
  --file-border: none;
  --file-box-shadow: none;
  --file-background-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 400;
  --text-transform: none;
  --color: #323130;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: #797775;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: #797775;
  --line3-text-transform: none;
}
```

<span data-ttu-id="c6ddc-186">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-186">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="c6ddc-187">Microsoft Graph API 和权限</span><span class="sxs-lookup"><span data-stu-id="c6ddc-187">Microsoft Graph APIs and permissions</span></span>

<span data-ttu-id="c6ddc-188">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-188">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="c6ddc-189">配置</span><span class="sxs-lookup"><span data-stu-id="c6ddc-189">Configuration</span></span> | <span data-ttu-id="c6ddc-190">权限范围</span><span class="sxs-lookup"><span data-stu-id="c6ddc-190">Permission Scopes</span></span> | <span data-ttu-id="c6ddc-191">API</span><span class="sxs-lookup"><span data-stu-id="c6ddc-191">API</span></span> |
| ------------- | ----------------- | --- |
| <span data-ttu-id="c6ddc-192">开发人员提供 `{drive-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-192">Developer provides `{drive-id}` AND `{item-id}`</span></span> | <span data-ttu-id="c6ddc-193">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-193">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/items/{item-id}` |
| <span data-ttu-id="c6ddc-194">开发人员提供 `{drive-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-194">Developer provides `{drive-id}` AND `{item-path}`</span></span> | <span data-ttu-id="c6ddc-195">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-195">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /drives/{drive-id}/root:/{item-path}` |
| <span data-ttu-id="c6ddc-196">开发人员提供 `{group-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-196">Developer provides `{group-id}` AND `{item-id}`</span></span> | <span data-ttu-id="c6ddc-197">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-197">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/items/{item-id}` |
| <span data-ttu-id="c6ddc-198">开发人员提供 `{group-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-198">Developer provides `{group-id}` AND `{item-path}`</span></span> | <span data-ttu-id="c6ddc-199">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-199">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /groups/{group-id}/drive/root:/{item-path}` |
| <span data-ttu-id="c6ddc-200">开发人员提供 ONLY `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-200">Developer provides ONLY `{item-id}`</span></span> | <span data-ttu-id="c6ddc-201">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-201">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/items/{item-id}` |
| <span data-ttu-id="c6ddc-202">开发人员提供 ONLY `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-202">Developer provides ONLY `{item-path}`</span></span> | <span data-ttu-id="c6ddc-203">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-203">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /me/drive/root:/{item-path}` |
| <span data-ttu-id="c6ddc-204">开发人员提供 `{site-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-204">Developer provides `{site-id}` AND `{item-id}`</span></span> | <span data-ttu-id="c6ddc-205">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-205">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/items/{item-id}` |
| <span data-ttu-id="c6ddc-206">开发人员提供 `{site-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-206">Developer provides `{site-id}` AND `{item-path}`</span></span> | <span data-ttu-id="c6ddc-207">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-207">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/drive/root:/{item-path}` |
| <span data-ttu-id="c6ddc-208">开发人员提供 `{site-id}` AND `{list-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-208">Developer provides `{site-id}` AND `{list-id}` AND `{item-id}`</span></span> | <span data-ttu-id="c6ddc-209">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-209">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /sites/{site-id}/lists/{list-id}/items/{item-id}/driveItem` |
| <span data-ttu-id="c6ddc-210">开发人员提供 `{user-id}` AND `{item-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-210">Developer provides `{user-id}` AND `{item-id}`</span></span> | <span data-ttu-id="c6ddc-211">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-211">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/items/{item-id}` |
| <span data-ttu-id="c6ddc-212">开发人员提供 `{user-id}` AND `{item-path}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-212">Developer provides `{user-id}` AND `{item-path}`</span></span> | <span data-ttu-id="c6ddc-213">Files.Read、Files.Read.All、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-213">Files.Read, Files.Read.All, Sites.Read.All</span></span> | `GET /users/{user-id}/drive/root:/{item-path}` |
| <span data-ttu-id="c6ddc-214">`insight-type` 设置为 `trending` AND 开发人员提供 `{insight-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-214">`insight-type` is set to `trending` AND developer provides `{insight-id}`</span></span> | <span data-ttu-id="c6ddc-215">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-215">Sites.Read.All</span></span> | `GET /me/insights/trending/{insight-id}/resource` |
| <span data-ttu-id="c6ddc-216">开发人员提供 `{user-id or upn}` `{insight-id}` AND AND `insight-type` 设置为 `trending`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-216">Developer provides `{user-id or upn}` AND `{insight-id}` AND `insight-type` is set to `trending`</span></span> | <span data-ttu-id="c6ddc-217">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-217">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/trending/{insight-id}/resource` |
| <span data-ttu-id="c6ddc-218">`insight-type` 设置为 `used` AND 开发人员提供 `{insight-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-218">`insight-type` is set to `used` AND developer provides `{insight-id}`</span></span> | <span data-ttu-id="c6ddc-219">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-219">Sites.Read.All</span></span> | `GET /me/insights/used/{id}/resource` |
| <span data-ttu-id="c6ddc-220">开发人员提供 `{user-id or upn}` `{insight-id}` AND AND `insight-type` 设置为 `used`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-220">Developer provides `{user-id or upn}` AND `{insight-id}` AND `insight-type` is set to `used`</span></span> | <span data-ttu-id="c6ddc-221">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-221">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/used/{id}/resource` |
| <span data-ttu-id="c6ddc-222">`insight-type` is `shared` AND 开发人员提供 `{insight-id}`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-222">`insight-type` is `shared` AND developer provides `{insight-id}`</span></span> | <span data-ttu-id="c6ddc-223">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-223">Sites.Read.All</span></span> | `GET /me/insights/shared/{id}/resource` |
| <span data-ttu-id="c6ddc-224">开发人员提供 `{user-id or upn}` `{insight-id}` AND AND `insight-type` 设置为 `shared`</span><span class="sxs-lookup"><span data-stu-id="c6ddc-224">Developer provides `{user-id or upn}` AND `{insight-id}` AND `insight-type` is set to `shared`</span></span> | <span data-ttu-id="c6ddc-225">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6ddc-225">Sites.Read.All</span></span> | `GET /users/{id or userPrincipalName}/insights/shared/{id}/resource` |

## <a name="templates"></a><span data-ttu-id="c6ddc-226">模板</span><span class="sxs-lookup"><span data-stu-id="c6ddc-226">Templates</span></span>

<span data-ttu-id="c6ddc-227">组件 `mgt-file` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-227">The `mgt-file` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="c6ddc-228">若要指定模板，请包含组件 `<template>` 内的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="c6ddc-228">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="c6ddc-229">数据类型</span><span class="sxs-lookup"><span data-stu-id="c6ddc-229">Data Type</span></span> | <span data-ttu-id="c6ddc-230">数据上下文</span><span class="sxs-lookup"><span data-stu-id="c6ddc-230">Data Context</span></span> | <span data-ttu-id="c6ddc-231">说明</span><span class="sxs-lookup"><span data-stu-id="c6ddc-231">Description</span></span> |
| ----------- | -------------- | ------------- |
| <span data-ttu-id="c6ddc-232">loading</span><span class="sxs-lookup"><span data-stu-id="c6ddc-232">loading</span></span> | <span data-ttu-id="c6ddc-233">无</span><span class="sxs-lookup"><span data-stu-id="c6ddc-233">none</span></span> | <span data-ttu-id="c6ddc-234">组件在加载状态时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-234">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="c6ddc-235">no-data</span><span class="sxs-lookup"><span data-stu-id="c6ddc-235">no-data</span></span> | <span data-ttu-id="c6ddc-236">无</span><span class="sxs-lookup"><span data-stu-id="c6ddc-236">none</span></span> | <span data-ttu-id="c6ddc-237">在文件数据不可用时要呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-237">The template to render when no file data is available.</span></span> |
| <span data-ttu-id="c6ddc-238">default</span><span class="sxs-lookup"><span data-stu-id="c6ddc-238">default</span></span> | <span data-ttu-id="c6ddc-239">file：文件详细信息对象</span><span class="sxs-lookup"><span data-stu-id="c6ddc-239">file: the file details object</span></span> | <span data-ttu-id="c6ddc-240">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-240">The default template replaces the entire component with your own.</span></span> |

## <a name="authentication"></a><span data-ttu-id="c6ddc-241">身份验证</span><span class="sxs-lookup"><span data-stu-id="c6ddc-241">Authentication</span></span>

<span data-ttu-id="c6ddc-242">该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-242">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="c6ddc-243">缓存</span><span class="sxs-lookup"><span data-stu-id="c6ddc-243">Cache</span></span>

|<span data-ttu-id="c6ddc-244">对象存储</span><span class="sxs-lookup"><span data-stu-id="c6ddc-244">Object store</span></span>|<span data-ttu-id="c6ddc-245">缓存数据</span><span class="sxs-lookup"><span data-stu-id="c6ddc-245">Cached data</span></span>|<span data-ttu-id="c6ddc-246">备注</span><span class="sxs-lookup"><span data-stu-id="c6ddc-246">Remarks</span></span>|
|---------|-----------|-------|
|`driveFiles`|<span data-ttu-id="c6ddc-247">按驱动器 ID 列出文件</span><span class="sxs-lookup"><span data-stu-id="c6ddc-247">List of files by drive id</span></span>|<span data-ttu-id="c6ddc-248">提供时 `driveId` 使用</span><span class="sxs-lookup"><span data-stu-id="c6ddc-248">Used when `driveId` is provided</span></span>|
|`groupFiles`|<span data-ttu-id="c6ddc-249">按组 ID 列出文件</span><span class="sxs-lookup"><span data-stu-id="c6ddc-249">List of files by group id</span></span>|<span data-ttu-id="c6ddc-250">提供时 `groupId` 使用</span><span class="sxs-lookup"><span data-stu-id="c6ddc-250">Used when `groupId` is provided</span></span>|
|`siteFiles`|<span data-ttu-id="c6ddc-251">按网站 ID 列出文件</span><span class="sxs-lookup"><span data-stu-id="c6ddc-251">List of files by site id</span></span>|<span data-ttu-id="c6ddc-252">提供时 `siteId` 使用</span><span class="sxs-lookup"><span data-stu-id="c6ddc-252">Used when `siteId` is provided</span></span>|
|`userFiles`|<span data-ttu-id="c6ddc-253">按用户 ID 列出文件</span><span class="sxs-lookup"><span data-stu-id="c6ddc-253">List of files by user id</span></span>|<span data-ttu-id="c6ddc-254">提供时 `userId` 使用</span><span class="sxs-lookup"><span data-stu-id="c6ddc-254">Used when `userId` is provided</span></span>|
|`insightFiles`|<span data-ttu-id="c6ddc-255">按见解列出文件</span><span class="sxs-lookup"><span data-stu-id="c6ddc-255">List of files by insights</span></span>|<span data-ttu-id="c6ddc-256">提供 `insightType` 和 `insightId` 时使用</span><span class="sxs-lookup"><span data-stu-id="c6ddc-256">Used when `insightType` and `insightId` are provided</span></span>|
|`fileQueries`|<span data-ttu-id="c6ddc-257">按查询列出文件</span><span class="sxs-lookup"><span data-stu-id="c6ddc-257">List of files by queries</span></span>|<span data-ttu-id="c6ddc-258">提供时 `fileQuery` 使用</span><span class="sxs-lookup"><span data-stu-id="c6ddc-258">Used when `fileQuery` is provided</span></span>|

<span data-ttu-id="c6ddc-259">若要详细了解如何配置缓存[，请参阅](../customize-components/cache.md)Caching。</span><span class="sxs-lookup"><span data-stu-id="c6ddc-259">For details about how to configure the cache, see [Caching](../customize-components/cache.md).</span></span>