---
title: 获取 onenoteOperation
description: '获取长时间运行的操作OneNote状态。 这适用于在响应中返回 **Operation-Location** 标头的操作，如 、 `CopyNotebook` `CopyToNotebook` 、 `CopyToSectionGroup` 、 `and CopyToSection` 。   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 3bb2cdf5eca3df3484273f99f10132cb1a80491d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050400"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="53729-104">获取 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="53729-104">Get onenoteOperation</span></span>

<span data-ttu-id="53729-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53729-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53729-106">获取长时间运行的操作OneNote状态。</span><span class="sxs-lookup"><span data-stu-id="53729-106">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="53729-107">这适用于在响应中返回 **Operation-Location** 标头的操作，如 、 `CopyNotebook` `CopyToNotebook` 、 `CopyToSectionGroup` 、 `and CopyToSection` 。</span><span class="sxs-lookup"><span data-stu-id="53729-107">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="53729-108">你可以轮询 Operation-Location 终结点，直到 `status` 属性返回 `completed` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="53729-108">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="53729-109">如果状态为 `completed` ， `resourceLocation` 则 属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="53729-109">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="53729-110">如果状态为 `failed` ，则错误 `@api.diagnostics` 和属性提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="53729-110">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="53729-111">权限</span><span class="sxs-lookup"><span data-stu-id="53729-111">Permissions</span></span>
<span data-ttu-id="53729-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53729-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53729-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="53729-114">Permission type</span></span>      | <span data-ttu-id="53729-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53729-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53729-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53729-116">Delegated (work or school account)</span></span> | <span data-ttu-id="53729-117">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53729-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="53729-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53729-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53729-119">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53729-119">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="53729-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="53729-120">Application</span></span> | <span data-ttu-id="53729-121">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53729-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53729-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53729-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53729-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53729-123">Optional query parameters</span></span>
<span data-ttu-id="53729-124">无。</span><span class="sxs-lookup"><span data-stu-id="53729-124">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53729-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="53729-125">Request headers</span></span>
| <span data-ttu-id="53729-126">名称</span><span class="sxs-lookup"><span data-stu-id="53729-126">Name</span></span>       | <span data-ttu-id="53729-127">类型</span><span class="sxs-lookup"><span data-stu-id="53729-127">Type</span></span> | <span data-ttu-id="53729-128">说明</span><span class="sxs-lookup"><span data-stu-id="53729-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53729-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="53729-129">Authorization</span></span>  | <span data-ttu-id="53729-130">string</span><span class="sxs-lookup"><span data-stu-id="53729-130">string</span></span>  | <span data-ttu-id="53729-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53729-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53729-133">接受</span><span class="sxs-lookup"><span data-stu-id="53729-133">Accept</span></span> | <span data-ttu-id="53729-134">string</span><span class="sxs-lookup"><span data-stu-id="53729-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="53729-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="53729-135">Request body</span></span>
<span data-ttu-id="53729-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53729-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53729-137">响应</span><span class="sxs-lookup"><span data-stu-id="53729-137">Response</span></span>

<span data-ttu-id="53729-138">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [onenoteOperation](../resources/onenoteoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53729-138">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53729-139">示例</span><span class="sxs-lookup"><span data-stu-id="53729-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53729-140">请求</span><span class="sxs-lookup"><span data-stu-id="53729-140">Request</span></span>
<span data-ttu-id="53729-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53729-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53729-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="53729-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="53729-143">C#</span><span class="sxs-lookup"><span data-stu-id="53729-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53729-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53729-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53729-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53729-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53729-146">Java</span><span class="sxs-lookup"><span data-stu-id="53729-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onenoteoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53729-147">响应</span><span class="sxs-lookup"><span data-stu-id="53729-147">Response</span></span>
<span data-ttu-id="53729-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53729-148">Here is an example of the response.</span></span> <span data-ttu-id="53729-149">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53729-149">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

