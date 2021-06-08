---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6e848342b2a14d836f2fc9c0df68db2f44e0531b
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787448"
---
# <a name="update-organization"></a><span data-ttu-id="f2c9b-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="f2c9b-103">Update organization</span></span>

<span data-ttu-id="f2c9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2c9b-105">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="f2c9b-106">在这种情况下，定义为只包含一条记录的集合，因此必须在请求中指定 `organization` 其 **ID。**</span><span class="sxs-lookup"><span data-stu-id="f2c9b-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="f2c9b-107">**ID** 也称为组织的 **tenantId。**</span><span class="sxs-lookup"><span data-stu-id="f2c9b-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c9b-108">权限</span><span class="sxs-lookup"><span data-stu-id="f2c9b-108">Permissions</span></span>

<span data-ttu-id="f2c9b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c9b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2c9b-111">Permission type</span></span> | <span data-ttu-id="f2c9b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2c9b-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c9b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c9b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f2c9b-114">Organization.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2c9b-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2c9b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c9b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2c9b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-116">Not supported.</span></span>    |
|<span data-ttu-id="f2c9b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2c9b-117">Application</span></span> | <span data-ttu-id="f2c9b-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c9b-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2c9b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2c9b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2c9b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2c9b-120">Request headers</span></span>

| <span data-ttu-id="f2c9b-121">名称</span><span class="sxs-lookup"><span data-stu-id="f2c9b-121">Name</span></span>       | <span data-ttu-id="f2c9b-122">说明</span><span class="sxs-lookup"><span data-stu-id="f2c9b-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="f2c9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2c9b-123">Authorization</span></span>  | <span data-ttu-id="f2c9b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2c9b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2c9b-126">Content-Type</span></span>   | <span data-ttu-id="f2c9b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f2c9b-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2c9b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2c9b-128">Request body</span></span>

<span data-ttu-id="f2c9b-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f2c9b-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f2c9b-131">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-131">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f2c9b-132">属性</span><span class="sxs-lookup"><span data-stu-id="f2c9b-132">Property</span></span>     | <span data-ttu-id="f2c9b-133">类型</span><span class="sxs-lookup"><span data-stu-id="f2c9b-133">Type</span></span>   |<span data-ttu-id="f2c9b-134">说明</span><span class="sxs-lookup"><span data-stu-id="f2c9b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2c9b-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f2c9b-135">marketingNotificationEmails</span></span>|<span data-ttu-id="f2c9b-136">String collection</span><span class="sxs-lookup"><span data-stu-id="f2c9b-136">String collection</span></span>|                                        <span data-ttu-id="f2c9b-137">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f2c9b-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f2c9b-138">privacyProfile</span></span>|[<span data-ttu-id="f2c9b-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f2c9b-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="f2c9b-140">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="f2c9b-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f2c9b-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="f2c9b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f2c9b-142">String collection</span></span>||
|<span data-ttu-id="f2c9b-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="f2c9b-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="f2c9b-144">String collection</span><span class="sxs-lookup"><span data-stu-id="f2c9b-144">String collection</span></span>||
|<span data-ttu-id="f2c9b-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f2c9b-145">technicalNotificationMails</span></span>|<span data-ttu-id="f2c9b-146">String collection</span><span class="sxs-lookup"><span data-stu-id="f2c9b-146">String collection</span></span>|                                        <span data-ttu-id="f2c9b-147">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-147">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="f2c9b-148">响应</span><span class="sxs-lookup"><span data-stu-id="f2c9b-148">Response</span></span>

<span data-ttu-id="f2c9b-149">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2c9b-149">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2c9b-150">示例</span><span class="sxs-lookup"><span data-stu-id="f2c9b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2c9b-151">请求</span><span class="sxs-lookup"><span data-stu-id="f2c9b-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f2c9b-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c9b-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f2c9b-153">C#</span><span class="sxs-lookup"><span data-stu-id="f2c9b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2c9b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2c9b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2c9b-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2c9b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2c9b-156">Java</span><span class="sxs-lookup"><span data-stu-id="f2c9b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2c9b-157">响应</span><span class="sxs-lookup"><span data-stu-id="f2c9b-157">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

