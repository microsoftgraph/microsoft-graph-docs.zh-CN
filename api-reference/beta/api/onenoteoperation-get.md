---
title: 获取 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。 这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 1404d406307b52f8ba0dfc507abe132c4d663f03
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267856"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="3dfba-104">获取 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="3dfba-104">Get onenoteOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dfba-105">获取长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3dfba-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="3dfba-106">这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`</span><span class="sxs-lookup"><span data-stu-id="3dfba-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="3dfba-107">您可以轮询操作-位置终结点, 直到`status`属性返回`completed`或`failed`。</span><span class="sxs-lookup"><span data-stu-id="3dfba-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="3dfba-108">如果状态为`completed`, 则`resourceLocation`属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="3dfba-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="3dfba-109">如果状态为`failed`, 则错误和`@api.diagnostics`属性将提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="3dfba-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dfba-110">权限</span><span class="sxs-lookup"><span data-stu-id="3dfba-110">Permissions</span></span>
<span data-ttu-id="3dfba-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dfba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dfba-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dfba-113">Permission type</span></span>      | <span data-ttu-id="3dfba-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dfba-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dfba-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfba-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3dfba-116">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfba-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dfba-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfba-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dfba-118">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3dfba-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3dfba-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dfba-119">Application</span></span> | <span data-ttu-id="3dfba-120">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfba-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dfba-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dfba-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3dfba-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3dfba-122">Optional query parameters</span></span>
<span data-ttu-id="3dfba-123">无。</span><span class="sxs-lookup"><span data-stu-id="3dfba-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dfba-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dfba-124">Request headers</span></span>
| <span data-ttu-id="3dfba-125">名称</span><span class="sxs-lookup"><span data-stu-id="3dfba-125">Name</span></span>       | <span data-ttu-id="3dfba-126">类型</span><span class="sxs-lookup"><span data-stu-id="3dfba-126">Type</span></span> | <span data-ttu-id="3dfba-127">说明</span><span class="sxs-lookup"><span data-stu-id="3dfba-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3dfba-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dfba-128">Authorization</span></span>  | <span data-ttu-id="3dfba-129">string</span><span class="sxs-lookup"><span data-stu-id="3dfba-129">string</span></span>  | <span data-ttu-id="3dfba-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dfba-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3dfba-132">接受</span><span class="sxs-lookup"><span data-stu-id="3dfba-132">Accept</span></span> | <span data-ttu-id="3dfba-133">string</span><span class="sxs-lookup"><span data-stu-id="3dfba-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3dfba-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dfba-134">Request body</span></span>
<span data-ttu-id="3dfba-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3dfba-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dfba-136">响应</span><span class="sxs-lookup"><span data-stu-id="3dfba-136">Response</span></span>

<span data-ttu-id="3dfba-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenoteOperation](../resources/onenoteoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3dfba-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3dfba-138">示例</span><span class="sxs-lookup"><span data-stu-id="3dfba-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3dfba-139">请求</span><span class="sxs-lookup"><span data-stu-id="3dfba-139">Request</span></span>
<span data-ttu-id="3dfba-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dfba-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="3dfba-141">响应</span><span class="sxs-lookup"><span data-stu-id="3dfba-141">Response</span></span>
<span data-ttu-id="3dfba-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3dfba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3dfba-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3dfba-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3dfba-146">C#</span><span class="sxs-lookup"><span data-stu-id="3dfba-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_onenoteoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3dfba-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="3dfba-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_onenoteoperation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3dfba-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="3dfba-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_onenoteoperation-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/onenoteoperation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/onenoteoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/onenoteoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
