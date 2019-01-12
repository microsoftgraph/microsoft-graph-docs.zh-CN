---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 109c3f68e1eaa719f18a7fa8c539d09a2e3061aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969847"
---
# <a name="update-organization"></a><span data-ttu-id="5308c-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="5308c-103">Update organization</span></span>

<span data-ttu-id="5308c-104">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="5308c-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="5308c-105">在这种情况下，`organization`指一准确按照一条记录上，因此必须请求中指定其**ID** 。</span><span class="sxs-lookup"><span data-stu-id="5308c-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="5308c-106">**ID**是也称为组织**tenantId** 。</span><span class="sxs-lookup"><span data-stu-id="5308c-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="5308c-107">权限</span><span class="sxs-lookup"><span data-stu-id="5308c-107">Permissions</span></span>

<span data-ttu-id="5308c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5308c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5308c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5308c-110">Permission type</span></span> | <span data-ttu-id="5308c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5308c-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5308c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5308c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5308c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5308c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5308c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5308c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5308c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5308c-115">Not supported.</span></span>    |
|<span data-ttu-id="5308c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5308c-116">Application</span></span> | <span data-ttu-id="5308c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5308c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5308c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5308c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="5308c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5308c-119">Request headers</span></span>

| <span data-ttu-id="5308c-120">名称</span><span class="sxs-lookup"><span data-stu-id="5308c-120">Name</span></span>       | <span data-ttu-id="5308c-121">类型</span><span class="sxs-lookup"><span data-stu-id="5308c-121">Type</span></span> | <span data-ttu-id="5308c-122">说明</span><span class="sxs-lookup"><span data-stu-id="5308c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5308c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5308c-123">Authorization</span></span>  | <span data-ttu-id="5308c-124">string</span><span class="sxs-lookup"><span data-stu-id="5308c-124">string</span></span>  | <span data-ttu-id="5308c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5308c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5308c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5308c-127">Request body</span></span>

<span data-ttu-id="5308c-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5308c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5308c-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5308c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5308c-130">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="5308c-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5308c-131">属性</span><span class="sxs-lookup"><span data-stu-id="5308c-131">Property</span></span>     | <span data-ttu-id="5308c-132">类型</span><span class="sxs-lookup"><span data-stu-id="5308c-132">Type</span></span>   |<span data-ttu-id="5308c-133">说明</span><span class="sxs-lookup"><span data-stu-id="5308c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5308c-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="5308c-134">marketingNotificationEmails</span></span>|<span data-ttu-id="5308c-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="5308c-135">String collection</span></span>|                                        <span data-ttu-id="5308c-136">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5308c-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="5308c-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5308c-137">privacyProfile</span></span>|[<span data-ttu-id="5308c-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5308c-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="5308c-139">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="5308c-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="5308c-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5308c-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="5308c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5308c-141">String collection</span></span>||
|<span data-ttu-id="5308c-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="5308c-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="5308c-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="5308c-143">String collection</span></span>||
|<span data-ttu-id="5308c-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5308c-144">technicalNotificationMails</span></span>|<span data-ttu-id="5308c-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="5308c-145">String collection</span></span>|                                        <span data-ttu-id="5308c-146">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5308c-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="5308c-147">响应</span><span class="sxs-lookup"><span data-stu-id="5308c-147">Response</span></span>

<span data-ttu-id="5308c-148">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5308c-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5308c-149">示例</span><span class="sxs-lookup"><span data-stu-id="5308c-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5308c-150">请求</span><span class="sxs-lookup"><span data-stu-id="5308c-150">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="5308c-151">响应</span><span class="sxs-lookup"><span data-stu-id="5308c-151">Response</span></span>

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
