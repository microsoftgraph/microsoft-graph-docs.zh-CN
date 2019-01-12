---
title: 重置 accessReview
description: 在 Azure AD 访问评论功能中，重置当前处于活动状态 accessReview 的决策。  目标对象可以是一次性访问回顾或定期访问评审的实例。  以前的决策就不再记录，但审阅者可以继续更新决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b1f107733543380dbd6ad095133f09befc03736
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941490"
---
# <a name="reset-accessreview"></a><span data-ttu-id="ea71e-105">重置 accessReview</span><span class="sxs-lookup"><span data-stu-id="ea71e-105">Reset accessReview</span></span>

> <span data-ttu-id="ea71e-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea71e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea71e-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea71e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea71e-108">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，重置当前处于活动状态[accessReview](../resources/accessreview.md)的决策。</span><span class="sxs-lookup"><span data-stu-id="ea71e-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="ea71e-109">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="ea71e-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="ea71e-110">以前的决策就不再记录，但审阅者可以继续更新决策。</span><span class="sxs-lookup"><span data-stu-id="ea71e-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea71e-111">权限</span><span class="sxs-lookup"><span data-stu-id="ea71e-111">Permissions</span></span>
<span data-ttu-id="ea71e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea71e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea71e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea71e-114">Permission type</span></span>                        | <span data-ttu-id="ea71e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea71e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea71e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea71e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea71e-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea71e-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ea71e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea71e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea71e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea71e-119">Not supported.</span></span> |
|<span data-ttu-id="ea71e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea71e-120">Application</span></span>                            | <span data-ttu-id="ea71e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea71e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea71e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea71e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="ea71e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea71e-123">Request headers</span></span>
| <span data-ttu-id="ea71e-124">名称</span><span class="sxs-lookup"><span data-stu-id="ea71e-124">Name</span></span>         | <span data-ttu-id="ea71e-125">类型</span><span class="sxs-lookup"><span data-stu-id="ea71e-125">Type</span></span>        | <span data-ttu-id="ea71e-126">说明</span><span class="sxs-lookup"><span data-stu-id="ea71e-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ea71e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea71e-127">Authorization</span></span> | <span data-ttu-id="ea71e-128">string</span><span class="sxs-lookup"><span data-stu-id="ea71e-128">string</span></span> | <span data-ttu-id="ea71e-129">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="ea71e-129">Bearer \{token\}.</span></span> <span data-ttu-id="ea71e-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ea71e-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea71e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea71e-131">Request body</span></span>
<span data-ttu-id="ea71e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea71e-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ea71e-133">响应</span><span class="sxs-lookup"><span data-stu-id="ea71e-133">Response</span></span>
<span data-ttu-id="ea71e-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ea71e-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea71e-136">示例</span><span class="sxs-lookup"><span data-stu-id="ea71e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea71e-137">请求</span><span class="sxs-lookup"><span data-stu-id="ea71e-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="ea71e-138">响应</span><span class="sxs-lookup"><span data-stu-id="ea71e-138">Response</span></span>
><span data-ttu-id="ea71e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ea71e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
