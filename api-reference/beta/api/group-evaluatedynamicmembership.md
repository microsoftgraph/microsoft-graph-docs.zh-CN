---
title: group： evaluateDynamicMembership
description: 评估用户或设备是或将是动态组的成员。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 94594d31c4e7630b91905edb244f616cac1b21ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961879"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="25d9d-103">group： evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="25d9d-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="25d9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d9d-105">评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="25d9d-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="25d9d-106">将返回成员身份规则以及评估中使用的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="25d9d-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="25d9d-107">可以按照以下方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="25d9d-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="25d9d-108">评估用户或设备是否是指定动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="25d9d-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="25d9d-109">根据用户或设备的 ID 以及成员身份规则，评估用户或设备是否是动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="25d9d-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="25d9d-110">权限</span><span class="sxs-lookup"><span data-stu-id="25d9d-110">Permissions</span></span>

<span data-ttu-id="25d9d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25d9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="25d9d-113">评估具有成员 ID 和组 ID 的动态成员身份</span><span class="sxs-lookup"><span data-stu-id="25d9d-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="25d9d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="25d9d-114">Permission type</span></span> | <span data-ttu-id="25d9d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25d9d-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="25d9d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25d9d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="25d9d-117">对于用户：Group.Read.All 和 User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="25d9d-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="25d9d-118">对于设备：Group.Read.All 和 Device.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="25d9d-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="25d9d-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25d9d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25d9d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="25d9d-120">Not supported.</span></span> |
| <span data-ttu-id="25d9d-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="25d9d-121">Application</span></span>                            | <span data-ttu-id="25d9d-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="25d9d-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="25d9d-123">使用成员 ID 和成员身份规则评估动态成员身份</span><span class="sxs-lookup"><span data-stu-id="25d9d-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="25d9d-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="25d9d-124">Permission type</span></span> | <span data-ttu-id="25d9d-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25d9d-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="25d9d-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25d9d-126">Delegated (work or school account)</span></span> | <span data-ttu-id="25d9d-127">对于用户：User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="25d9d-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="25d9d-128">对于设备：Device.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="25d9d-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="25d9d-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25d9d-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25d9d-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="25d9d-130">Not supported.</span></span> |
| <span data-ttu-id="25d9d-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="25d9d-131">Application</span></span>                            | <span data-ttu-id="25d9d-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="25d9d-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25d9d-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25d9d-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="25d9d-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="25d9d-134">Request headers</span></span>

| <span data-ttu-id="25d9d-135">名称</span><span class="sxs-lookup"><span data-stu-id="25d9d-135">Name</span></span> | <span data-ttu-id="25d9d-136">说明</span><span class="sxs-lookup"><span data-stu-id="25d9d-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="25d9d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="25d9d-137">Authorization</span></span> | <span data-ttu-id="25d9d-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="25d9d-138">Bearer {token}</span></span> |
| <span data-ttu-id="25d9d-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="25d9d-139">Content-type</span></span>  | <span data-ttu-id="25d9d-140">application/json</span><span class="sxs-lookup"><span data-stu-id="25d9d-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="25d9d-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="25d9d-141">Request body</span></span>

<span data-ttu-id="25d9d-142">在请求正文中，提供所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25d9d-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="25d9d-143">下表列出了评估组成员身份时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25d9d-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="25d9d-144">参数</span><span class="sxs-lookup"><span data-stu-id="25d9d-144">Parameter</span></span> | <span data-ttu-id="25d9d-145">类型</span><span class="sxs-lookup"><span data-stu-id="25d9d-145">Type</span></span> | <span data-ttu-id="25d9d-146">说明</span><span class="sxs-lookup"><span data-stu-id="25d9d-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="25d9d-147">memberId</span><span class="sxs-lookup"><span data-stu-id="25d9d-147">memberId</span></span> | <span data-ttu-id="25d9d-148">String collection</span><span class="sxs-lookup"><span data-stu-id="25d9d-148">String collection</span></span> | <span data-ttu-id="25d9d-149">memberId 是要评估的用户或设备的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="25d9d-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="25d9d-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="25d9d-150">membershipRule</span></span> | <span data-ttu-id="25d9d-151">String collection</span><span class="sxs-lookup"><span data-stu-id="25d9d-151">String collection</span></span> | <span data-ttu-id="25d9d-152">用于成员评估的规则。</span><span class="sxs-lookup"><span data-stu-id="25d9d-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="25d9d-153">如果未提供此属性，则评估现有组的规则。</span><span class="sxs-lookup"><span data-stu-id="25d9d-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="25d9d-154">如果提供此属性，将评估用户或设备是否具有同一规则组中可能的成员身份。</span><span class="sxs-lookup"><span data-stu-id="25d9d-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="25d9d-155">有关详细信息，请参阅 [Azure Active Directory 中组的动态成员身份规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="25d9d-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="25d9d-156">响应</span><span class="sxs-lookup"><span data-stu-id="25d9d-156">Response</span></span>

<span data-ttu-id="25d9d-157">如果成功，此方法返回 `200 OK` 响应代码和 [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25d9d-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="25d9d-158">示例</span><span class="sxs-lookup"><span data-stu-id="25d9d-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="25d9d-159">示例 1：评估用户或设备是现有组的成员</span><span class="sxs-lookup"><span data-stu-id="25d9d-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="25d9d-160">请求</span><span class="sxs-lookup"><span data-stu-id="25d9d-160">Request</span></span>

<span data-ttu-id="25d9d-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25d9d-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="25d9d-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="25d9d-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[<span data-ttu-id="25d9d-163">C#</span><span class="sxs-lookup"><span data-stu-id="25d9d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25d9d-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25d9d-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25d9d-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25d9d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25d9d-166">Java</span><span class="sxs-lookup"><span data-stu-id="25d9d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="25d9d-167">响应</span><span class="sxs-lookup"><span data-stu-id="25d9d-167">Response</span></span>

<span data-ttu-id="25d9d-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25d9d-168">The following is an example of the response.</span></span> 

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

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="25d9d-169">示例 2：根据成员身份规则评估用户或设备是否为组的成员</span><span class="sxs-lookup"><span data-stu-id="25d9d-169">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="25d9d-170">请求</span><span class="sxs-lookup"><span data-stu-id="25d9d-170">Request</span></span>

<span data-ttu-id="25d9d-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25d9d-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="25d9d-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="25d9d-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_2"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[<span data-ttu-id="25d9d-173">C#</span><span class="sxs-lookup"><span data-stu-id="25d9d-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25d9d-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25d9d-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25d9d-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25d9d-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25d9d-176">Java</span><span class="sxs-lookup"><span data-stu-id="25d9d-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="25d9d-177">响应</span><span class="sxs-lookup"><span data-stu-id="25d9d-177">Response</span></span>

<span data-ttu-id="25d9d-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25d9d-178">The following is an example of the response.</span></span> 

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
