---
title: SendReminder accessReview
description: '在 Azure AD 中访问审阅功能，向审阅者的当前活动 accessReview 发送提醒。  目标对象可以是一次性访问回顾或定期访问评审的实例。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cf5b78d2c67993fbf2da9be7c55a07fb752985c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917277"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="4d176-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="4d176-104">SendReminder accessReview</span></span>

> <span data-ttu-id="4d176-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4d176-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d176-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4d176-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d176-107">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，将发送给审阅者的当前活动[accessReview](../resources/accessreview.md)的提醒。</span><span class="sxs-lookup"><span data-stu-id="4d176-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="4d176-108">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="4d176-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4d176-109">权限</span><span class="sxs-lookup"><span data-stu-id="4d176-109">Permissions</span></span>
<span data-ttu-id="4d176-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d176-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d176-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d176-112">Permission type</span></span>                        | <span data-ttu-id="4d176-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d176-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d176-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d176-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d176-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d176-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4d176-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d176-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d176-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d176-117">Not supported.</span></span> |
|<span data-ttu-id="4d176-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d176-118">Application</span></span>                            | <span data-ttu-id="4d176-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d176-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d176-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d176-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="4d176-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d176-121">Request headers</span></span>
| <span data-ttu-id="4d176-122">名称</span><span class="sxs-lookup"><span data-stu-id="4d176-122">Name</span></span>         | <span data-ttu-id="4d176-123">类型</span><span class="sxs-lookup"><span data-stu-id="4d176-123">Type</span></span>        | <span data-ttu-id="4d176-124">说明</span><span class="sxs-lookup"><span data-stu-id="4d176-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4d176-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d176-125">Authorization</span></span> | <span data-ttu-id="4d176-126">string</span><span class="sxs-lookup"><span data-stu-id="4d176-126">string</span></span> | <span data-ttu-id="4d176-127">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="4d176-127">Bearer \{token\}.</span></span> <span data-ttu-id="4d176-128">必填。</span><span class="sxs-lookup"><span data-stu-id="4d176-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d176-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d176-129">Request body</span></span>
<span data-ttu-id="4d176-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d176-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4d176-131">响应</span><span class="sxs-lookup"><span data-stu-id="4d176-131">Response</span></span>
<span data-ttu-id="4d176-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4d176-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d176-134">示例</span><span class="sxs-lookup"><span data-stu-id="4d176-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d176-135">请求</span><span class="sxs-lookup"><span data-stu-id="4d176-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="4d176-136">响应</span><span class="sxs-lookup"><span data-stu-id="4d176-136">Response</span></span>
><span data-ttu-id="4d176-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4d176-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
