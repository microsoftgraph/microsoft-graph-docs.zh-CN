---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 08a7a2173208fbeaecd1b76b9b75f1e7678a1103
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265882"
---
# <a name="update-organization"></a><span data-ttu-id="22c30-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="22c30-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22c30-104">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="22c30-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="22c30-105">在这种情况`organization`下, 将定义为恰好一个记录的集合, 因此必须在请求中指定其**ID** 。</span><span class="sxs-lookup"><span data-stu-id="22c30-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="22c30-106">该**ID**也称为组织的**tenantId** 。</span><span class="sxs-lookup"><span data-stu-id="22c30-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="22c30-107">权限</span><span class="sxs-lookup"><span data-stu-id="22c30-107">Permissions</span></span>

<span data-ttu-id="22c30-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22c30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22c30-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22c30-110">Permission type</span></span> | <span data-ttu-id="22c30-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22c30-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22c30-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22c30-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22c30-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22c30-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="22c30-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22c30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22c30-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="22c30-115">Not supported.</span></span> |
|<span data-ttu-id="22c30-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22c30-116">Application</span></span> | <span data-ttu-id="22c30-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22c30-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22c30-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22c30-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="22c30-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="22c30-119">Request headers</span></span>

| <span data-ttu-id="22c30-120">名称</span><span class="sxs-lookup"><span data-stu-id="22c30-120">Name</span></span>       | <span data-ttu-id="22c30-121">类型</span><span class="sxs-lookup"><span data-stu-id="22c30-121">Type</span></span> | <span data-ttu-id="22c30-122">说明</span><span class="sxs-lookup"><span data-stu-id="22c30-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="22c30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22c30-123">Authorization</span></span>  | <span data-ttu-id="22c30-124">string</span><span class="sxs-lookup"><span data-stu-id="22c30-124">string</span></span>  | <span data-ttu-id="22c30-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22c30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22c30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22c30-127">Request body</span></span>

<span data-ttu-id="22c30-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="22c30-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="22c30-131">属性</span><span class="sxs-lookup"><span data-stu-id="22c30-131">Property</span></span>     | <span data-ttu-id="22c30-132">类型</span><span class="sxs-lookup"><span data-stu-id="22c30-132">Type</span></span>   |<span data-ttu-id="22c30-133">说明</span><span class="sxs-lookup"><span data-stu-id="22c30-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22c30-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="22c30-134">marketingNotificationEmails</span></span>|<span data-ttu-id="22c30-135">String collection</span><span class="sxs-lookup"><span data-stu-id="22c30-135">String collection</span></span>|                                        <span data-ttu-id="22c30-136">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="22c30-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="22c30-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="22c30-137">privacyProfile</span></span>|[<span data-ttu-id="22c30-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="22c30-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="22c30-139">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="22c30-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="22c30-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="22c30-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="22c30-141">String collection</span><span class="sxs-lookup"><span data-stu-id="22c30-141">String collection</span></span>||
|<span data-ttu-id="22c30-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="22c30-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="22c30-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="22c30-143">String collection</span></span>||
|<span data-ttu-id="22c30-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="22c30-144">technicalNotificationMails</span></span>|<span data-ttu-id="22c30-145">String collection</span><span class="sxs-lookup"><span data-stu-id="22c30-145">String collection</span></span>|                                        <span data-ttu-id="22c30-146">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="22c30-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="22c30-147">由于**组织**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**组织**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="22c30-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="22c30-148">响应</span><span class="sxs-lookup"><span data-stu-id="22c30-148">Response</span></span>

<span data-ttu-id="22c30-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="22c30-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22c30-151">示例</span><span class="sxs-lookup"><span data-stu-id="22c30-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22c30-152">请求</span><span class="sxs-lookup"><span data-stu-id="22c30-152">Request</span></span>
<span data-ttu-id="22c30-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22c30-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
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

##### <a name="response"></a><span data-ttu-id="22c30-154">响应</span><span class="sxs-lookup"><span data-stu-id="22c30-154">Response</span></span>

<span data-ttu-id="22c30-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="22c30-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="22c30-156">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="22c30-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="22c30-157">C#</span><span class="sxs-lookup"><span data-stu-id="22c30-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22c30-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="22c30-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="22c30-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="22c30-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="22c30-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="22c30-160">See also</span></span>

- [<span data-ttu-id="22c30-161">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="22c30-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="22c30-162">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="22c30-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
