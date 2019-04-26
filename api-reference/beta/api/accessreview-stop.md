---
title: 停止 accessReview
description: 在 "Azure AD access 评论" 功能中, 停止当前处于活动状态的 accessReview。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  (若要防止定期访问审核启动以后的实例, 请更新它以更改计划的结束日期)。  在访问审核停止后, 审阅者无法再提供输入, 并且可以应用访问审核决定。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 190d5a22c0ccc0920861d1a87064f846fada6914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322997"
---
# <a name="stop-accessreview"></a><span data-ttu-id="c7c71-106">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="c7c71-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7c71-107">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 停止当前处于活动状态的[accessReview](../resources/accessreview.md)。</span><span class="sxs-lookup"><span data-stu-id="c7c71-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="c7c71-108">目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="c7c71-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="c7c71-109">(若要防止定期访问审核启动以后的实例, 请[更新它](accessreview-update.md)以更改计划的结束日期)。</span><span class="sxs-lookup"><span data-stu-id="c7c71-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="c7c71-110">在访问审核停止后, 审阅者无法再提供输入, 并且可以应用访问审核决定。</span><span class="sxs-lookup"><span data-stu-id="c7c71-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7c71-111">权限</span><span class="sxs-lookup"><span data-stu-id="c7c71-111">Permissions</span></span>
<span data-ttu-id="c7c71-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7c71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c71-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7c71-114">Permission type</span></span>                        | <span data-ttu-id="c7c71-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7c71-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c71-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c71-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7c71-117">AccessReview</span><span class="sxs-lookup"><span data-stu-id="c7c71-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c7c71-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7c71-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c71-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c71-119">Not supported.</span></span> |
|<span data-ttu-id="c7c71-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7c71-120">Application</span></span>                            | <span data-ttu-id="c7c71-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7c71-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c7c71-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7c71-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="c7c71-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7c71-123">Request headers</span></span>
| <span data-ttu-id="c7c71-124">名称</span><span class="sxs-lookup"><span data-stu-id="c7c71-124">Name</span></span>         | <span data-ttu-id="c7c71-125">类型</span><span class="sxs-lookup"><span data-stu-id="c7c71-125">Type</span></span>        | <span data-ttu-id="c7c71-126">说明</span><span class="sxs-lookup"><span data-stu-id="c7c71-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c7c71-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c71-127">Authorization</span></span> | <span data-ttu-id="c7c71-128">string</span><span class="sxs-lookup"><span data-stu-id="c7c71-128">string</span></span> | <span data-ttu-id="c7c71-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7c71-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7c71-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7c71-131">Request body</span></span>
<span data-ttu-id="c7c71-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7c71-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c7c71-133">响应</span><span class="sxs-lookup"><span data-stu-id="c7c71-133">Response</span></span>
<span data-ttu-id="c7c71-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c7c71-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c71-136">示例</span><span class="sxs-lookup"><span data-stu-id="c7c71-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7c71-137">请求</span><span class="sxs-lookup"><span data-stu-id="c7c71-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
##### <a name="response"></a><span data-ttu-id="c7c71-138">响应</span><span class="sxs-lookup"><span data-stu-id="c7c71-138">Response</span></span>
><span data-ttu-id="c7c71-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7c71-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
