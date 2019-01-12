---
title: 列表 accessReview 审阅者
description: 在 Azure AD 中访问审阅功能，检索 accessReview 对象的审阅者。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8dca759f71f13af18c291f1af9843da6729ef701
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946810"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="86071-103">列表 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="86071-103">List accessReview reviewers</span></span>

> <span data-ttu-id="86071-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="86071-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86071-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86071-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86071-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="86071-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86071-107">权限</span><span class="sxs-lookup"><span data-stu-id="86071-107">Permissions</span></span>
<span data-ttu-id="86071-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86071-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86071-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86071-110">Permission type</span></span>                        | <span data-ttu-id="86071-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86071-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="86071-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86071-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="86071-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="86071-113"></span></span>  <span data-ttu-id="86071-114">登录的用户还必须在目录角色中允许他们阅读访问审阅。</span><span class="sxs-lookup"><span data-stu-id="86071-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="86071-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86071-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86071-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86071-116">Not supported.</span></span> |
|<span data-ttu-id="86071-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86071-117">Application</span></span>                            | <span data-ttu-id="86071-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="86071-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86071-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86071-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="86071-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86071-120">Request headers</span></span>
| <span data-ttu-id="86071-121">名称</span><span class="sxs-lookup"><span data-stu-id="86071-121">Name</span></span>         | <span data-ttu-id="86071-122">类型</span><span class="sxs-lookup"><span data-stu-id="86071-122">Type</span></span>        | <span data-ttu-id="86071-123">说明</span><span class="sxs-lookup"><span data-stu-id="86071-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="86071-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="86071-124">Authorization</span></span> | <span data-ttu-id="86071-125">string</span><span class="sxs-lookup"><span data-stu-id="86071-125">string</span></span> | <span data-ttu-id="86071-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="86071-126">Bearer \{token\}.</span></span> <span data-ttu-id="86071-127">必需。</span><span class="sxs-lookup"><span data-stu-id="86071-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86071-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="86071-128">Request body</span></span>
<span data-ttu-id="86071-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="86071-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="86071-130">响应</span><span class="sxs-lookup"><span data-stu-id="86071-130">Response</span></span>
<span data-ttu-id="86071-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[userIdentity](../resources/useridentity.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="86071-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86071-132">示例</span><span class="sxs-lookup"><span data-stu-id="86071-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86071-133">请求</span><span class="sxs-lookup"><span data-stu-id="86071-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="86071-134">响应</span><span class="sxs-lookup"><span data-stu-id="86071-134">Response</span></span>
><span data-ttu-id="86071-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86071-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "value":[
    {
       "id":"006111db-0810-4494-a6df-904d368bd81b"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="86071-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="86071-137">See also</span></span>

| <span data-ttu-id="86071-138">方法</span><span class="sxs-lookup"><span data-stu-id="86071-138">Method</span></span>           | <span data-ttu-id="86071-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="86071-139">Return Type</span></span>    |<span data-ttu-id="86071-140">说明</span><span class="sxs-lookup"><span data-stu-id="86071-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86071-141">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="86071-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="86071-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="86071-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="86071-143">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="86071-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="86071-144">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="86071-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="86071-145">无。</span><span class="sxs-lookup"><span data-stu-id="86071-145">None.</span></span>   |   <span data-ttu-id="86071-146">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="86071-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="86071-147">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="86071-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="86071-148">无。</span><span class="sxs-lookup"><span data-stu-id="86071-148">None.</span></span> |   <span data-ttu-id="86071-149">删除 accessReview 审阅者。</span><span class="sxs-lookup"><span data-stu-id="86071-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
