---
title: 组： evaluateDynamicMembership
description: 评估用户或设备是否为动态组的成员。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d23e08d2e412f77e94c802fcc03778eb89ab7158
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012752"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="08f49-103">组： evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="08f49-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="08f49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08f49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f49-105">评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="08f49-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="08f49-106">成员身份规则与评估中使用的其他详细信息一起返回。</span><span class="sxs-lookup"><span data-stu-id="08f49-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="08f49-107">您可以通过以下方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="08f49-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="08f49-108">评估用户或设备是否为指定的动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="08f49-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="08f49-109">根据用户或设备的 ID 和成员身份规则评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="08f49-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="08f49-110">权限</span><span class="sxs-lookup"><span data-stu-id="08f49-110">Permissions</span></span>

<span data-ttu-id="08f49-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08f49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="08f49-113">使用成员 ID 和组 ID 评估动态成员身份</span><span class="sxs-lookup"><span data-stu-id="08f49-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="08f49-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="08f49-114">Permission type</span></span> | <span data-ttu-id="08f49-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08f49-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="08f49-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08f49-116">Delegated (work or school account)</span></span> | <span data-ttu-id="08f49-117">对于 user： Group. All 和 Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="08f49-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="08f49-118">对于 device： Group. All 和 Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="08f49-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="08f49-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08f49-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08f49-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="08f49-120">Not supported.</span></span> |
| <span data-ttu-id="08f49-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="08f49-121">Application</span></span>                            | <span data-ttu-id="08f49-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="08f49-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="08f49-123">使用成员 ID 和成员身份规则评估动态成员资格</span><span class="sxs-lookup"><span data-stu-id="08f49-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="08f49-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="08f49-124">Permission type</span></span> | <span data-ttu-id="08f49-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08f49-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="08f49-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08f49-126">Delegated (work or school account)</span></span> | <span data-ttu-id="08f49-127">对于 user： User： Read. All，Read. All</span><span class="sxs-lookup"><span data-stu-id="08f49-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="08f49-128">对于 device： Device. all、Directory、Read. All</span><span class="sxs-lookup"><span data-stu-id="08f49-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="08f49-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08f49-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08f49-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="08f49-130">Not supported.</span></span> |
| <span data-ttu-id="08f49-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="08f49-131">Application</span></span>                            | <span data-ttu-id="08f49-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="08f49-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08f49-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08f49-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="08f49-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="08f49-134">Request headers</span></span>

| <span data-ttu-id="08f49-135">名称</span><span class="sxs-lookup"><span data-stu-id="08f49-135">Name</span></span> | <span data-ttu-id="08f49-136">说明</span><span class="sxs-lookup"><span data-stu-id="08f49-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="08f49-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="08f49-137">Authorization</span></span> | <span data-ttu-id="08f49-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="08f49-138">Bearer {token}</span></span> |
| <span data-ttu-id="08f49-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="08f49-139">Content-type</span></span>  | <span data-ttu-id="08f49-140">application/json</span><span class="sxs-lookup"><span data-stu-id="08f49-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08f49-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="08f49-141">Request body</span></span>

<span data-ttu-id="08f49-142">在请求正文中，提供所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08f49-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="08f49-143">下表列出了评估组成员资格时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08f49-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="08f49-144">参数</span><span class="sxs-lookup"><span data-stu-id="08f49-144">Parameter</span></span> | <span data-ttu-id="08f49-145">类型</span><span class="sxs-lookup"><span data-stu-id="08f49-145">Type</span></span> | <span data-ttu-id="08f49-146">说明</span><span class="sxs-lookup"><span data-stu-id="08f49-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="08f49-147">memberId</span><span class="sxs-lookup"><span data-stu-id="08f49-147">memberId</span></span> | <span data-ttu-id="08f49-148">String collection</span><span class="sxs-lookup"><span data-stu-id="08f49-148">String collection</span></span> | <span data-ttu-id="08f49-149">memberId 是要评估的用户或设备的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="08f49-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="08f49-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="08f49-150">membershipRule</span></span> | <span data-ttu-id="08f49-151">String collection</span><span class="sxs-lookup"><span data-stu-id="08f49-151">String collection</span></span> | <span data-ttu-id="08f49-152">用于成员资格评估的规则。</span><span class="sxs-lookup"><span data-stu-id="08f49-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="08f49-153">如果未提供此属性，则对现有组的规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="08f49-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="08f49-154">如果提供了此属性，则将针对具有相同规则的组中的可能成员资格评估用户或设备。</span><span class="sxs-lookup"><span data-stu-id="08f49-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="08f49-155">有关详细信息，请参阅 [Azure Active Directory 中的组的动态成员身份规则](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="08f49-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="08f49-156">响应</span><span class="sxs-lookup"><span data-stu-id="08f49-156">Response</span></span>

<span data-ttu-id="08f49-157">如果成功，此方法将返回 `200 OK` 响应代码和 [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08f49-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="08f49-158">示例</span><span class="sxs-lookup"><span data-stu-id="08f49-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="08f49-159">示例1：评估用户或设备是否为现有组的成员</span><span class="sxs-lookup"><span data-stu-id="08f49-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="08f49-160">请求</span><span class="sxs-lookup"><span data-stu-id="08f49-160">Request</span></span>

<span data-ttu-id="08f49-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08f49-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08f49-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="08f49-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08f49-163">C#</span><span class="sxs-lookup"><span data-stu-id="08f49-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08f49-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08f49-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08f49-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08f49-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08f49-166">响应</span><span class="sxs-lookup"><span data-stu-id="08f49-166">Response</span></span>

<span data-ttu-id="08f49-167">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="08f49-167">The following is an example of the response.</span></span> 

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

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="08f49-168">示例2：评估用户或设备是否是基于成员身份规则的组的成员</span><span class="sxs-lookup"><span data-stu-id="08f49-168">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="08f49-169">请求</span><span class="sxs-lookup"><span data-stu-id="08f49-169">Request</span></span>

<span data-ttu-id="08f49-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08f49-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08f49-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="08f49-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08f49-172">C#</span><span class="sxs-lookup"><span data-stu-id="08f49-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08f49-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08f49-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08f49-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08f49-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08f49-175">响应</span><span class="sxs-lookup"><span data-stu-id="08f49-175">Response</span></span>

<span data-ttu-id="08f49-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08f49-176">The following is an example of the response.</span></span> 

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


