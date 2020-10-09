---
title: 组： evaluateDynamicMembership
description: 评估用户或设备是否为动态组的成员。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: aad3e32cc1dd6936d0be221fe20225d56b386cb2
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403124"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="4ebef-103">组： evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="4ebef-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="4ebef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ebef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ebef-105">评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="4ebef-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="4ebef-106">成员身份规则与评估中使用的其他详细信息一起返回。</span><span class="sxs-lookup"><span data-stu-id="4ebef-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="4ebef-107">您可以通过以下方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="4ebef-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="4ebef-108">评估用户或设备是否为指定的动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="4ebef-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="4ebef-109">根据用户或设备的 ID 和成员身份规则评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="4ebef-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ebef-110">权限</span><span class="sxs-lookup"><span data-stu-id="4ebef-110">Permissions</span></span>

<span data-ttu-id="4ebef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ebef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="4ebef-113">使用成员 ID 和组 ID 评估动态成员身份</span><span class="sxs-lookup"><span data-stu-id="4ebef-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="4ebef-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ebef-114">Permission type</span></span> | <span data-ttu-id="4ebef-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ebef-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4ebef-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebef-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4ebef-117">对于 user： Group. All 和 Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="4ebef-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="4ebef-118">对于 device： Group. All 和 Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="4ebef-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="4ebef-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebef-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ebef-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebef-120">Not supported.</span></span> |
| <span data-ttu-id="4ebef-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ebef-121">Application</span></span>                            | <span data-ttu-id="4ebef-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebef-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="4ebef-123">使用成员 ID 和成员身份规则评估动态成员资格</span><span class="sxs-lookup"><span data-stu-id="4ebef-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="4ebef-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ebef-124">Permission type</span></span> | <span data-ttu-id="4ebef-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ebef-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4ebef-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebef-126">Delegated (work or school account)</span></span> | <span data-ttu-id="4ebef-127">对于 user： User： Read. All，Read. All</span><span class="sxs-lookup"><span data-stu-id="4ebef-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="4ebef-128">对于 device： Device. all、Directory、Read. All</span><span class="sxs-lookup"><span data-stu-id="4ebef-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="4ebef-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebef-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ebef-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebef-130">Not supported.</span></span> |
| <span data-ttu-id="4ebef-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ebef-131">Application</span></span>                            | <span data-ttu-id="4ebef-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebef-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ebef-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ebef-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="4ebef-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ebef-134">Request headers</span></span>

| <span data-ttu-id="4ebef-135">名称</span><span class="sxs-lookup"><span data-stu-id="4ebef-135">Name</span></span> | <span data-ttu-id="4ebef-136">说明</span><span class="sxs-lookup"><span data-stu-id="4ebef-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="4ebef-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ebef-137">Authorization</span></span> | <span data-ttu-id="4ebef-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4ebef-138">Bearer {token}</span></span> |
| <span data-ttu-id="4ebef-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="4ebef-139">Content-type</span></span>  | <span data-ttu-id="4ebef-140">application/json</span><span class="sxs-lookup"><span data-stu-id="4ebef-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ebef-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ebef-141">Request body</span></span>

<span data-ttu-id="4ebef-142">在请求正文中，提供所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ebef-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="4ebef-143">下表列出了评估组成员资格时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ebef-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="4ebef-144">参数</span><span class="sxs-lookup"><span data-stu-id="4ebef-144">Parameter</span></span> | <span data-ttu-id="4ebef-145">类型</span><span class="sxs-lookup"><span data-stu-id="4ebef-145">Type</span></span> | <span data-ttu-id="4ebef-146">说明</span><span class="sxs-lookup"><span data-stu-id="4ebef-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="4ebef-147">memberId</span><span class="sxs-lookup"><span data-stu-id="4ebef-147">memberId</span></span> | <span data-ttu-id="4ebef-148">字符串集合</span><span class="sxs-lookup"><span data-stu-id="4ebef-148">String collection</span></span> | <span data-ttu-id="4ebef-149">memberId 是要评估的用户或设备的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="4ebef-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="4ebef-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="4ebef-150">membershipRule</span></span> | <span data-ttu-id="4ebef-151">字符串集合</span><span class="sxs-lookup"><span data-stu-id="4ebef-151">String collection</span></span> | <span data-ttu-id="4ebef-152">用于成员资格评估的规则。</span><span class="sxs-lookup"><span data-stu-id="4ebef-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="4ebef-153">如果未提供此属性，则对现有组的规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="4ebef-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="4ebef-154">如果提供了此属性，则将针对具有相同规则的组中的可能成员资格评估用户或设备。</span><span class="sxs-lookup"><span data-stu-id="4ebef-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="4ebef-155">有关详细信息，请参阅 [Azure Active Directory 中的组的动态成员身份规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="4ebef-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="4ebef-156">响应</span><span class="sxs-lookup"><span data-stu-id="4ebef-156">Response</span></span>

<span data-ttu-id="4ebef-157">如果成功，此方法将返回 `200 OK` 响应代码和 [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ebef-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="4ebef-158">示例</span><span class="sxs-lookup"><span data-stu-id="4ebef-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="4ebef-159">示例1：评估用户或设备是否为现有组的成员</span><span class="sxs-lookup"><span data-stu-id="4ebef-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="4ebef-160">请求</span><span class="sxs-lookup"><span data-stu-id="4ebef-160">Request</span></span>

<span data-ttu-id="4ebef-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ebef-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4ebef-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ebef-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[<span data-ttu-id="4ebef-163">C#</span><span class="sxs-lookup"><span data-stu-id="4ebef-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ebef-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ebef-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ebef-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ebef-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ebef-166">响应</span><span class="sxs-lookup"><span data-stu-id="4ebef-166">Response</span></span>

<span data-ttu-id="4ebef-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ebef-167">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="4ebef-168">示例2：评估用户或设备是否是基于成员身份规则的组的成员</span><span class="sxs-lookup"><span data-stu-id="4ebef-168">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="4ebef-169">请求</span><span class="sxs-lookup"><span data-stu-id="4ebef-169">Request</span></span>

<span data-ttu-id="4ebef-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ebef-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4ebef-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ebef-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[<span data-ttu-id="4ebef-172">C#</span><span class="sxs-lookup"><span data-stu-id="4ebef-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ebef-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ebef-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ebef-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ebef-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4ebef-175">响应</span><span class="sxs-lookup"><span data-stu-id="4ebef-175">Response</span></span>

<span data-ttu-id="4ebef-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ebef-176">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->