---
title: 停止 accessReview
description: 在 Azure AD 中访问审阅功能，停止当前的活动 accessReview。  目标对象可以是一次性访问回顾或定期访问评审的实例。  （若要防止定期访问回顾启动以后实例，更新其以更改其安排的结束日期）。  后访问查看停止，审阅者不再可以授予输入，以及可以应用访问审阅决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 070f91faa411fcc6d98db419d1683a7fb6493859
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521836"
---
# <a name="stop-accessreview"></a><span data-ttu-id="5cf06-106">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="5cf06-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf06-107">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，停止当前的活动[accessReview](../resources/accessreview.md)。</span><span class="sxs-lookup"><span data-stu-id="5cf06-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="5cf06-108">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="5cf06-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="5cf06-109">（要阻止定期访问回顾启动以后实例，[对其进行更新](accessreview-update.md)，以更改其安排的结束日期）。</span><span class="sxs-lookup"><span data-stu-id="5cf06-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="5cf06-110">后访问查看停止，审阅者不再可以授予输入，以及可以应用访问审阅决策。</span><span class="sxs-lookup"><span data-stu-id="5cf06-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="5cf06-111">权限</span><span class="sxs-lookup"><span data-stu-id="5cf06-111">Permissions</span></span>
<span data-ttu-id="5cf06-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cf06-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cf06-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cf06-114">Permission type</span></span>                        | <span data-ttu-id="5cf06-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cf06-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cf06-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cf06-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cf06-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cf06-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="5cf06-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cf06-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cf06-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cf06-119">Not supported.</span></span> |
|<span data-ttu-id="5cf06-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cf06-120">Application</span></span>                            | <span data-ttu-id="5cf06-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cf06-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cf06-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cf06-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="5cf06-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cf06-123">Request headers</span></span>
| <span data-ttu-id="5cf06-124">名称</span><span class="sxs-lookup"><span data-stu-id="5cf06-124">Name</span></span>         | <span data-ttu-id="5cf06-125">类型</span><span class="sxs-lookup"><span data-stu-id="5cf06-125">Type</span></span>        | <span data-ttu-id="5cf06-126">说明</span><span class="sxs-lookup"><span data-stu-id="5cf06-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5cf06-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cf06-127">Authorization</span></span> | <span data-ttu-id="5cf06-128">string</span><span class="sxs-lookup"><span data-stu-id="5cf06-128">string</span></span> | <span data-ttu-id="5cf06-129">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="5cf06-129">Bearer \{token\}.</span></span> <span data-ttu-id="5cf06-130">必需。</span><span class="sxs-lookup"><span data-stu-id="5cf06-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cf06-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cf06-131">Request body</span></span>
<span data-ttu-id="5cf06-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5cf06-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5cf06-133">响应</span><span class="sxs-lookup"><span data-stu-id="5cf06-133">Response</span></span>
<span data-ttu-id="5cf06-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5cf06-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cf06-136">示例</span><span class="sxs-lookup"><span data-stu-id="5cf06-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cf06-137">请求</span><span class="sxs-lookup"><span data-stu-id="5cf06-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="5cf06-138">响应</span><span class="sxs-lookup"><span data-stu-id="5cf06-138">Response</span></span>
><span data-ttu-id="5cf06-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5cf06-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
