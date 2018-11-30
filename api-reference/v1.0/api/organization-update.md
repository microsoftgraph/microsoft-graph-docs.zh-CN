---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
ms.openlocfilehash: ac07f3ded31f8d6c7169d24208ed7e8cf967e07a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010805"
---
# <a name="update-organization"></a><span data-ttu-id="9f3cf-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="9f3cf-103">Update organization</span></span>

<span data-ttu-id="9f3cf-104">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-104">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f3cf-105">权限</span><span class="sxs-lookup"><span data-stu-id="9f3cf-105">Permissions</span></span>

<span data-ttu-id="9f3cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f3cf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f3cf-108">Permission type</span></span> | <span data-ttu-id="9f3cf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f3cf-109">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f3cf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f3cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f3cf-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f3cf-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f3cf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f3cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f3cf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-113">Not supported.</span></span>    |
|<span data-ttu-id="9f3cf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f3cf-114">Application</span></span> | <span data-ttu-id="9f3cf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f3cf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f3cf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="9f3cf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f3cf-117">Request headers</span></span>

| <span data-ttu-id="9f3cf-118">名称</span><span class="sxs-lookup"><span data-stu-id="9f3cf-118">Name</span></span>       | <span data-ttu-id="9f3cf-119">类型</span><span class="sxs-lookup"><span data-stu-id="9f3cf-119">Type</span></span> | <span data-ttu-id="9f3cf-120">说明</span><span class="sxs-lookup"><span data-stu-id="9f3cf-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9f3cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f3cf-121">Authorization</span></span>  | <span data-ttu-id="9f3cf-122">string</span><span class="sxs-lookup"><span data-stu-id="9f3cf-122">string</span></span>  | <span data-ttu-id="9f3cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f3cf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f3cf-125">Request body</span></span>
<span data-ttu-id="9f3cf-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9f3cf-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9f3cf-128">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-128">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f3cf-129">属性</span><span class="sxs-lookup"><span data-stu-id="9f3cf-129">Property</span></span>     | <span data-ttu-id="9f3cf-130">类型</span><span class="sxs-lookup"><span data-stu-id="9f3cf-130">Type</span></span>   |<span data-ttu-id="9f3cf-131">说明</span><span class="sxs-lookup"><span data-stu-id="9f3cf-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f3cf-132">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="9f3cf-132">marketingNotificationEmails</span></span>|<span data-ttu-id="9f3cf-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f3cf-133">String collection</span></span>|                                        <span data-ttu-id="9f3cf-134">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-134">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="9f3cf-135">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9f3cf-135">privacyProfile</span></span>|[<span data-ttu-id="9f3cf-136">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9f3cf-136">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="9f3cf-137">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-137">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="9f3cf-138">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="9f3cf-138">securityComplianceNotificationMails</span></span>|<span data-ttu-id="9f3cf-139">String collection</span><span class="sxs-lookup"><span data-stu-id="9f3cf-139">String collection</span></span>||
|<span data-ttu-id="9f3cf-140">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="9f3cf-140">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="9f3cf-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f3cf-141">String collection</span></span>||
|<span data-ttu-id="9f3cf-142">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="9f3cf-142">technicalNotificationMails</span></span>|<span data-ttu-id="9f3cf-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f3cf-143">String collection</span></span>|                                        <span data-ttu-id="9f3cf-144">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-144">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="9f3cf-145">响应</span><span class="sxs-lookup"><span data-stu-id="9f3cf-145">Response</span></span>

<span data-ttu-id="9f3cf-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9f3cf-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f3cf-147">示例</span><span class="sxs-lookup"><span data-stu-id="9f3cf-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f3cf-148">请求</span><span class="sxs-lookup"><span data-stu-id="9f3cf-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
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

### <a name="response"></a><span data-ttu-id="9f3cf-149">响应</span><span class="sxs-lookup"><span data-stu-id="9f3cf-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
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
  "tocPath": ""
}-->
