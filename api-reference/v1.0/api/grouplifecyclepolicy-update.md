---
title: 更新 groupLifecyclePolicy
description: 更新 groupLifecyclePolicy 资源类型对象的属性。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0c198d637f23522ad1fd6a93a19a09ee4d1a6ab6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014583"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="b0655-103">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b0655-103">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="b0655-104">更新 [groupLifecyclePolicy 资源类型](../resources/grouplifecyclepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0655-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0655-105">权限</span><span class="sxs-lookup"><span data-stu-id="b0655-105">Permissions</span></span>

<span data-ttu-id="b0655-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 
|<span data-ttu-id="b0655-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0655-108">Permission type</span></span>      | <span data-ttu-id="b0655-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0655-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0655-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0655-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0655-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0655-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0655-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0655-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0655-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0655-113">Not supported.</span></span>    |
|<span data-ttu-id="b0655-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0655-114">Application</span></span> | <span data-ttu-id="b0655-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0655-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0655-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0655-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b0655-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b0655-117">Optional request headers</span></span>
| <span data-ttu-id="b0655-118">名称</span><span class="sxs-lookup"><span data-stu-id="b0655-118">Name</span></span> | <span data-ttu-id="b0655-119">说明</span><span class="sxs-lookup"><span data-stu-id="b0655-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="b0655-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0655-120">Authorization</span></span> | <span data-ttu-id="b0655-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0655-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0655-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0655-123">Content-Type</span></span>  | <span data-ttu-id="b0655-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0655-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b0655-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0655-125">Request body</span></span>

<span data-ttu-id="b0655-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b0655-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b0655-127">未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b0655-127">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="b0655-128">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="b0655-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b0655-129">属性</span><span class="sxs-lookup"><span data-stu-id="b0655-129">Property</span></span> | <span data-ttu-id="b0655-130">类型</span><span class="sxs-lookup"><span data-stu-id="b0655-130">Type</span></span> | <span data-ttu-id="b0655-131">说明</span><span class="sxs-lookup"><span data-stu-id="b0655-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b0655-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="b0655-132">alternateNotificationEmails</span></span>|<span data-ttu-id="b0655-133">String</span><span class="sxs-lookup"><span data-stu-id="b0655-133">String</span></span>| <span data-ttu-id="b0655-134">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="b0655-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="b0655-135">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b0655-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="b0655-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="b0655-136">groupLifetimeInDays</span></span>|<span data-ttu-id="b0655-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b0655-137">Int32</span></span>| <span data-ttu-id="b0655-138">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="b0655-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="b0655-139">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="b0655-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="b0655-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="b0655-140">managedGroupTypes</span></span>|<span data-ttu-id="b0655-141">String</span><span class="sxs-lookup"><span data-stu-id="b0655-141">String</span></span>| <span data-ttu-id="b0655-142">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="b0655-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="b0655-143">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="b0655-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="b0655-144">响应</span><span class="sxs-lookup"><span data-stu-id="b0655-144">Response</span></span>

<span data-ttu-id="b0655-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0655-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0655-146">示例</span><span class="sxs-lookup"><span data-stu-id="b0655-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0655-147">请求</span><span class="sxs-lookup"><span data-stu-id="b0655-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b0655-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b0655-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0655-149">C#</span><span class="sxs-lookup"><span data-stu-id="b0655-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0655-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0655-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0655-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="b0655-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0655-152">Java</span><span class="sxs-lookup"><span data-stu-id="b0655-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0655-153">响应</span><span class="sxs-lookup"><span data-stu-id="b0655-153">Response</span></span>
<span data-ttu-id="b0655-154">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b0655-154">Note: The response object shown here may be truncated for brevity.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
