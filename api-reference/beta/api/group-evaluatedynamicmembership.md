---
title: group： evaluateDynamicMembership
description: 评估用户或设备是或将是动态组的成员。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: de8e44a79644bcea5e3c44b214580e16359468e2
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681758"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="dbbfb-103">group： evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="dbbfb-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="dbbfb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbbfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbbfb-105">评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="dbbfb-106">将返回成员身份规则以及评估中使用的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="dbbfb-107">可以按照以下方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="dbbfb-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="dbbfb-108">评估用户或设备是否是指定动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="dbbfb-109">根据用户或设备的 ID 以及成员身份规则，评估用户或设备是否是动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbbfb-110">权限</span><span class="sxs-lookup"><span data-stu-id="dbbfb-110">Permissions</span></span>

<span data-ttu-id="dbbfb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="dbbfb-113">评估具有成员 ID 和组 ID 的动态成员身份</span><span class="sxs-lookup"><span data-stu-id="dbbfb-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="dbbfb-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbbfb-114">Permission type</span></span> | <span data-ttu-id="dbbfb-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbbfb-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="dbbfb-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbbfb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="dbbfb-117">对于用户：Group.Read.All 和 User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbfb-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="dbbfb-118">对于设备：Group.Read.All 和 Device.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbfb-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="dbbfb-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbbfb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbbfb-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-120">Not supported.</span></span> |
| <span data-ttu-id="dbbfb-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbbfb-121">Application</span></span>                            | <span data-ttu-id="dbbfb-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="dbbfb-123">使用成员 ID 和成员身份规则评估动态成员身份</span><span class="sxs-lookup"><span data-stu-id="dbbfb-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="dbbfb-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbbfb-124">Permission type</span></span> | <span data-ttu-id="dbbfb-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbbfb-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="dbbfb-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbbfb-126">Delegated (work or school account)</span></span> | <span data-ttu-id="dbbfb-127">对于用户：User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbfb-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="dbbfb-128">对于设备：Device.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbfb-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="dbbfb-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbbfb-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbbfb-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-130">Not supported.</span></span> |
| <span data-ttu-id="dbbfb-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbbfb-131">Application</span></span>                            | <span data-ttu-id="dbbfb-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbbfb-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbbfb-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="dbbfb-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbbfb-134">Request headers</span></span>

| <span data-ttu-id="dbbfb-135">名称</span><span class="sxs-lookup"><span data-stu-id="dbbfb-135">Name</span></span> | <span data-ttu-id="dbbfb-136">说明</span><span class="sxs-lookup"><span data-stu-id="dbbfb-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="dbbfb-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbbfb-137">Authorization</span></span> | <span data-ttu-id="dbbfb-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dbbfb-138">Bearer {token}</span></span> |
| <span data-ttu-id="dbbfb-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="dbbfb-139">Content-type</span></span>  | <span data-ttu-id="dbbfb-140">application/json</span><span class="sxs-lookup"><span data-stu-id="dbbfb-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbbfb-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbbfb-141">Request body</span></span>

<span data-ttu-id="dbbfb-142">在请求正文中，提供所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="dbbfb-143">下表列出了评估组成员身份时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="dbbfb-144">参数</span><span class="sxs-lookup"><span data-stu-id="dbbfb-144">Parameter</span></span> | <span data-ttu-id="dbbfb-145">类型</span><span class="sxs-lookup"><span data-stu-id="dbbfb-145">Type</span></span> | <span data-ttu-id="dbbfb-146">说明</span><span class="sxs-lookup"><span data-stu-id="dbbfb-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="dbbfb-147">memberId</span><span class="sxs-lookup"><span data-stu-id="dbbfb-147">memberId</span></span> | <span data-ttu-id="dbbfb-148">String collection</span><span class="sxs-lookup"><span data-stu-id="dbbfb-148">String collection</span></span> | <span data-ttu-id="dbbfb-149">memberId 是要评估的用户或设备的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="dbbfb-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="dbbfb-150">membershipRule</span></span> | <span data-ttu-id="dbbfb-151">String collection</span><span class="sxs-lookup"><span data-stu-id="dbbfb-151">String collection</span></span> | <span data-ttu-id="dbbfb-152">用于成员评估的规则。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="dbbfb-153">如果未提供此属性，则评估现有组的规则。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="dbbfb-154">如果提供此属性，将评估用户或设备是否具有同一规则组中可能的成员身份。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="dbbfb-155">有关详细信息，请参阅 Dynamic [membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="dbbfb-156">响应</span><span class="sxs-lookup"><span data-stu-id="dbbfb-156">Response</span></span>

<span data-ttu-id="dbbfb-157">如果成功，此方法返回 `200 OK` 响应代码和 [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="dbbfb-158">示例</span><span class="sxs-lookup"><span data-stu-id="dbbfb-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="dbbfb-159">示例 1：评估用户或设备是现有组的成员</span><span class="sxs-lookup"><span data-stu-id="dbbfb-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="dbbfb-160">请求</span><span class="sxs-lookup"><span data-stu-id="dbbfb-160">Request</span></span>

<span data-ttu-id="dbbfb-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dbbfb-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbbfb-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dbbfb-163">C#</span><span class="sxs-lookup"><span data-stu-id="dbbfb-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbbfb-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbbfb-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbbfb-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbbfb-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dbbfb-166">Java</span><span class="sxs-lookup"><span data-stu-id="dbbfb-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbbfb-167">响应</span><span class="sxs-lookup"><span data-stu-id="dbbfb-167">Response</span></span>

<span data-ttu-id="dbbfb-168">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-168">The following is an example of the response.</span></span> 

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

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="dbbfb-169">示例 2：根据成员身份规则评估用户或设备是否为组的成员</span><span class="sxs-lookup"><span data-stu-id="dbbfb-169">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="dbbfb-170">请求</span><span class="sxs-lookup"><span data-stu-id="dbbfb-170">Request</span></span>

<span data-ttu-id="dbbfb-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dbbfb-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbbfb-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dbbfb-173">C#</span><span class="sxs-lookup"><span data-stu-id="dbbfb-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbbfb-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbbfb-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbbfb-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbbfb-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dbbfb-176">Java</span><span class="sxs-lookup"><span data-stu-id="dbbfb-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbbfb-177">响应</span><span class="sxs-lookup"><span data-stu-id="dbbfb-177">Response</span></span>

<span data-ttu-id="dbbfb-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dbbfb-178">The following is an example of the response.</span></span> 

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
