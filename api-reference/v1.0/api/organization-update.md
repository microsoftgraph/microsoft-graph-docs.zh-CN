---
title: 更新组织
description: 更新当前经过身份验证的组织的属性。
localization_priority: Normal
ms.openlocfilehash: 83b1514831e930e3eabe6e6a78203c44ec3b5b3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834956"
---
# <a name="update-organization"></a><span data-ttu-id="a4431-103">更新组织</span><span class="sxs-lookup"><span data-stu-id="a4431-103">Update organization</span></span>

<span data-ttu-id="a4431-104">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="a4431-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="a4431-105">在这种情况下，`organization`指一准确按照一条记录上，因此必须请求中指定其**ID** 。</span><span class="sxs-lookup"><span data-stu-id="a4431-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="a4431-106">**ID**是也称为组织**tenantId** 。</span><span class="sxs-lookup"><span data-stu-id="a4431-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="a4431-107">权限</span><span class="sxs-lookup"><span data-stu-id="a4431-107">Permissions</span></span>

<span data-ttu-id="a4431-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4431-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4431-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4431-110">Permission type</span></span> | <span data-ttu-id="a4431-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4431-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4431-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4431-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a4431-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4431-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4431-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4431-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4431-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4431-115">Not supported.</span></span>    |
|<span data-ttu-id="a4431-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4431-116">Application</span></span> | <span data-ttu-id="a4431-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4431-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4431-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4431-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="a4431-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4431-119">Request headers</span></span>

| <span data-ttu-id="a4431-120">名称</span><span class="sxs-lookup"><span data-stu-id="a4431-120">Name</span></span>       | <span data-ttu-id="a4431-121">类型</span><span class="sxs-lookup"><span data-stu-id="a4431-121">Type</span></span> | <span data-ttu-id="a4431-122">说明</span><span class="sxs-lookup"><span data-stu-id="a4431-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4431-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4431-123">Authorization</span></span>  | <span data-ttu-id="a4431-124">string</span><span class="sxs-lookup"><span data-stu-id="a4431-124">string</span></span>  | <span data-ttu-id="a4431-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4431-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4431-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4431-127">Request body</span></span>

<span data-ttu-id="a4431-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a4431-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a4431-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a4431-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a4431-130">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="a4431-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a4431-131">属性</span><span class="sxs-lookup"><span data-stu-id="a4431-131">Property</span></span>     | <span data-ttu-id="a4431-132">类型</span><span class="sxs-lookup"><span data-stu-id="a4431-132">Type</span></span>   |<span data-ttu-id="a4431-133">说明</span><span class="sxs-lookup"><span data-stu-id="a4431-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4431-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a4431-134">marketingNotificationEmails</span></span>|<span data-ttu-id="a4431-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="a4431-135">String collection</span></span>|                                        <span data-ttu-id="a4431-136">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="a4431-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="a4431-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="a4431-137">privacyProfile</span></span>|[<span data-ttu-id="a4431-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="a4431-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="a4431-139">组织的隐私配置文件（设置 statementUrl 和 contactEmail）。</span><span class="sxs-lookup"><span data-stu-id="a4431-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="a4431-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="a4431-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="a4431-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a4431-141">String collection</span></span>||
|<span data-ttu-id="a4431-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="a4431-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="a4431-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="a4431-143">String collection</span></span>||
|<span data-ttu-id="a4431-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="a4431-144">technicalNotificationMails</span></span>|<span data-ttu-id="a4431-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="a4431-145">String collection</span></span>|                                        <span data-ttu-id="a4431-146">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="a4431-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="a4431-147">响应</span><span class="sxs-lookup"><span data-stu-id="a4431-147">Response</span></span>

<span data-ttu-id="a4431-148">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4431-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4431-149">示例</span><span class="sxs-lookup"><span data-stu-id="a4431-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4431-150">请求</span><span class="sxs-lookup"><span data-stu-id="a4431-150">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="a4431-151">响应</span><span class="sxs-lookup"><span data-stu-id="a4431-151">Response</span></span>

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
