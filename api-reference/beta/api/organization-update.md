---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32a522b3ed8a21189f60ef68ce6990c2a7e78938
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346623"
---
# <a name="update-organization"></a><span data-ttu-id="5e83d-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="5e83d-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e83d-104">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="5e83d-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="5e83d-105">在这种情况`organization`下, 将定义为恰好一个记录的集合, 因此必须在请求中指定其**ID** 。</span><span class="sxs-lookup"><span data-stu-id="5e83d-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="5e83d-106">该**ID**也称为组织的**tenantId** 。</span><span class="sxs-lookup"><span data-stu-id="5e83d-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e83d-107">权限</span><span class="sxs-lookup"><span data-stu-id="5e83d-107">Permissions</span></span>

<span data-ttu-id="5e83d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e83d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e83d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e83d-110">Permission type</span></span> | <span data-ttu-id="5e83d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e83d-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e83d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e83d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e83d-113">Directory.accessasuser.all、All、All</span><span class="sxs-lookup"><span data-stu-id="5e83d-113">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5e83d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e83d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e83d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e83d-115">Not supported.</span></span> |
|<span data-ttu-id="5e83d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e83d-116">Application</span></span> | <span data-ttu-id="5e83d-117">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="5e83d-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e83d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e83d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e83d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e83d-119">Request headers</span></span>

| <span data-ttu-id="5e83d-120">名称</span><span class="sxs-lookup"><span data-stu-id="5e83d-120">Name</span></span>       | <span data-ttu-id="5e83d-121">说明</span><span class="sxs-lookup"><span data-stu-id="5e83d-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5e83d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e83d-122">Authorization</span></span>  | <span data-ttu-id="5e83d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e83d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e83d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e83d-125">Content-Type</span></span>   | <span data-ttu-id="5e83d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e83d-126">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="5e83d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e83d-127">Request body</span></span>

<span data-ttu-id="5e83d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5e83d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e83d-131">属性</span><span class="sxs-lookup"><span data-stu-id="5e83d-131">Property</span></span>  | <span data-ttu-id="5e83d-132">类型</span><span class="sxs-lookup"><span data-stu-id="5e83d-132">Type</span></span> |<span data-ttu-id="5e83d-133">说明</span><span class="sxs-lookup"><span data-stu-id="5e83d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e83d-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="5e83d-134">marketingNotificationEmails</span></span>|<span data-ttu-id="5e83d-135">String collection</span><span class="sxs-lookup"><span data-stu-id="5e83d-135">String collection</span></span>|                                        <span data-ttu-id="5e83d-136">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5e83d-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="5e83d-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5e83d-137">privacyProfile</span></span>|[<span data-ttu-id="5e83d-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5e83d-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="5e83d-139">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="5e83d-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="5e83d-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5e83d-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="5e83d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5e83d-141">String collection</span></span>||
|<span data-ttu-id="5e83d-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="5e83d-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="5e83d-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="5e83d-143">String collection</span></span>||
|<span data-ttu-id="5e83d-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5e83d-144">technicalNotificationMails</span></span>|<span data-ttu-id="5e83d-145">String collection</span><span class="sxs-lookup"><span data-stu-id="5e83d-145">String collection</span></span>|                                        <span data-ttu-id="5e83d-146">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5e83d-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="5e83d-147">由于**组织**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**组织**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="5e83d-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="5e83d-148">响应</span><span class="sxs-lookup"><span data-stu-id="5e83d-148">Response</span></span>

<span data-ttu-id="5e83d-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5e83d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e83d-151">示例</span><span class="sxs-lookup"><span data-stu-id="5e83d-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e83d-152">请求</span><span class="sxs-lookup"><span data-stu-id="5e83d-152">Request</span></span>
<span data-ttu-id="5e83d-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e83d-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5e83d-154">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5e83d-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e83d-155">C#</span><span class="sxs-lookup"><span data-stu-id="5e83d-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e83d-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e83d-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e83d-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="5e83d-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5e83d-158">Java</span><span class="sxs-lookup"><span data-stu-id="5e83d-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e83d-159">响应</span><span class="sxs-lookup"><span data-stu-id="5e83d-159">Response</span></span>

<span data-ttu-id="5e83d-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e83d-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5e83d-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5e83d-161">See also</span></span>

- [<span data-ttu-id="5e83d-162">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5e83d-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5e83d-163">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5e83d-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
