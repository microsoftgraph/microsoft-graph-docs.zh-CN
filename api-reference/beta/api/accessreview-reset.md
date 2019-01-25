---
title: 重置 accessReview
description: 在 Azure AD 访问评论功能中，重置当前处于活动状态 accessReview 的决策。  目标对象可以是一次性访问回顾或定期访问评审的实例。  以前的决策就不再记录，但审阅者可以继续更新决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e258a781707d2c3fe5419e3ebd5f7c6b43f271b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517013"
---
# <a name="reset-accessreview"></a><span data-ttu-id="6f804-105">重置 accessReview</span><span class="sxs-lookup"><span data-stu-id="6f804-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f804-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，重置当前处于活动状态[accessReview](../resources/accessreview.md)的决策。</span><span class="sxs-lookup"><span data-stu-id="6f804-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="6f804-107">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="6f804-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="6f804-108">以前的决策就不再记录，但审阅者可以继续更新决策。</span><span class="sxs-lookup"><span data-stu-id="6f804-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f804-109">权限</span><span class="sxs-lookup"><span data-stu-id="6f804-109">Permissions</span></span>
<span data-ttu-id="6f804-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f804-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f804-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f804-112">Permission type</span></span>                        | <span data-ttu-id="6f804-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f804-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f804-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f804-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f804-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f804-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="6f804-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f804-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f804-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f804-117">Not supported.</span></span> |
|<span data-ttu-id="6f804-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f804-118">Application</span></span>                            | <span data-ttu-id="6f804-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f804-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f804-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f804-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="6f804-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f804-121">Request headers</span></span>
| <span data-ttu-id="6f804-122">名称</span><span class="sxs-lookup"><span data-stu-id="6f804-122">Name</span></span>         | <span data-ttu-id="6f804-123">类型</span><span class="sxs-lookup"><span data-stu-id="6f804-123">Type</span></span>        | <span data-ttu-id="6f804-124">说明</span><span class="sxs-lookup"><span data-stu-id="6f804-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6f804-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f804-125">Authorization</span></span> | <span data-ttu-id="6f804-126">string</span><span class="sxs-lookup"><span data-stu-id="6f804-126">string</span></span> | <span data-ttu-id="6f804-127">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="6f804-127">Bearer \{token\}.</span></span> <span data-ttu-id="6f804-128">必需。</span><span class="sxs-lookup"><span data-stu-id="6f804-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f804-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f804-129">Request body</span></span>
<span data-ttu-id="6f804-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f804-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6f804-131">响应</span><span class="sxs-lookup"><span data-stu-id="6f804-131">Response</span></span>
<span data-ttu-id="6f804-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6f804-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f804-134">示例</span><span class="sxs-lookup"><span data-stu-id="6f804-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f804-135">请求</span><span class="sxs-lookup"><span data-stu-id="6f804-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="6f804-136">响应</span><span class="sxs-lookup"><span data-stu-id="6f804-136">Response</span></span>
><span data-ttu-id="6f804-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f804-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
