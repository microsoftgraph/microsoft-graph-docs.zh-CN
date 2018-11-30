---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
ms.openlocfilehash: 62e03d7bee58f14acc5d5ace12d55f95d1d07a2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043341"
---
# <a name="update-organization"></a><span data-ttu-id="9e2e4-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="9e2e4-103">Update organization</span></span>

> <span data-ttu-id="9e2e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e2e4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e2e4-106">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-106">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e2e4-107">权限</span><span class="sxs-lookup"><span data-stu-id="9e2e4-107">Permissions</span></span>
<span data-ttu-id="9e2e4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e2e4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e2e4-110">Permission type</span></span> | <span data-ttu-id="9e2e4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e2e4-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e2e4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e2e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e2e4-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e2e4-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9e2e4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e2e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e2e4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-115">Not supported.</span></span> |
|<span data-ttu-id="9e2e4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e2e4-116">Application</span></span> | <span data-ttu-id="9e2e4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e2e4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e2e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="9e2e4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e2e4-119">Request headers</span></span>
| <span data-ttu-id="9e2e4-120">名称</span><span class="sxs-lookup"><span data-stu-id="9e2e4-120">Name</span></span>       | <span data-ttu-id="9e2e4-121">类型</span><span class="sxs-lookup"><span data-stu-id="9e2e4-121">Type</span></span> | <span data-ttu-id="9e2e4-122">说明</span><span class="sxs-lookup"><span data-stu-id="9e2e4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9e2e4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e2e4-123">Authorization</span></span>  | <span data-ttu-id="9e2e4-124">string</span><span class="sxs-lookup"><span data-stu-id="9e2e4-124">string</span></span>  | <span data-ttu-id="9e2e4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e2e4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e2e4-127">Request body</span></span>
<span data-ttu-id="9e2e4-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9e2e4-131">属性</span><span class="sxs-lookup"><span data-stu-id="9e2e4-131">Property</span></span>     | <span data-ttu-id="9e2e4-132">类型</span><span class="sxs-lookup"><span data-stu-id="9e2e4-132">Type</span></span>   |<span data-ttu-id="9e2e4-133">说明</span><span class="sxs-lookup"><span data-stu-id="9e2e4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e2e4-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="9e2e4-134">marketingNotificationEmails</span></span>|<span data-ttu-id="9e2e4-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e2e4-135">String collection</span></span>|                                        <span data-ttu-id="9e2e4-136">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="9e2e4-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9e2e4-137">privacyProfile</span></span>|[<span data-ttu-id="9e2e4-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9e2e4-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="9e2e4-139">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="9e2e4-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="9e2e4-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="9e2e4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9e2e4-141">String collection</span></span>||
|<span data-ttu-id="9e2e4-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="9e2e4-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="9e2e4-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e2e4-143">String collection</span></span>||
|<span data-ttu-id="9e2e4-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="9e2e4-144">technicalNotificationMails</span></span>|<span data-ttu-id="9e2e4-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e2e4-145">String collection</span></span>|                                        <span data-ttu-id="9e2e4-146">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="9e2e4-147">由于**组织**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**组织**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="9e2e4-148">响应</span><span class="sxs-lookup"><span data-stu-id="9e2e4-148">Response</span></span>

<span data-ttu-id="9e2e4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e2e4-151">示例</span><span class="sxs-lookup"><span data-stu-id="9e2e4-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e2e4-152">请求</span><span class="sxs-lookup"><span data-stu-id="9e2e4-152">Request</span></span>
<span data-ttu-id="9e2e4-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->
```http
PATCH https://graph.microsoft.com/beta/organization
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
##### <a name="response"></a><span data-ttu-id="9e2e4-154">响应</span><span class="sxs-lookup"><span data-stu-id="9e2e4-154">Response</span></span>
<span data-ttu-id="9e2e4-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9e2e4-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="9e2e4-156">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9e2e4-156">See also</span></span>

- [<span data-ttu-id="9e2e4-157">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="9e2e4-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9e2e4-158">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="9e2e4-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
