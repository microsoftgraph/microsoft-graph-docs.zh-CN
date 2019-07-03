---
title: 获取 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。 这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ae44a94114c7ed85633393bfc1a9014116ed32ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457595"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="baf9d-104">获取 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="baf9d-104">Get onenoteOperation</span></span>

<span data-ttu-id="baf9d-105">获取长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="baf9d-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="baf9d-106">这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`</span><span class="sxs-lookup"><span data-stu-id="baf9d-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="baf9d-107">您可以轮询操作-位置终结点, 直到`status`属性返回`completed`或`failed`。</span><span class="sxs-lookup"><span data-stu-id="baf9d-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="baf9d-108">如果状态为`completed`, 则`resourceLocation`属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="baf9d-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="baf9d-109">如果状态为`failed`, 则错误和`@api.diagnostics`属性将提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="baf9d-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="baf9d-110">权限</span><span class="sxs-lookup"><span data-stu-id="baf9d-110">Permissions</span></span>
<span data-ttu-id="baf9d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baf9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baf9d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="baf9d-113">Permission type</span></span>      | <span data-ttu-id="baf9d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baf9d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baf9d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baf9d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="baf9d-116">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf9d-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="baf9d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baf9d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf9d-118">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="baf9d-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="baf9d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="baf9d-119">Application</span></span> | <span data-ttu-id="baf9d-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf9d-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="baf9d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baf9d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="baf9d-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="baf9d-122">Optional query parameters</span></span>
<span data-ttu-id="baf9d-123">无。</span><span class="sxs-lookup"><span data-stu-id="baf9d-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="baf9d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="baf9d-124">Request headers</span></span>
| <span data-ttu-id="baf9d-125">名称</span><span class="sxs-lookup"><span data-stu-id="baf9d-125">Name</span></span>       | <span data-ttu-id="baf9d-126">类型</span><span class="sxs-lookup"><span data-stu-id="baf9d-126">Type</span></span> | <span data-ttu-id="baf9d-127">说明</span><span class="sxs-lookup"><span data-stu-id="baf9d-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="baf9d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="baf9d-128">Authorization</span></span>  | <span data-ttu-id="baf9d-129">string</span><span class="sxs-lookup"><span data-stu-id="baf9d-129">string</span></span>  | <span data-ttu-id="baf9d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="baf9d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="baf9d-132">接受</span><span class="sxs-lookup"><span data-stu-id="baf9d-132">Accept</span></span> | <span data-ttu-id="baf9d-133">string</span><span class="sxs-lookup"><span data-stu-id="baf9d-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="baf9d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="baf9d-134">Request body</span></span>
<span data-ttu-id="baf9d-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="baf9d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baf9d-136">响应</span><span class="sxs-lookup"><span data-stu-id="baf9d-136">Response</span></span>

<span data-ttu-id="baf9d-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenoteOperation](../resources/onenoteoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="baf9d-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="baf9d-138">示例</span><span class="sxs-lookup"><span data-stu-id="baf9d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baf9d-139">请求</span><span class="sxs-lookup"><span data-stu-id="baf9d-139">Request</span></span>
<span data-ttu-id="baf9d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="baf9d-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="baf9d-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="baf9d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="baf9d-142">C#</span><span class="sxs-lookup"><span data-stu-id="baf9d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="baf9d-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="baf9d-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="baf9d-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="baf9d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="baf9d-145">响应</span><span class="sxs-lookup"><span data-stu-id="baf9d-145">Response</span></span>
<span data-ttu-id="baf9d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="baf9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
