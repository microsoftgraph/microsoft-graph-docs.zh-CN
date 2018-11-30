---
title: 停止 accessReview
description: 在 Azure AD 中访问审阅功能，停止当前的活动 accessReview。  目标对象可以是一次性访问回顾或定期访问评审的实例。  （若要防止定期访问回顾启动以后实例，更新其以更改其安排的结束日期）。  后访问查看停止，审阅者不再可以授予输入，以及可以应用访问审阅决策。
ms.openlocfilehash: 2a4ac5d13f3be70cc5a4a24f4051429c473e7690
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044296"
---
# <a name="stop-accessreview"></a><span data-ttu-id="88f8a-106">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="88f8a-106">Stop accessReview</span></span>

> <span data-ttu-id="88f8a-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88f8a-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88f8a-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88f8a-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88f8a-109">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，停止当前的活动[accessReview](../resources/accessreview.md)。</span><span class="sxs-lookup"><span data-stu-id="88f8a-109">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="88f8a-110">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="88f8a-110">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="88f8a-111">（要阻止定期访问回顾启动以后实例，[对其进行更新](accessreview-update.md)，以更改其安排的结束日期）。</span><span class="sxs-lookup"><span data-stu-id="88f8a-111">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="88f8a-112">后访问查看停止，审阅者不再可以授予输入，以及可以应用访问审阅决策。</span><span class="sxs-lookup"><span data-stu-id="88f8a-112">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="88f8a-113">权限</span><span class="sxs-lookup"><span data-stu-id="88f8a-113">Permissions</span></span>
<span data-ttu-id="88f8a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88f8a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88f8a-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="88f8a-116">Permission type</span></span>                        | <span data-ttu-id="88f8a-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88f8a-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="88f8a-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88f8a-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="88f8a-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f8a-119">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="88f8a-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88f8a-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88f8a-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="88f8a-121">Not supported.</span></span> |
|<span data-ttu-id="88f8a-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="88f8a-122">Application</span></span>                            | <span data-ttu-id="88f8a-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="88f8a-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88f8a-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88f8a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="88f8a-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="88f8a-125">Request headers</span></span>
| <span data-ttu-id="88f8a-126">名称</span><span class="sxs-lookup"><span data-stu-id="88f8a-126">Name</span></span>         | <span data-ttu-id="88f8a-127">类型</span><span class="sxs-lookup"><span data-stu-id="88f8a-127">Type</span></span>        | <span data-ttu-id="88f8a-128">说明</span><span class="sxs-lookup"><span data-stu-id="88f8a-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="88f8a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="88f8a-129">Authorization</span></span> | <span data-ttu-id="88f8a-130">string</span><span class="sxs-lookup"><span data-stu-id="88f8a-130">string</span></span> | <span data-ttu-id="88f8a-131">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="88f8a-131">Bearer \{token\}.</span></span> <span data-ttu-id="88f8a-132">必需。</span><span class="sxs-lookup"><span data-stu-id="88f8a-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88f8a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="88f8a-133">Request body</span></span>
<span data-ttu-id="88f8a-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88f8a-134">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="88f8a-135">响应</span><span class="sxs-lookup"><span data-stu-id="88f8a-135">Response</span></span>
<span data-ttu-id="88f8a-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="88f8a-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f8a-138">示例</span><span class="sxs-lookup"><span data-stu-id="88f8a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88f8a-139">请求</span><span class="sxs-lookup"><span data-stu-id="88f8a-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="88f8a-140">响应</span><span class="sxs-lookup"><span data-stu-id="88f8a-140">Response</span></span>
><span data-ttu-id="88f8a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88f8a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
