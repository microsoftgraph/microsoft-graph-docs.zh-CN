---
title: 创建会话
description: '使用此 API 创建新的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8d8da9c17656bf2c54662a902dfc59ebeb9d44f9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637029"
---
# <a name="create-session"></a><span data-ttu-id="df315-103">创建会话</span><span class="sxs-lookup"><span data-stu-id="df315-103">Create Session</span></span>

<span data-ttu-id="df315-104">使用此 API 创建新的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="df315-104">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="df315-105">可以在以下任一模式下调用 Excel API：</span><span class="sxs-lookup"><span data-stu-id="df315-105">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="df315-p101">永久会话 - 保持（保存）对工作簿所做的全部更改。这是常用的操作模式。</span><span class="sxs-lookup"><span data-stu-id="df315-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="df315-p102">非永久会话 - 不会将 API 所做的更改保存到源位置。相反，Excel 后端服务器保留文件的临时副本，体现在特定 API 会话期间所做的更改。Excel 会话过期时，这些更改将丢失。此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。</span><span class="sxs-lookup"><span data-stu-id="df315-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="df315-112">若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。</span><span class="sxs-lookup"><span data-stu-id="df315-112">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="df315-p103">**注意：** Excel API 不需要会话标头也能起作用。但是，建议你使用会话标头来提高性能。如果不使用会话标头，API 调用过程中进行的更改_仅_保持在该文件中。</span><span class="sxs-lookup"><span data-stu-id="df315-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="df315-116">错误处理</span><span class="sxs-lookup"><span data-stu-id="df315-116">Error Handling</span></span>

<span data-ttu-id="df315-117">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="df315-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="df315-118">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="df315-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="df315-119">权限</span><span class="sxs-lookup"><span data-stu-id="df315-119">Permissions</span></span>
<span data-ttu-id="df315-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df315-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df315-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="df315-122">Permission type</span></span>      | <span data-ttu-id="df315-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df315-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df315-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df315-124">Delegated (work or school account)</span></span> | <span data-ttu-id="df315-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df315-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df315-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df315-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df315-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="df315-127">Not supported.</span></span>    |
|<span data-ttu-id="df315-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="df315-128">Application</span></span> | <span data-ttu-id="df315-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="df315-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df315-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df315-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="df315-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="df315-131">Request headers</span></span>
| <span data-ttu-id="df315-132">名称</span><span class="sxs-lookup"><span data-stu-id="df315-132">Name</span></span>       | <span data-ttu-id="df315-133">说明</span><span class="sxs-lookup"><span data-stu-id="df315-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df315-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="df315-134">Authorization</span></span>  | <span data-ttu-id="df315-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df315-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df315-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="df315-137">Request body</span></span>
<span data-ttu-id="df315-138">在请求正文中，提供 [WorkbookSessionInfo](../resources/workbooksessioninfo.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df315-138">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df315-139">响应</span><span class="sxs-lookup"><span data-stu-id="df315-139">Response</span></span>

<span data-ttu-id="df315-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [WorkbookSessionInfo](../resources/workbooksessioninfo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df315-140">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df315-141">示例</span><span class="sxs-lookup"><span data-stu-id="df315-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df315-142">请求</span><span class="sxs-lookup"><span data-stu-id="df315-142">Request</span></span>
<span data-ttu-id="df315-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df315-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
<span data-ttu-id="df315-144">在请求正文中，提供 [WorkbookSessionInfo](../resources/workbooksessioninfo.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df315-144">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="df315-145">响应</span><span class="sxs-lookup"><span data-stu-id="df315-145">Response</span></span>
<span data-ttu-id="df315-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df315-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="df315-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="df315-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="df315-150">语言</span><span class="sxs-lookup"><span data-stu-id="df315-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df315-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="df315-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_excel_session-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-createsession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbook-createsession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
