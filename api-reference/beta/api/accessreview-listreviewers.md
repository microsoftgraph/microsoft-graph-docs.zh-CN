---
title: 列出 accessReview 审阅者
description: 在 "Azure AD access 评论" 功能中, 检索 accessReview 对象的审阅者。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7be3d5ea922f8d2dca87dba005e62fd30fef3540
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323075"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="de19c-103">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="de19c-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de19c-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="de19c-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de19c-105">权限</span><span class="sxs-lookup"><span data-stu-id="de19c-105">Permissions</span></span>
<span data-ttu-id="de19c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de19c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de19c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="de19c-108">Permission type</span></span>                        | <span data-ttu-id="de19c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de19c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="de19c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de19c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de19c-111">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="de19c-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="de19c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de19c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de19c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="de19c-113">Not supported.</span></span> |
|<span data-ttu-id="de19c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="de19c-114">Application</span></span>                            | <span data-ttu-id="de19c-115">AccessReview</span><span class="sxs-lookup"><span data-stu-id="de19c-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="de19c-116">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="de19c-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="de19c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de19c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="de19c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="de19c-118">Request headers</span></span>
| <span data-ttu-id="de19c-119">名称</span><span class="sxs-lookup"><span data-stu-id="de19c-119">Name</span></span>         | <span data-ttu-id="de19c-120">类型</span><span class="sxs-lookup"><span data-stu-id="de19c-120">Type</span></span>        | <span data-ttu-id="de19c-121">说明</span><span class="sxs-lookup"><span data-stu-id="de19c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="de19c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de19c-122">Authorization</span></span> | <span data-ttu-id="de19c-123">string</span><span class="sxs-lookup"><span data-stu-id="de19c-123">string</span></span> | <span data-ttu-id="de19c-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="de19c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de19c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de19c-126">Request body</span></span>
<span data-ttu-id="de19c-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="de19c-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="de19c-128">响应</span><span class="sxs-lookup"><span data-stu-id="de19c-128">Response</span></span>
<span data-ttu-id="de19c-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[userIdentity](../resources/useridentity.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="de19c-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de19c-130">示例</span><span class="sxs-lookup"><span data-stu-id="de19c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de19c-131">请求</span><span class="sxs-lookup"><span data-stu-id="de19c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```

##### <a name="response"></a><span data-ttu-id="de19c-132">响应</span><span class="sxs-lookup"><span data-stu-id="de19c-132">Response</span></span>
><span data-ttu-id="de19c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="de19c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="de19c-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="de19c-135">See also</span></span>

| <span data-ttu-id="de19c-136">方法</span><span class="sxs-lookup"><span data-stu-id="de19c-136">Method</span></span>           | <span data-ttu-id="de19c-137">返回类型</span><span class="sxs-lookup"><span data-stu-id="de19c-137">Return Type</span></span>    |<span data-ttu-id="de19c-138">说明</span><span class="sxs-lookup"><span data-stu-id="de19c-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de19c-139">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="de19c-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="de19c-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="de19c-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="de19c-141">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="de19c-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="de19c-142">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="de19c-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="de19c-143">无。</span><span class="sxs-lookup"><span data-stu-id="de19c-143">None.</span></span>   |   <span data-ttu-id="de19c-144">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="de19c-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="de19c-145">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="de19c-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="de19c-146">无。</span><span class="sxs-lookup"><span data-stu-id="de19c-146">None.</span></span> |   <span data-ttu-id="de19c-147">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="de19c-147">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
