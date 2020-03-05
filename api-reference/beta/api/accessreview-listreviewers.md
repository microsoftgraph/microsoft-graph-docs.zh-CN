---
title: 列出 accessReview 审阅者
description: 在 "Azure AD access 评论" 功能中，检索 accessReview 对象的审阅者。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 114a59e0d5e96983a30afcf31d8452c979f2f486
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441877"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="713f7-103">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="713f7-103">List accessReview reviewers</span></span>

<span data-ttu-id="713f7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="713f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="713f7-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，检索[accessReview](../resources/accessreview.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="713f7-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="713f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="713f7-106">Permissions</span></span>
<span data-ttu-id="713f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="713f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="713f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="713f7-109">Permission type</span></span>                        | <span data-ttu-id="713f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="713f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="713f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="713f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="713f7-112">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="713f7-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="713f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="713f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="713f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="713f7-114">Not supported.</span></span> |
|<span data-ttu-id="713f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="713f7-115">Application</span></span>                            | <span data-ttu-id="713f7-116">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="713f7-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="713f7-117">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="713f7-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="713f7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="713f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="713f7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="713f7-119">Request headers</span></span>
| <span data-ttu-id="713f7-120">名称</span><span class="sxs-lookup"><span data-stu-id="713f7-120">Name</span></span>         | <span data-ttu-id="713f7-121">类型</span><span class="sxs-lookup"><span data-stu-id="713f7-121">Type</span></span>        | <span data-ttu-id="713f7-122">说明</span><span class="sxs-lookup"><span data-stu-id="713f7-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="713f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="713f7-123">Authorization</span></span> | <span data-ttu-id="713f7-124">string</span><span class="sxs-lookup"><span data-stu-id="713f7-124">string</span></span> | <span data-ttu-id="713f7-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="713f7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="713f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="713f7-127">Request body</span></span>
<span data-ttu-id="713f7-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="713f7-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="713f7-129">响应</span><span class="sxs-lookup"><span data-stu-id="713f7-129">Response</span></span>
<span data-ttu-id="713f7-130">如果成功，此方法在响应`200, OK`正文中返回响应代码和[userIdentity](../resources/useridentity.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="713f7-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="713f7-131">示例</span><span class="sxs-lookup"><span data-stu-id="713f7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="713f7-132">请求</span><span class="sxs-lookup"><span data-stu-id="713f7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="713f7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="713f7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="713f7-134">C#</span><span class="sxs-lookup"><span data-stu-id="713f7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="713f7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="713f7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="713f7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="713f7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="713f7-137">响应</span><span class="sxs-lookup"><span data-stu-id="713f7-137">Response</span></span>
><span data-ttu-id="713f7-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="713f7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":
    [
        {
            "id":"006111db-0810-4494-a6df-904d368bd81b"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="713f7-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="713f7-140">See also</span></span>

| <span data-ttu-id="713f7-141">方法</span><span class="sxs-lookup"><span data-stu-id="713f7-141">Method</span></span>           | <span data-ttu-id="713f7-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="713f7-142">Return Type</span></span>    |<span data-ttu-id="713f7-143">说明</span><span class="sxs-lookup"><span data-stu-id="713f7-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="713f7-144">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="713f7-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="713f7-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="713f7-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="713f7-146">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="713f7-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="713f7-147">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="713f7-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="713f7-148">无。</span><span class="sxs-lookup"><span data-stu-id="713f7-148">None.</span></span>   |   <span data-ttu-id="713f7-149">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="713f7-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="713f7-150">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="713f7-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="713f7-151">无。</span><span class="sxs-lookup"><span data-stu-id="713f7-151">None.</span></span> |   <span data-ttu-id="713f7-152">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="713f7-152">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
