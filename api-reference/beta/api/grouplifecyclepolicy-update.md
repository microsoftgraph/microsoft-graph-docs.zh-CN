---
title: 更新 groupLifecyclePolicy
description: 更新 groupLifecyclePolicy 资源类型对象的属性。
author: dkershaw10
ms.openlocfilehash: 6977bb53a1b885ee65f110238727d4db0c212391
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303617"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="aaf8c-103">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aaf8c-103">Update groupLifecyclePolicy</span></span>

> <span data-ttu-id="aaf8c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaf8c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aaf8c-106">更新 [groupLifecyclePolicy 资源类型](../resources/grouplifecyclepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-106">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaf8c-107">权限</span><span class="sxs-lookup"><span data-stu-id="aaf8c-107">Permissions</span></span>

<span data-ttu-id="aaf8c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="aaf8c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaf8c-110">Permission type</span></span>      | <span data-ttu-id="aaf8c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aaf8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaf8c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf8c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aaf8c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf8c-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="aaf8c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf8c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaf8c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="aaf8c-115">Not supported</span></span> |
|<span data-ttu-id="aaf8c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaf8c-116">Application</span></span> | <span data-ttu-id="aaf8c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf8c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaf8c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaf8c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="aaf8c-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="aaf8c-119">Optional request headers</span></span>
| <span data-ttu-id="aaf8c-120">Name</span><span class="sxs-lookup"><span data-stu-id="aaf8c-120">Name</span></span> | <span data-ttu-id="aaf8c-121">说明</span><span class="sxs-lookup"><span data-stu-id="aaf8c-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="aaf8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf8c-122">Authorization</span></span> | <span data-ttu-id="aaf8c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aaf8c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aaf8c-125">Content-Type</span></span>  | <span data-ttu-id="aaf8c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaf8c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aaf8c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaf8c-127">Request body</span></span>

<span data-ttu-id="aaf8c-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aaf8c-131">属性</span><span class="sxs-lookup"><span data-stu-id="aaf8c-131">Property</span></span> | <span data-ttu-id="aaf8c-132">类型</span><span class="sxs-lookup"><span data-stu-id="aaf8c-132">Type</span></span> | <span data-ttu-id="aaf8c-133">说明</span><span class="sxs-lookup"><span data-stu-id="aaf8c-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aaf8c-134">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="aaf8c-134">alternateNotificationEmails</span></span>|<span data-ttu-id="aaf8c-135">String</span><span class="sxs-lookup"><span data-stu-id="aaf8c-135">String</span></span>| <span data-ttu-id="aaf8c-136">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-136">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="aaf8c-137">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-137">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="aaf8c-138">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="aaf8c-138">groupLifetimeInDays</span></span>|<span data-ttu-id="aaf8c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf8c-139">Int32</span></span>| <span data-ttu-id="aaf8c-140">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-140">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="aaf8c-141">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-141">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="aaf8c-142">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="aaf8c-142">managedGroupTypes</span></span>|<span data-ttu-id="aaf8c-143">String</span><span class="sxs-lookup"><span data-stu-id="aaf8c-143">String</span></span>| <span data-ttu-id="aaf8c-144">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-144">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="aaf8c-145">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-145">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="aaf8c-146">响应</span><span class="sxs-lookup"><span data-stu-id="aaf8c-146">Response</span></span>

<span data-ttu-id="aaf8c-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-147">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aaf8c-148">示例</span><span class="sxs-lookup"><span data-stu-id="aaf8c-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aaf8c-149">请求</span><span class="sxs-lookup"><span data-stu-id="aaf8c-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="aaf8c-150">响应</span><span class="sxs-lookup"><span data-stu-id="aaf8c-150">Response</span></span>
<span data-ttu-id="aaf8c-151">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aaf8c-151">Note: The response object shown here may be truncated for brevity.</span></span> 
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