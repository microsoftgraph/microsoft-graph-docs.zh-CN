---
title: 更新 groupLifecyclePolicy
description: 更新 groupLifecyclePolicy 资源类型对象的属性。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 66b0d19ac4f1ae24ec76702ffb55542b363e43ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864867"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="113db-103">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="113db-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="113db-104">更新 [groupLifecyclePolicy 资源类型](../resources/grouplifecyclepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="113db-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="113db-105">权限</span><span class="sxs-lookup"><span data-stu-id="113db-105">Permissions</span></span>

<span data-ttu-id="113db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="113db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="113db-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="113db-108">Permission type</span></span>      | <span data-ttu-id="113db-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="113db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="113db-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="113db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="113db-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113db-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="113db-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="113db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113db-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="113db-113">Not supported.</span></span>    |
|<span data-ttu-id="113db-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="113db-114">Application</span></span> | <span data-ttu-id="113db-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113db-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="113db-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="113db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="113db-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="113db-117">Optional request headers</span></span>
| <span data-ttu-id="113db-118">名称</span><span class="sxs-lookup"><span data-stu-id="113db-118">Name</span></span> | <span data-ttu-id="113db-119">说明</span><span class="sxs-lookup"><span data-stu-id="113db-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="113db-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="113db-120">Authorization</span></span> | <span data-ttu-id="113db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="113db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="113db-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="113db-123">Content-Type</span></span>  | <span data-ttu-id="113db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="113db-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="113db-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="113db-125">Request body</span></span>

<span data-ttu-id="113db-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="113db-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="113db-127">未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="113db-127">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="113db-128">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="113db-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="113db-129">属性</span><span class="sxs-lookup"><span data-stu-id="113db-129">Property</span></span> | <span data-ttu-id="113db-130">类型</span><span class="sxs-lookup"><span data-stu-id="113db-130">Type</span></span> | <span data-ttu-id="113db-131">说明</span><span class="sxs-lookup"><span data-stu-id="113db-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="113db-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="113db-132">alternateNotificationEmails</span></span>|<span data-ttu-id="113db-133">String</span><span class="sxs-lookup"><span data-stu-id="113db-133">String</span></span>| <span data-ttu-id="113db-134">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="113db-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="113db-135">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="113db-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="113db-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="113db-136">groupLifetimeInDays</span></span>|<span data-ttu-id="113db-137">Int32</span><span class="sxs-lookup"><span data-stu-id="113db-137">Int32</span></span>| <span data-ttu-id="113db-138">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="113db-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="113db-139">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="113db-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="113db-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="113db-140">managedGroupTypes</span></span>|<span data-ttu-id="113db-141">String</span><span class="sxs-lookup"><span data-stu-id="113db-141">String</span></span>| <span data-ttu-id="113db-142">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="113db-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="113db-143">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="113db-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="113db-144">响应</span><span class="sxs-lookup"><span data-stu-id="113db-144">Response</span></span>

<span data-ttu-id="113db-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="113db-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="113db-146">示例</span><span class="sxs-lookup"><span data-stu-id="113db-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="113db-147">请求</span><span class="sxs-lookup"><span data-stu-id="113db-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="113db-148">响应</span><span class="sxs-lookup"><span data-stu-id="113db-148">Response</span></span>
<span data-ttu-id="113db-149">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="113db-149">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
