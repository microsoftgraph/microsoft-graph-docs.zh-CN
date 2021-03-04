---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d137f9e519247c61a1b38d547c15f0eb3e68b859
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447873"
---
# <a name="update-organization"></a><span data-ttu-id="76aa7-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="76aa7-103">Update organization</span></span>

<span data-ttu-id="76aa7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76aa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76aa7-105">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="76aa7-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="76aa7-106">在这种情况下，定义为只包含一条记录的集合，因此必须在 `organization` 请求中指定其 **ID。**</span><span class="sxs-lookup"><span data-stu-id="76aa7-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="76aa7-107">**ID** 也称为组织的 **tenantId。**</span><span class="sxs-lookup"><span data-stu-id="76aa7-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="76aa7-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="76aa7-108">Permissions</span></span>

<span data-ttu-id="76aa7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76aa7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76aa7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76aa7-111">Permission type</span></span> | <span data-ttu-id="76aa7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76aa7-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76aa7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76aa7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="76aa7-114">Organization.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76aa7-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="76aa7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76aa7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76aa7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76aa7-116">Not supported.</span></span> |
|<span data-ttu-id="76aa7-117">Application</span><span class="sxs-lookup"><span data-stu-id="76aa7-117">Application</span></span> | <span data-ttu-id="76aa7-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76aa7-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76aa7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76aa7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76aa7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="76aa7-120">Request headers</span></span>

| <span data-ttu-id="76aa7-121">名称</span><span class="sxs-lookup"><span data-stu-id="76aa7-121">Name</span></span>       | <span data-ttu-id="76aa7-122">说明</span><span class="sxs-lookup"><span data-stu-id="76aa7-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="76aa7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76aa7-123">Authorization</span></span>  | <span data-ttu-id="76aa7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76aa7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76aa7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76aa7-126">Content-Type</span></span>   | <span data-ttu-id="76aa7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="76aa7-127">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="76aa7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="76aa7-128">Request body</span></span>

<span data-ttu-id="76aa7-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="76aa7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76aa7-132">属性</span><span class="sxs-lookup"><span data-stu-id="76aa7-132">Property</span></span>  | <span data-ttu-id="76aa7-133">类型</span><span class="sxs-lookup"><span data-stu-id="76aa7-133">Type</span></span> |<span data-ttu-id="76aa7-134">说明</span><span class="sxs-lookup"><span data-stu-id="76aa7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76aa7-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="76aa7-135">marketingNotificationEmails</span></span>|<span data-ttu-id="76aa7-136">String collection</span><span class="sxs-lookup"><span data-stu-id="76aa7-136">String collection</span></span>|                                        <span data-ttu-id="76aa7-137">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="76aa7-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="76aa7-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="76aa7-138">privacyProfile</span></span>|[<span data-ttu-id="76aa7-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="76aa7-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="76aa7-140">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="76aa7-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="76aa7-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="76aa7-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="76aa7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="76aa7-142">String collection</span></span>||
|<span data-ttu-id="76aa7-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="76aa7-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="76aa7-144">String collection</span><span class="sxs-lookup"><span data-stu-id="76aa7-144">String collection</span></span>||
|<span data-ttu-id="76aa7-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="76aa7-145">technicalNotificationMails</span></span>|<span data-ttu-id="76aa7-146">String collection</span><span class="sxs-lookup"><span data-stu-id="76aa7-146">String collection</span></span>|                                        <span data-ttu-id="76aa7-147">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="76aa7-147">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="76aa7-148">由于 **组织** 资源 [支持](/graph/extensibility-overview)扩展，因此可以使用该操作在现有组织实例的扩展的自定义属性中添加、更新或删除你自己的特定于 `PATCH` 应用的数据。</span><span class="sxs-lookup"><span data-stu-id="76aa7-148">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="76aa7-149">响应</span><span class="sxs-lookup"><span data-stu-id="76aa7-149">Response</span></span>

<span data-ttu-id="76aa7-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="76aa7-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76aa7-152">示例</span><span class="sxs-lookup"><span data-stu-id="76aa7-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76aa7-153">请求</span><span class="sxs-lookup"><span data-stu-id="76aa7-153">Request</span></span>
<span data-ttu-id="76aa7-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76aa7-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76aa7-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="76aa7-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="76aa7-156">C#</span><span class="sxs-lookup"><span data-stu-id="76aa7-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76aa7-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76aa7-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76aa7-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76aa7-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76aa7-159">Java</span><span class="sxs-lookup"><span data-stu-id="76aa7-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="76aa7-160">响应</span><span class="sxs-lookup"><span data-stu-id="76aa7-160">Response</span></span>

<span data-ttu-id="76aa7-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="76aa7-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="76aa7-162">另请参阅</span><span class="sxs-lookup"><span data-stu-id="76aa7-162">See also</span></span>

- [<span data-ttu-id="76aa7-163">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="76aa7-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="76aa7-164">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="76aa7-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
  ]
}
-->


