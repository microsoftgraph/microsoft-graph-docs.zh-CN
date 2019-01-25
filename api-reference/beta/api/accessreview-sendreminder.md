---
title: SendReminder accessReview
description: '在 Azure AD 中访问审阅功能，向审阅者的当前活动 accessReview 发送提醒。  目标对象可以是一次性访问回顾或定期访问评审的实例。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db394036a228f405a8cebb783a9279779054b04d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518546"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="eb06b-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="eb06b-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb06b-105">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，将发送给审阅者的当前活动[accessReview](../resources/accessreview.md)的提醒。</span><span class="sxs-lookup"><span data-stu-id="eb06b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="eb06b-106">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="eb06b-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="eb06b-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb06b-107">Permissions</span></span>
<span data-ttu-id="eb06b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb06b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb06b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb06b-110">Permission type</span></span>                        | <span data-ttu-id="eb06b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb06b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb06b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb06b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb06b-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb06b-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="eb06b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb06b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb06b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb06b-115">Not supported.</span></span> |
|<span data-ttu-id="eb06b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb06b-116">Application</span></span>                            | <span data-ttu-id="eb06b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb06b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb06b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb06b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="eb06b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb06b-119">Request headers</span></span>
| <span data-ttu-id="eb06b-120">名称</span><span class="sxs-lookup"><span data-stu-id="eb06b-120">Name</span></span>         | <span data-ttu-id="eb06b-121">类型</span><span class="sxs-lookup"><span data-stu-id="eb06b-121">Type</span></span>        | <span data-ttu-id="eb06b-122">说明</span><span class="sxs-lookup"><span data-stu-id="eb06b-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eb06b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb06b-123">Authorization</span></span> | <span data-ttu-id="eb06b-124">string</span><span class="sxs-lookup"><span data-stu-id="eb06b-124">string</span></span> | <span data-ttu-id="eb06b-125">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="eb06b-125">Bearer \{token\}.</span></span> <span data-ttu-id="eb06b-126">必需。</span><span class="sxs-lookup"><span data-stu-id="eb06b-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb06b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb06b-127">Request body</span></span>
<span data-ttu-id="eb06b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb06b-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="eb06b-129">响应</span><span class="sxs-lookup"><span data-stu-id="eb06b-129">Response</span></span>
<span data-ttu-id="eb06b-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb06b-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb06b-132">示例</span><span class="sxs-lookup"><span data-stu-id="eb06b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb06b-133">请求</span><span class="sxs-lookup"><span data-stu-id="eb06b-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/sendReminder()
```
##### <a name="response"></a><span data-ttu-id="eb06b-134">响应</span><span class="sxs-lookup"><span data-stu-id="eb06b-134">Response</span></span>
><span data-ttu-id="eb06b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb06b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
