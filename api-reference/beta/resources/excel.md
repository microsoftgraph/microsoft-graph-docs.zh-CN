---
title: 在 Microsoft Graph 中使用 Excel
description: 可以使用 Microsoft Graph，使 Web 和移动应用程序可以读取和修改存储在 OneDrive、SharePoint 或其他支持的存储平台中的 Excel 工作簿。 （或 Excel 文件）资源通过关系包含所有其他 Excel 资源。 可以通过识别文件在该 URL 中的位置，借助 驱动器 API 访问工作簿。 例如：
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 8e054e884fdc70130b9a39731a0b2641d69689dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542928"
---
# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="9e090-106">在 Microsoft Graph 中使用 Excel</span><span class="sxs-lookup"><span data-stu-id="9e090-106">Working with Excel in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e090-p102">可以使用 Microsoft Graph，使 Web 和移动应用程序可以读取和修改存储在 OneDrive、SharePoint 或其他支持的存储平台中的 Excel 工作簿。`Workbook`（或 Excel 文件）资源通过关系包含所有其他 Excel 资源。可以通过识别文件在该 URL 中的位置，借助 [驱动器 API](drive.md) 访问工作簿。例如：</span><span class="sxs-lookup"><span data-stu-id="9e090-p102">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="9e090-p103">可以通过使用标准 REST API 访问一组 Excel 对象（例如表、区域或图表），以便对工作簿执行创建、读取、更新和删除 (CRUD) 操作。例如，`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span><span class="sxs-lookup"><span data-stu-id="9e090-p103">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="9e090-113">返回属于工作簿的工作表对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9e090-113">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="9e090-114">**注意:** Excel REST API 仅支持 Office Open XML 文件格式的工作簿。</span><span class="sxs-lookup"><span data-stu-id="9e090-114">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks.</span></span> <span data-ttu-id="9e090-115">不`.xls`支持扩展工作簿。</span><span class="sxs-lookup"><span data-stu-id="9e090-115">The `.xls` extension workbooks are not supported.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="9e090-116">授权和范围</span><span class="sxs-lookup"><span data-stu-id="9e090-116">Authorization and scopes</span></span>

<span data-ttu-id="9e090-p105">可以使用 [Azure AD v.20 终结点](https://developer.microsoft.com/graph/docs/authorization/converged_auth) 对 Excel API 进行身份验证。所有 API 都要求提供 `Authorization: Bearer {access-token}` HTTP 标头。</span><span class="sxs-lookup"><span data-stu-id="9e090-p105">You can use the [Azure AD v.20 endpoint](https://developer.microsoft.com/graph/docs/authorization/converged_auth) to authenticate Excel APIs. All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="9e090-119">要使用 Excel 资源，需要以下 [权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) 之一：</span><span class="sxs-lookup"><span data-stu-id="9e090-119">One of the following [permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="9e090-120">Files.Read</span><span class="sxs-lookup"><span data-stu-id="9e090-120">Files.Read</span></span> 
* <span data-ttu-id="9e090-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e090-121">Files.ReadWrite</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="9e090-122">会话和永久性</span><span class="sxs-lookup"><span data-stu-id="9e090-122">Sessions and persistence</span></span>

<span data-ttu-id="9e090-123">可以在以下任一模式下调用 Excel API：</span><span class="sxs-lookup"><span data-stu-id="9e090-123">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="9e090-p106">永久会话 - 保持（保存）对工作簿所做的全部更改。这是常用的操作模式。</span><span class="sxs-lookup"><span data-stu-id="9e090-p106">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="9e090-p107">非永久会话 - 不会将 API 所做的更改保存到源位置。相反，Excel 后端服务器保留文件的临时副本，体现在特定 API 会话期间所做的更改。Excel 会话过期时，这些更改将丢失。此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。</span><span class="sxs-lookup"><span data-stu-id="9e090-p107">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="9e090-130">若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。</span><span class="sxs-lookup"><span data-stu-id="9e090-130">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="9e090-p108">**注意：** Excel API 不需要会话标头也能起作用。但是，建议你使用会话标头来提高性能。如果不使用会话标头，API 调用过程中进行的更改_仅_保持在该文件中。</span><span class="sxs-lookup"><span data-stu-id="9e090-p108">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="9e090-134">获取会话的 API 调用</span><span class="sxs-lookup"><span data-stu-id="9e090-134">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="9e090-135">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-135">Request</span></span> 

<span data-ttu-id="9e090-136">通过将 `persistchanges` 值设置为 `true` 或 `false` 可传递一个 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9e090-136">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="9e090-137">如果 `persistChanges` 值设置为 `false`，返回非永久会话 ID。</span><span class="sxs-lookup"><span data-stu-id="9e090-137">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="9e090-138">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-138">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="9e090-139">用法</span><span class="sxs-lookup"><span data-stu-id="9e090-139">Usage</span></span> 

<span data-ttu-id="9e090-140">将前一个调用中返回的会话 ID</span><span class="sxs-lookup"><span data-stu-id="9e090-140">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="9e090-141">作为 `workbook-session-id` HTTP 标头的后续 API 请求中的标头进行传递。</span><span class="sxs-lookup"><span data-stu-id="9e090-141">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="9e090-142">注意: 如果会话 id 已过期, 则会`404`在会话中返回 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="9e090-142">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="9e090-143">在此类 scenarion 中, 可以选择创建新会话并继续。</span><span class="sxs-lookup"><span data-stu-id="9e090-143">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="9e090-144">另一种方法是定期刷新会话以保持会话处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="9e090-144">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="9e090-145">通常情况下, 持续会话在大约7分钟的不活动状态后过期。</span><span class="sxs-lookup"><span data-stu-id="9e090-145">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="9e090-146">非永久会话在大约5分钟不活动后过期。</span><span class="sxs-lookup"><span data-stu-id="9e090-146">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="9e090-147">常见的 Excel 方案</span><span class="sxs-lookup"><span data-stu-id="9e090-147">Common Excel scenarios</span></span>

<span data-ttu-id="9e090-148">本节提供可用于 Excel 对象的常见操作的示例。</span><span class="sxs-lookup"><span data-stu-id="9e090-148">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="9e090-149">工作表操作</span><span class="sxs-lookup"><span data-stu-id="9e090-149">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="9e090-150">列出工作簿的工作表部分</span><span class="sxs-lookup"><span data-stu-id="9e090-150">List worksheets part of the workbook</span></span> 
<span data-ttu-id="9e090-151">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-151">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-152">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-152">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="9e090-153">添加新的工作表</span><span class="sxs-lookup"><span data-stu-id="9e090-153">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="9e090-154">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-154">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="9e090-155">获取新工作表</span><span class="sxs-lookup"><span data-stu-id="9e090-155">Get a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-156">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-156">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

<span data-ttu-id="9e090-157">\* \* 注意: 还可以使用 ID 检索工作表。</span><span class="sxs-lookup"><span data-stu-id="9e090-157">\*\* Note: Worksheets can also be retrieved using the ID.</span></span> <span data-ttu-id="9e090-158">但是, 当前 ID 包含`{`和 '} ' 字符, 这些字符需要经过 URL 编码, API 才能正常工作。</span><span class="sxs-lookup"><span data-stu-id="9e090-158">However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work.</span></span> <span data-ttu-id="9e090-159">示例: 若要获取 ID 为的`{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`工作表, URL 会将路径中的 ID 编码为`/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`。</span><span class="sxs-lookup"><span data-stu-id="9e090-159">Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="9e090-160">删除工作表</span><span class="sxs-lookup"><span data-stu-id="9e090-160">Delete a worksheet</span></span>

<span data-ttu-id="9e090-161">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-161">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-162">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-162">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="9e090-163">更新工作表属性</span><span class="sxs-lookup"><span data-stu-id="9e090-163">Update worksheet properties</span></span>

<span data-ttu-id="9e090-164">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-164">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="9e090-165">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-165">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a><span data-ttu-id="9e090-166">图表操作</span><span class="sxs-lookup"><span data-stu-id="9e090-166">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="9e090-167">列出属于工作表的图表</span><span class="sxs-lookup"><span data-stu-id="9e090-167">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="9e090-168">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-168">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="9e090-169">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-169">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

<span data-ttu-id="9e090-170">\* \* 注意: 图表 ID 包含`{`和`}`字符 (例如: `{00000000-0008-0000-0100-000003000000}`), 需要 URL 编码才能使 API 正常工作。</span><span class="sxs-lookup"><span data-stu-id="9e090-170">\*\* Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work.</span></span> <span data-ttu-id="9e090-171">示例: 为了获取 chart 对象, URL 将路径中的 ID 编码为`/charts/%7B00000000-0008-0000-0100-000003000000%7D`。</span><span class="sxs-lookup"><span data-stu-id="9e090-171">Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="9e090-172">获取图表图像</span><span class="sxs-lookup"><span data-stu-id="9e090-172">Get chart image</span></span>

<span data-ttu-id="9e090-173">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-173">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="9e090-174">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-174">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="9e090-175">添加图表</span><span class="sxs-lookup"><span data-stu-id="9e090-175">Add a chart</span></span>  

<span data-ttu-id="9e090-176">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-176">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="9e090-177">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-177">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#chart",
  "@odata.type": "#microsoft.graph.chart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="9e090-178">更新图表</span><span class="sxs-lookup"><span data-stu-id="9e090-178">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="9e090-179">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-179">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a><span data-ttu-id="9e090-180">更新图表的源数据</span><span class="sxs-lookup"><span data-stu-id="9e090-180">Update chart source data</span></span> 

<span data-ttu-id="9e090-181">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-181">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="9e090-182">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-182">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="9e090-183">表操作</span><span class="sxs-lookup"><span data-stu-id="9e090-183">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="9e090-184">获取表列表</span><span class="sxs-lookup"><span data-stu-id="9e090-184">Get list of tables</span></span> 

<span data-ttu-id="9e090-185">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-185">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-186">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-186">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="9e090-187">创建表</span><span class="sxs-lookup"><span data-stu-id="9e090-187">Create table</span></span>

<span data-ttu-id="9e090-188">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-188">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/$/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="9e090-189">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-189">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="update-table"></a><span data-ttu-id="9e090-190">更新表</span><span class="sxs-lookup"><span data-stu-id="9e090-190">Update table</span></span>

<span data-ttu-id="9e090-191">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-191">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="9e090-192">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-192">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="9e090-193">获取表行列表</span><span class="sxs-lookup"><span data-stu-id="9e090-193">Get list of table rows</span></span>
<span data-ttu-id="9e090-194">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-194">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-195">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-195">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="9e090-196">获取表列列表</span><span class="sxs-lookup"><span data-stu-id="9e090-196">Get list of table columns</span></span>

<span data-ttu-id="9e090-197">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-197">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-198">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-198">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a><span data-ttu-id="9e090-199">添加表行</span><span class="sxs-lookup"><span data-stu-id="9e090-199">Add a table row</span></span>

<span data-ttu-id="9e090-200">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-200">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="9e090-201">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-201">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a><span data-ttu-id="9e090-202">添加表列</span><span class="sxs-lookup"><span data-stu-id="9e090-202">Add a table column</span></span> 

<span data-ttu-id="9e090-203">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-203">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/Columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="9e090-204">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-204">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a><span data-ttu-id="9e090-205">删除表行</span><span class="sxs-lookup"><span data-stu-id="9e090-205">Delete table row</span></span>

<span data-ttu-id="9e090-206">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-206">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows/$/ItemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-207">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-207">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="9e090-208">删除表列</span><span class="sxs-lookup"><span data-stu-id="9e090-208">Delete table column</span></span> 
<span data-ttu-id="9e090-209">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-209">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-210">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-210">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="9e090-211">将表转换为区域</span><span class="sxs-lookup"><span data-stu-id="9e090-211">Convert table to range</span></span> 
<span data-ttu-id="9e090-212">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-212">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-213">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-213">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="9e090-214">表排序</span><span class="sxs-lookup"><span data-stu-id="9e090-214">Table sort</span></span>
<span data-ttu-id="9e090-215">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-215">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


<span data-ttu-id="9e090-216">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-216">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="9e090-217">表筛选器</span><span class="sxs-lookup"><span data-stu-id="9e090-217">Table filter</span></span>
<span data-ttu-id="9e090-218">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-218">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

<span data-ttu-id="9e090-219">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-219">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="9e090-220">清除筛选器</span><span class="sxs-lookup"><span data-stu-id="9e090-220">Clear filter</span></span>
<span data-ttu-id="9e090-221">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-221">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-222">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-222">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="9e090-223">区域操作</span><span class="sxs-lookup"><span data-stu-id="9e090-223">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="9e090-224">获取范围</span><span class="sxs-lookup"><span data-stu-id="9e090-224">Get Range</span></span> 

<span data-ttu-id="9e090-225">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-225">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-226">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-226">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a><span data-ttu-id="9e090-227">区域更新</span><span class="sxs-lookup"><span data-stu-id="9e090-227">Range update</span></span> 

<!-- { "blockType": "ignored" } -->
```http
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a><span data-ttu-id="9e090-228">区域排序</span><span class="sxs-lookup"><span data-stu-id="9e090-228">Range sort</span></span>
<span data-ttu-id="9e090-229">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-229">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

<span data-ttu-id="9e090-230">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-230">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="9e090-231">已命名项目</span><span class="sxs-lookup"><span data-stu-id="9e090-231">Named items</span></span>
<span data-ttu-id="9e090-232">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-232">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9e090-233">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-233">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a><span data-ttu-id="9e090-234">使用 null</span><span class="sxs-lookup"><span data-stu-id="9e090-234">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="9e090-235">二维数组中的 null 输入</span><span class="sxs-lookup"><span data-stu-id="9e090-235">null input in 2-D array</span></span>

<span data-ttu-id="9e090-p112">区域和表资源中将忽略二维数组中的 `null` 输入（对于值、数字格式、公式）。当 `null` 输入在值、值的数字格式或值的公式网格中发送时，不会对预期目标（单元格）进行更新。</span><span class="sxs-lookup"><span data-stu-id="9e090-p112">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="9e090-238">例如，要仅更新区域的特定部分（例如某些单元格的数字格式）并保留区域其他部分的现有数字格式，请根据需要设置数字格式并对其他单元格发送 `null`。</span><span class="sxs-lookup"><span data-stu-id="9e090-238">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="9e090-239">在以下设置请求中，仅会设置区域数字格式的某些部分，同时保留其余部分的现有数字格式（通过传递 null）。</span><span class="sxs-lookup"><span data-stu-id="9e090-239">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="9e090-240">属性的 null 输入</span><span class="sxs-lookup"><span data-stu-id="9e090-240">null input for a property</span></span>

<span data-ttu-id="9e090-p113">`null` 并非整个属性的有效的单个输入。例如，以下输入无效，因为整个值不能设置为 null，也不能忽略。</span><span class="sxs-lookup"><span data-stu-id="9e090-p113">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="9e090-243">以下输入无效，因为 null 不是有效的颜色值。</span><span class="sxs-lookup"><span data-stu-id="9e090-243">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="9e090-244">Null 响应</span><span class="sxs-lookup"><span data-stu-id="9e090-244">Null-Response</span></span>

<span data-ttu-id="9e090-245">由不一致的值组成的格式属性的表示形式将导致在响应中返回 null 值。</span><span class="sxs-lookup"><span data-stu-id="9e090-245">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="9e090-p114">例如，区域可以由一个或多个单元格组成。如果指定区域中包含的单个单元格不具有一致的格式值，则不会定义区域级别表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e090-p114">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="9e090-248">空白输入和输出</span><span class="sxs-lookup"><span data-stu-id="9e090-248">Blank input and output</span></span>

<span data-ttu-id="9e090-p115">更新请求中的空白值视为清除或重置相应属性的指令。空白值表示为两个双引号，中间没有空格：`""`。</span><span class="sxs-lookup"><span data-stu-id="9e090-p115">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="9e090-251">示例：</span><span class="sxs-lookup"><span data-stu-id="9e090-251">Examples:</span></span>

* <span data-ttu-id="9e090-252">对于 `values`，将清除区域值。这与清除应用程序中的内容相同。</span><span class="sxs-lookup"><span data-stu-id="9e090-252">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="9e090-253">对于 `numberFormat`，数字格式设置为 `General`。</span><span class="sxs-lookup"><span data-stu-id="9e090-253">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="9e090-254">对于 `formula` 和 `formulaLocale`，将清除公式值。</span><span class="sxs-lookup"><span data-stu-id="9e090-254">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="9e090-p116">对于读取操作，预计单元格内容为空时会收到空白值。如果单元格不包含数据或值，该 API 将返回空白值。空白值表示为两个双引号，中间没有空格：`""`。</span><span class="sxs-lookup"><span data-stu-id="9e090-p116">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a><span data-ttu-id="9e090-258">无限区域</span><span class="sxs-lookup"><span data-stu-id="9e090-258">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="9e090-259">阅读</span><span class="sxs-lookup"><span data-stu-id="9e090-259">Read</span></span>

<span data-ttu-id="9e090-260">无限区域地址仅包含列或行标识符和未指定的行标识符或列标识符（分别），例如：</span><span class="sxs-lookup"><span data-stu-id="9e090-260">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="9e090-261">`C:C`、`A:F`、`A:XFD`（包含未指定的行）</span><span class="sxs-lookup"><span data-stu-id="9e090-261">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="9e090-262">`2:2`、`1:4`、`1:1048546`（包含未指定的列）</span><span class="sxs-lookup"><span data-stu-id="9e090-262">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="9e090-p117">当 API 发出检索无限区域 (`getRange('C:C')`) 的请求时，返回的响应包含单元格级别属性的 `null`例如 `values`、`text`、`numberFormat` 或 `formula`。其他区域属性（例如 `address` 或 `cellCount`）将反映无限区域。</span><span class="sxs-lookup"><span data-stu-id="9e090-p117">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="9e090-265">写入</span><span class="sxs-lookup"><span data-stu-id="9e090-265">Write</span></span>

<span data-ttu-id="9e090-266">**不允许**在无限区域上设置单元格级别属性（例如值、numberFormat 等），因为输入请求可能过大而无法处理。</span><span class="sxs-lookup"><span data-stu-id="9e090-266">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="9e090-267">例如，下面不是一个有效的更新请求，因为所请求的区域是无限的。</span><span class="sxs-lookup"><span data-stu-id="9e090-267">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="9e090-268">当尝试对此类区域执行更新操作时，API 将返回错误。</span><span class="sxs-lookup"><span data-stu-id="9e090-268">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="9e090-269">大区域</span><span class="sxs-lookup"><span data-stu-id="9e090-269">Large Range</span></span>

<span data-ttu-id="9e090-p118">大区域意味着区域大小对于单个 API 调用来说过大。区域中包含的很多因素（例如单元格数量、值、numberFormat 和公式）都会使响应过大，而不适合于 API 交互。API 努力尝试返回或写入到请求的数据。但是，由于资源利用率较高，涉及的大尺寸可能会导致 API 错误的情况。</span><span class="sxs-lookup"><span data-stu-id="9e090-p118">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="9e090-274">为了避免出现这种情况，建议以多个较小的区域大小对大区域执行读取或写入。</span><span class="sxs-lookup"><span data-stu-id="9e090-274">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="9e090-275">单个输入副本</span><span class="sxs-lookup"><span data-stu-id="9e090-275">Single input copy</span></span>

<span data-ttu-id="9e090-p119">为了支持使用相同的值或数字格式更新区域或在整个区域应用相同的公式，在一组 API 中使用以下约定。在 Excel 中，此行为与在 CTRL+Enter 模式下将值或公式输入到区域中相似。</span><span class="sxs-lookup"><span data-stu-id="9e090-p119">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="9e090-278">API 将查找*单个单元格值*，如果目标区域尺寸与输入区域尺寸不符，它将在 CTRL+Enter 模式下，使用请求中提供的值或公式更新整个区域。</span><span class="sxs-lookup"><span data-stu-id="9e090-278">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="9e090-279">示例</span><span class="sxs-lookup"><span data-stu-id="9e090-279">Examples</span></span>

<span data-ttu-id="9e090-p120">以下请求使用“Sample text”文本更新选定的区域。请注意，区域包含 200 个单元格，而提供的输入仅包含 1 个单元格值。</span><span class="sxs-lookup"><span data-stu-id="9e090-p120">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="9e090-282">工作簿函数</span><span class="sxs-lookup"><span data-stu-id="9e090-282">Workbook functions</span></span> 
<span data-ttu-id="9e090-283">可以通过 /Functions 资源中包含的函数集合访问工作簿函数。</span><span class="sxs-lookup"><span data-stu-id="9e090-283">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="9e090-284">请求</span><span class="sxs-lookup"><span data-stu-id="9e090-284">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="9e090-285">响应</span><span class="sxs-lookup"><span data-stu-id="9e090-285">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="9e090-286">错误信息</span><span class="sxs-lookup"><span data-stu-id="9e090-286">Error information</span></span> 

<span data-ttu-id="9e090-p121">返回错误，其中包括 HTTP 错误代码和错误对象。错误 `code` 和 `message` 解释了导致错误的原因。</span><span class="sxs-lookup"><span data-stu-id="9e090-p121">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="9e090-289">示例如下。</span><span class="sxs-lookup"><span data-stu-id="9e090-289">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/excel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
