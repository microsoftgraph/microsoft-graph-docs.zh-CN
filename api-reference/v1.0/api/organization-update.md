---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 41f8dd22d5d1327e4f8b65ab037dc9c46fa91d12
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274380"
---
# <a name="update-organization"></a><span data-ttu-id="07182-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="07182-103">Update organization</span></span>

<span data-ttu-id="07182-104">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="07182-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="07182-105">在这种情况`organization`下, 将定义为恰好一个记录的集合, 因此必须在请求中指定其**ID** 。</span><span class="sxs-lookup"><span data-stu-id="07182-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="07182-106">该**ID**也称为组织的**tenantId** 。</span><span class="sxs-lookup"><span data-stu-id="07182-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="07182-107">权限</span><span class="sxs-lookup"><span data-stu-id="07182-107">Permissions</span></span>

<span data-ttu-id="07182-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07182-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07182-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="07182-110">Permission type</span></span> | <span data-ttu-id="07182-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07182-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07182-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07182-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07182-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07182-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07182-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07182-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07182-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="07182-115">Not supported.</span></span>    |
|<span data-ttu-id="07182-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="07182-116">Application</span></span> | <span data-ttu-id="07182-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="07182-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07182-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07182-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="07182-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="07182-119">Request headers</span></span>

| <span data-ttu-id="07182-120">名称</span><span class="sxs-lookup"><span data-stu-id="07182-120">Name</span></span>       | <span data-ttu-id="07182-121">类型</span><span class="sxs-lookup"><span data-stu-id="07182-121">Type</span></span> | <span data-ttu-id="07182-122">说明</span><span class="sxs-lookup"><span data-stu-id="07182-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07182-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07182-123">Authorization</span></span>  | <span data-ttu-id="07182-124">string</span><span class="sxs-lookup"><span data-stu-id="07182-124">string</span></span>  | <span data-ttu-id="07182-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07182-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07182-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="07182-127">Request body</span></span>

<span data-ttu-id="07182-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="07182-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="07182-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="07182-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07182-130">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="07182-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07182-131">属性</span><span class="sxs-lookup"><span data-stu-id="07182-131">Property</span></span>     | <span data-ttu-id="07182-132">类型</span><span class="sxs-lookup"><span data-stu-id="07182-132">Type</span></span>   |<span data-ttu-id="07182-133">说明</span><span class="sxs-lookup"><span data-stu-id="07182-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07182-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="07182-134">marketingNotificationEmails</span></span>|<span data-ttu-id="07182-135">String collection</span><span class="sxs-lookup"><span data-stu-id="07182-135">String collection</span></span>|                                        <span data-ttu-id="07182-136">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="07182-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="07182-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="07182-137">privacyProfile</span></span>|[<span data-ttu-id="07182-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="07182-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="07182-139">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="07182-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="07182-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="07182-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="07182-141">String collection</span><span class="sxs-lookup"><span data-stu-id="07182-141">String collection</span></span>||
|<span data-ttu-id="07182-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="07182-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="07182-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="07182-143">String collection</span></span>||
|<span data-ttu-id="07182-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="07182-144">technicalNotificationMails</span></span>|<span data-ttu-id="07182-145">String collection</span><span class="sxs-lookup"><span data-stu-id="07182-145">String collection</span></span>|                                        <span data-ttu-id="07182-146">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="07182-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="07182-147">响应</span><span class="sxs-lookup"><span data-stu-id="07182-147">Response</span></span>

<span data-ttu-id="07182-148">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="07182-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07182-149">示例</span><span class="sxs-lookup"><span data-stu-id="07182-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="07182-150">请求</span><span class="sxs-lookup"><span data-stu-id="07182-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="07182-151">响应</span><span class="sxs-lookup"><span data-stu-id="07182-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="07182-152">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="07182-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07182-153">C#</span><span class="sxs-lookup"><span data-stu-id="07182-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07182-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="07182-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="07182-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="07182-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
