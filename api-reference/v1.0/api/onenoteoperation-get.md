---
title: 获取 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。 这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: accbed7c935b0b624ab921031b96aea2690211e2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274436"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="e1306-104">获取 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="e1306-104">Get onenoteOperation</span></span>

<span data-ttu-id="e1306-105">获取长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e1306-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="e1306-106">这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`</span><span class="sxs-lookup"><span data-stu-id="e1306-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="e1306-107">您可以轮询操作-位置终结点, 直到`status`属性返回`completed`或`failed`。</span><span class="sxs-lookup"><span data-stu-id="e1306-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="e1306-108">如果状态为`completed`, 则`resourceLocation`属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="e1306-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="e1306-109">如果状态为`failed`, 则错误和`@api.diagnostics`属性将提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="e1306-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1306-110">权限</span><span class="sxs-lookup"><span data-stu-id="e1306-110">Permissions</span></span>
<span data-ttu-id="e1306-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1306-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1306-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1306-113">Permission type</span></span>      | <span data-ttu-id="e1306-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1306-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1306-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1306-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e1306-116">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1306-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1306-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1306-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1306-118">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1306-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e1306-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1306-119">Application</span></span> | <span data-ttu-id="e1306-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1306-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1306-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1306-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e1306-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1306-122">Optional query parameters</span></span>
<span data-ttu-id="e1306-123">无。</span><span class="sxs-lookup"><span data-stu-id="e1306-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1306-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1306-124">Request headers</span></span>
| <span data-ttu-id="e1306-125">名称</span><span class="sxs-lookup"><span data-stu-id="e1306-125">Name</span></span>       | <span data-ttu-id="e1306-126">类型</span><span class="sxs-lookup"><span data-stu-id="e1306-126">Type</span></span> | <span data-ttu-id="e1306-127">说明</span><span class="sxs-lookup"><span data-stu-id="e1306-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e1306-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1306-128">Authorization</span></span>  | <span data-ttu-id="e1306-129">string</span><span class="sxs-lookup"><span data-stu-id="e1306-129">string</span></span>  | <span data-ttu-id="e1306-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1306-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1306-132">接受</span><span class="sxs-lookup"><span data-stu-id="e1306-132">Accept</span></span> | <span data-ttu-id="e1306-133">string</span><span class="sxs-lookup"><span data-stu-id="e1306-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e1306-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1306-134">Request body</span></span>
<span data-ttu-id="e1306-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1306-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1306-136">响应</span><span class="sxs-lookup"><span data-stu-id="e1306-136">Response</span></span>

<span data-ttu-id="e1306-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenoteOperation](../resources/onenoteoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1306-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1306-138">示例</span><span class="sxs-lookup"><span data-stu-id="e1306-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1306-139">请求</span><span class="sxs-lookup"><span data-stu-id="e1306-139">Request</span></span>
<span data-ttu-id="e1306-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1306-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="e1306-141">响应</span><span class="sxs-lookup"><span data-stu-id="e1306-141">Response</span></span>
<span data-ttu-id="e1306-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1306-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1306-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e1306-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1306-146">C#</span><span class="sxs-lookup"><span data-stu-id="e1306-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_onenoteoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1306-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1306-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_onenoteoperation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1306-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="e1306-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_onenoteoperation-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/onenoteoperation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/onenoteoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/onenoteoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
