---
title: 列表 accessReview 审阅者
description: 在 Azure AD 中访问审阅功能，检索 accessReview 对象的审阅者。
localization_priority: Normal
ms.openlocfilehash: 042887944902be9a603ae0581835c8d55355f8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829370"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="5b679-103">列表 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="5b679-103">List accessReview reviewers</span></span>

> <span data-ttu-id="5b679-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b679-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b679-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b679-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b679-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="5b679-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b679-107">权限</span><span class="sxs-lookup"><span data-stu-id="5b679-107">Permissions</span></span>
<span data-ttu-id="5b679-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b679-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b679-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b679-110">Permission type</span></span>                        | <span data-ttu-id="5b679-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b679-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b679-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b679-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b679-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="5b679-113"></span></span>  <span data-ttu-id="5b679-114">登录的用户还必须在目录角色中允许他们阅读访问审阅。</span><span class="sxs-lookup"><span data-stu-id="5b679-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="5b679-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b679-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b679-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b679-116">Not supported.</span></span> |
|<span data-ttu-id="5b679-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b679-117">Application</span></span>                            | <span data-ttu-id="5b679-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b679-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b679-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b679-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="5b679-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b679-120">Request headers</span></span>
| <span data-ttu-id="5b679-121">名称</span><span class="sxs-lookup"><span data-stu-id="5b679-121">Name</span></span>         | <span data-ttu-id="5b679-122">类型</span><span class="sxs-lookup"><span data-stu-id="5b679-122">Type</span></span>        | <span data-ttu-id="5b679-123">说明</span><span class="sxs-lookup"><span data-stu-id="5b679-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5b679-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b679-124">Authorization</span></span> | <span data-ttu-id="5b679-125">string</span><span class="sxs-lookup"><span data-stu-id="5b679-125">string</span></span> | <span data-ttu-id="5b679-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="5b679-126">Bearer \{token\}.</span></span> <span data-ttu-id="5b679-127">必填。</span><span class="sxs-lookup"><span data-stu-id="5b679-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b679-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b679-128">Request body</span></span>
<span data-ttu-id="5b679-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b679-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="5b679-130">响应</span><span class="sxs-lookup"><span data-stu-id="5b679-130">Response</span></span>
<span data-ttu-id="5b679-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[userIdentity](../resources/useridentity.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="5b679-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b679-132">示例</span><span class="sxs-lookup"><span data-stu-id="5b679-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b679-133">请求</span><span class="sxs-lookup"><span data-stu-id="5b679-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="5b679-134">响应</span><span class="sxs-lookup"><span data-stu-id="5b679-134">Response</span></span>
><span data-ttu-id="5b679-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5b679-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5b679-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5b679-137">See also</span></span>

| <span data-ttu-id="5b679-138">方法</span><span class="sxs-lookup"><span data-stu-id="5b679-138">Method</span></span>           | <span data-ttu-id="5b679-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b679-139">Return Type</span></span>    |<span data-ttu-id="5b679-140">说明</span><span class="sxs-lookup"><span data-stu-id="5b679-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b679-141">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="5b679-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="5b679-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="5b679-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="5b679-143">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="5b679-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="5b679-144">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="5b679-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="5b679-145">无。</span><span class="sxs-lookup"><span data-stu-id="5b679-145">None.</span></span>   |   <span data-ttu-id="5b679-146">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="5b679-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="5b679-147">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="5b679-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="5b679-148">无。</span><span class="sxs-lookup"><span data-stu-id="5b679-148">None.</span></span> |   <span data-ttu-id="5b679-149">删除 accessReview 审阅者。</span><span class="sxs-lookup"><span data-stu-id="5b679-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
