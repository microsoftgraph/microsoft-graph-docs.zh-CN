---
title: 获取 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。 这适用于在响应中返回 **操作位置** 标头的操作，例如、、 `CopyNotebook` `CopyToNotebook` `CopyToSectionGroup` 、 `and CopyToSection` 。   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 0e5dc0d15ce7152a9713bbd1729b22cc901762c7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969337"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="7feaa-104">获取 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="7feaa-104">Get onenoteOperation</span></span>

<span data-ttu-id="7feaa-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7feaa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7feaa-106">获取长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7feaa-106">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="7feaa-107">这适用于在响应中返回 **操作位置** 标头的操作，例如、、 `CopyNotebook` `CopyToNotebook` `CopyToSectionGroup` 、 `and CopyToSection` 。</span><span class="sxs-lookup"><span data-stu-id="7feaa-107">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="7feaa-108">您可以轮询 Operation-Location 终结点，直到 `status` 属性返回 `completed` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="7feaa-108">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="7feaa-109">如果状态为 `completed` ，则 `resourceLocation` 属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="7feaa-109">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="7feaa-110">如果状态为 `failed` ，则错误和 `@api.diagnostics` 属性将提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="7feaa-110">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="7feaa-111">权限</span><span class="sxs-lookup"><span data-stu-id="7feaa-111">Permissions</span></span>
<span data-ttu-id="7feaa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7feaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7feaa-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7feaa-114">Permission type</span></span>      | <span data-ttu-id="7feaa-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7feaa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7feaa-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7feaa-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7feaa-117">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7feaa-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7feaa-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7feaa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7feaa-119">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7feaa-119">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7feaa-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7feaa-120">Application</span></span> | <span data-ttu-id="7feaa-121">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7feaa-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7feaa-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7feaa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7feaa-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7feaa-123">Optional query parameters</span></span>
<span data-ttu-id="7feaa-124">无。</span><span class="sxs-lookup"><span data-stu-id="7feaa-124">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7feaa-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7feaa-125">Request headers</span></span>
| <span data-ttu-id="7feaa-126">名称</span><span class="sxs-lookup"><span data-stu-id="7feaa-126">Name</span></span>       | <span data-ttu-id="7feaa-127">类型</span><span class="sxs-lookup"><span data-stu-id="7feaa-127">Type</span></span> | <span data-ttu-id="7feaa-128">说明</span><span class="sxs-lookup"><span data-stu-id="7feaa-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7feaa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7feaa-129">Authorization</span></span>  | <span data-ttu-id="7feaa-130">string</span><span class="sxs-lookup"><span data-stu-id="7feaa-130">string</span></span>  | <span data-ttu-id="7feaa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7feaa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7feaa-133">接受</span><span class="sxs-lookup"><span data-stu-id="7feaa-133">Accept</span></span> | <span data-ttu-id="7feaa-134">string</span><span class="sxs-lookup"><span data-stu-id="7feaa-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7feaa-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="7feaa-135">Request body</span></span>
<span data-ttu-id="7feaa-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7feaa-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7feaa-137">响应</span><span class="sxs-lookup"><span data-stu-id="7feaa-137">Response</span></span>

<span data-ttu-id="7feaa-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [onenoteOperation](../resources/onenoteoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7feaa-138">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7feaa-139">示例</span><span class="sxs-lookup"><span data-stu-id="7feaa-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7feaa-140">请求</span><span class="sxs-lookup"><span data-stu-id="7feaa-140">Request</span></span>
<span data-ttu-id="7feaa-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7feaa-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7feaa-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7feaa-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="7feaa-143">C#</span><span class="sxs-lookup"><span data-stu-id="7feaa-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7feaa-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7feaa-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7feaa-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7feaa-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7feaa-146">Java</span><span class="sxs-lookup"><span data-stu-id="7feaa-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onenoteoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7feaa-147">响应</span><span class="sxs-lookup"><span data-stu-id="7feaa-147">Response</span></span>
<span data-ttu-id="7feaa-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7feaa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


