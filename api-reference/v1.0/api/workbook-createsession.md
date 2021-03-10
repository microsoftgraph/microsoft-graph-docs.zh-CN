---
title: workbook： createSession
description: 创建新的工作簿会话。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f931313e09068892ebbe167ecb85d5577a148f92
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575054"
---
# <a name="workbook-createsession"></a><span data-ttu-id="f626d-103">workbook： createSession</span><span class="sxs-lookup"><span data-stu-id="f626d-103">workbook: createSession</span></span>

<span data-ttu-id="f626d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f626d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f626d-105">创建新的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="f626d-105">Create a new workbook session.</span></span> 

<span data-ttu-id="f626d-106">可以在以下任一模式下调用 Excel API：</span><span class="sxs-lookup"><span data-stu-id="f626d-106">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="f626d-p101">永久会话 - 保持（保存）对工作簿所做的全部更改。这是常用的操作模式。</span><span class="sxs-lookup"><span data-stu-id="f626d-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="f626d-p102">非永久会话 - 不会将 API 所做的更改保存到源位置。相反，Excel 后端服务器保留文件的临时副本，体现在特定 API 会话期间所做的更改。Excel 会话过期时，这些更改将丢失。此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。</span><span class="sxs-lookup"><span data-stu-id="f626d-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="f626d-113">若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。</span><span class="sxs-lookup"><span data-stu-id="f626d-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="f626d-p103">**注意：** Excel API 不需要会话标头也能起作用。但是，建议你使用会话标头来提高性能。如果不使用会话标头，API 调用过程中进行的更改 _仅_ 保持在该文件中。</span><span class="sxs-lookup"><span data-stu-id="f626d-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

<span data-ttu-id="f626d-117">在某些情况下，创建新会话需要不确定的时间才能完成。</span><span class="sxs-lookup"><span data-stu-id="f626d-117">In some cases, creating a new session requires an indeterminate time to complete.</span></span> <span data-ttu-id="f626d-118">Microsoft Graph 还提供长时间运行的操作模式。</span><span class="sxs-lookup"><span data-stu-id="f626d-118">Microsoft Graph also provides a long running operations pattern.</span></span> <span data-ttu-id="f626d-119">此模式提供了一种轮询创建状态更新的方法，而无需等待创建完成。</span><span class="sxs-lookup"><span data-stu-id="f626d-119">This pattern provides a way to poll for creation status updates, without waiting for the creation to complete.</span></span> <span data-ttu-id="f626d-120">步骤如下：</span><span class="sxs-lookup"><span data-stu-id="f626d-120">The following are the steps:</span></span>

1. <span data-ttu-id="f626d-121">标头 `Prefer: respond-async` 将添加到请求中，以指示这是长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="f626d-121">A `Prefer: respond-async` header is added to the request to indicate that it is a long-running operation.</span></span>
2. <span data-ttu-id="f626d-122">响应返回一 `Location` 个标头以指定轮询创建操作状态的 URL。</span><span class="sxs-lookup"><span data-stu-id="f626d-122">The response returns a `Location` header to specify the URL for polling the creation operation status.</span></span> <span data-ttu-id="f626d-123">可以通过访问指定的 URL 获取操作状态。</span><span class="sxs-lookup"><span data-stu-id="f626d-123">You can get the operation status by accessing the specified URL.</span></span> <span data-ttu-id="f626d-124">状态将为以下项之一：、、 `notStarted` `running` `succeeded` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="f626d-124">The status will be one of the following: `notStarted`, `running`, `succeeded`, or `failed`.</span></span>
3. <span data-ttu-id="f626d-125">操作完成后，可以再次请求状态，响应将显示或 `succeeded` `failed` 。</span><span class="sxs-lookup"><span data-stu-id="f626d-125">After the operation completes, you can request the status again and the response will show either `succeeded` or `failed`.</span></span>

## <a name="error-handling"></a><span data-ttu-id="f626d-126">错误处理</span><span class="sxs-lookup"><span data-stu-id="f626d-126">Error handling</span></span>

<span data-ttu-id="f626d-127">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="f626d-127">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="f626d-128">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="f626d-128">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="f626d-129">权限</span><span class="sxs-lookup"><span data-stu-id="f626d-129">Permissions</span></span>
<span data-ttu-id="f626d-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f626d-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f626d-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="f626d-132">Permission type</span></span>      | <span data-ttu-id="f626d-133">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f626d-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f626d-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f626d-134">Delegated (work or school account)</span></span> | <span data-ttu-id="f626d-135">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f626d-135">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f626d-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f626d-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f626d-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="f626d-137">Not supported.</span></span>    |
|<span data-ttu-id="f626d-138">Application</span><span class="sxs-lookup"><span data-stu-id="f626d-138">Application</span></span> | <span data-ttu-id="f626d-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="f626d-139">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f626d-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f626d-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/createSession
POST /me/drive/root:/{item-path}:/workbook/createSession
```
## <a name="request-headers"></a><span data-ttu-id="f626d-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="f626d-141">Request headers</span></span>
| <span data-ttu-id="f626d-142">名称</span><span class="sxs-lookup"><span data-stu-id="f626d-142">Name</span></span>       | <span data-ttu-id="f626d-143">说明</span><span class="sxs-lookup"><span data-stu-id="f626d-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f626d-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="f626d-144">Authorization</span></span>  | <span data-ttu-id="f626d-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f626d-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f626d-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="f626d-147">Request body</span></span>
<span data-ttu-id="f626d-148">在请求正文中，提供 [workbookSessionInfo](../resources/workbooksessioninfo.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f626d-148">In the request body, supply a JSON representation of [workbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f626d-149">响应</span><span class="sxs-lookup"><span data-stu-id="f626d-149">Response</span></span>

<span data-ttu-id="f626d-150">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [workbookSessionInfo](../resources/workbooksessioninfo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f626d-150">If successful, this method returns a `201 Created` response code and a [workbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span> <span data-ttu-id="f626d-151">对于长时间运行的操作，它会在响应中返回一个响应代码和一个正文为空 `202 Accepted ` `Location` 的标头。</span><span class="sxs-lookup"><span data-stu-id="f626d-151">For a long-running operation, it returns a `202 Accepted ` response code and a `Location` header with an empty body in the response.</span></span>

## <a name="examples"></a><span data-ttu-id="f626d-152">示例</span><span class="sxs-lookup"><span data-stu-id="f626d-152">Examples</span></span>

### <a name="example-1-basic-session-creation"></a><span data-ttu-id="f626d-153">示例 1：基本会话创建</span><span class="sxs-lookup"><span data-stu-id="f626d-153">Example 1: Basic session creation</span></span>
#### <a name="request"></a><span data-ttu-id="f626d-154">请求</span><span class="sxs-lookup"><span data-stu-id="f626d-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f626d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f626d-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[<span data-ttu-id="f626d-156">C#</span><span class="sxs-lookup"><span data-stu-id="f626d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f626d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f626d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f626d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f626d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f626d-159">Java</span><span class="sxs-lookup"><span data-stu-id="f626d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f626d-160">响应</span><span class="sxs-lookup"><span data-stu-id="f626d-160">Response</span></span>
><span data-ttu-id="f626d-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f626d-161">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

### <a name="example-2-session-creation-with-long-running-operation-pattern"></a><span data-ttu-id="f626d-162">示例 2：使用长时间运行的操作模式创建会话</span><span class="sxs-lookup"><span data-stu-id="f626d-162">Example 2: Session creation with long-running operation pattern</span></span>

#### <a name="request"></a><span data-ttu-id="f626d-163">请求</span><span class="sxs-lookup"><span data-stu-id="f626d-163">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a><span data-ttu-id="f626d-164">响应</span><span class="sxs-lookup"><span data-stu-id="f626d-164">Response</span></span>
><span data-ttu-id="f626d-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f626d-165">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

