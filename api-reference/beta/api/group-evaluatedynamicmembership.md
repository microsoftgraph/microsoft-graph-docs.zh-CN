---
title: 组： evaluateDynamicMembership
description: 评估用户或设备是否为动态组的成员。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b49f89da63b68f15329f7f700cc7699ff07e6208
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272827"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="e81cb-103">组： evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="e81cb-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="e81cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e81cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e81cb-105">评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="e81cb-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="e81cb-106">成员身份规则与评估中使用的其他详细信息一起返回。</span><span class="sxs-lookup"><span data-stu-id="e81cb-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="e81cb-107">您可以通过以下方式完成此操作：</span><span class="sxs-lookup"><span data-stu-id="e81cb-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="e81cb-108">评估用户或设备是否为指定的动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="e81cb-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="e81cb-109">根据用户或设备的 ID 和成员身份规则评估用户或设备是否为动态组的成员。</span><span class="sxs-lookup"><span data-stu-id="e81cb-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="e81cb-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="e81cb-110">Permissions</span></span>

<span data-ttu-id="e81cb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e81cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="e81cb-113">使用成员 ID 和组 ID 评估动态成员身份</span><span class="sxs-lookup"><span data-stu-id="e81cb-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="e81cb-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e81cb-114">Permission type</span></span> | <span data-ttu-id="e81cb-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e81cb-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e81cb-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e81cb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e81cb-117">对于 user： Group. All 和 Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="e81cb-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="e81cb-118">对于 device： Group. All 和 Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="e81cb-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="e81cb-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e81cb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e81cb-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e81cb-120">Not supported.</span></span> |
| <span data-ttu-id="e81cb-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="e81cb-121">Application</span></span>                            | <span data-ttu-id="e81cb-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="e81cb-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="e81cb-123">使用成员 ID 和成员身份规则评估动态成员资格</span><span class="sxs-lookup"><span data-stu-id="e81cb-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="e81cb-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="e81cb-124">Permission type</span></span> | <span data-ttu-id="e81cb-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e81cb-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e81cb-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e81cb-126">Delegated (work or school account)</span></span> | <span data-ttu-id="e81cb-127">对于 user： User： Read. All，Read. All</span><span class="sxs-lookup"><span data-stu-id="e81cb-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="e81cb-128">对于 device： Device. all、Directory、Read. All</span><span class="sxs-lookup"><span data-stu-id="e81cb-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="e81cb-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e81cb-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e81cb-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="e81cb-130">Not supported.</span></span> |
| <span data-ttu-id="e81cb-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="e81cb-131">Application</span></span>                            | <span data-ttu-id="e81cb-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="e81cb-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e81cb-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e81cb-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="e81cb-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="e81cb-134">Request headers</span></span>

| <span data-ttu-id="e81cb-135">名称</span><span class="sxs-lookup"><span data-stu-id="e81cb-135">Name</span></span> | <span data-ttu-id="e81cb-136">说明</span><span class="sxs-lookup"><span data-stu-id="e81cb-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="e81cb-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="e81cb-137">Authorization</span></span> | <span data-ttu-id="e81cb-138">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="e81cb-138">Bearer {token}</span></span> |
| <span data-ttu-id="e81cb-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="e81cb-139">Content-type</span></span>  | <span data-ttu-id="e81cb-140">application/json</span><span class="sxs-lookup"><span data-stu-id="e81cb-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e81cb-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="e81cb-141">Request body</span></span>

<span data-ttu-id="e81cb-142">在请求正文中，提供所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e81cb-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="e81cb-143">下表列出了评估组成员资格时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e81cb-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="e81cb-144">参数</span><span class="sxs-lookup"><span data-stu-id="e81cb-144">Parameter</span></span> | <span data-ttu-id="e81cb-145">类型</span><span class="sxs-lookup"><span data-stu-id="e81cb-145">Type</span></span> | <span data-ttu-id="e81cb-146">Description</span><span class="sxs-lookup"><span data-stu-id="e81cb-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="e81cb-147">memberId</span><span class="sxs-lookup"><span data-stu-id="e81cb-147">memberId</span></span> | <span data-ttu-id="e81cb-148">String collection</span><span class="sxs-lookup"><span data-stu-id="e81cb-148">String collection</span></span> | <span data-ttu-id="e81cb-149">memberId 是要评估的用户或设备的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="e81cb-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="e81cb-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="e81cb-150">membershipRule</span></span> | <span data-ttu-id="e81cb-151">String collection</span><span class="sxs-lookup"><span data-stu-id="e81cb-151">String collection</span></span> | <span data-ttu-id="e81cb-152">用于成员资格评估的规则。</span><span class="sxs-lookup"><span data-stu-id="e81cb-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="e81cb-153">如果未提供此属性，则对现有组的规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="e81cb-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="e81cb-154">如果提供了此属性，则将针对具有相同规则的组中的可能成员资格评估用户或设备。</span><span class="sxs-lookup"><span data-stu-id="e81cb-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="e81cb-155">有关详细信息，请参阅[Azure Active Directory 中的组的动态成员身份规则](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="e81cb-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="e81cb-156">响应</span><span class="sxs-lookup"><span data-stu-id="e81cb-156">Response</span></span>

<span data-ttu-id="e81cb-157">如果成功，此方法将返回 `200 OK` 响应代码和[evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e81cb-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="e81cb-158">示例</span><span class="sxs-lookup"><span data-stu-id="e81cb-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="e81cb-159">示例1：评估用户或设备是否为现有组的成员</span><span class="sxs-lookup"><span data-stu-id="e81cb-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="e81cb-160">请求</span><span class="sxs-lookup"><span data-stu-id="e81cb-160">Request</span></span>

<span data-ttu-id="e81cb-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e81cb-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e81cb-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="e81cb-162">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="e81cb-163">响应</span><span class="sxs-lookup"><span data-stu-id="e81cb-163">Response</span></span>

<span data-ttu-id="e81cb-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e81cb-164">The following is an example of the response.</span></span> 

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

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="e81cb-165">示例2：评估用户或设备是否是基于成员身份规则的组的成员</span><span class="sxs-lookup"><span data-stu-id="e81cb-165">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="e81cb-166">请求</span><span class="sxs-lookup"><span data-stu-id="e81cb-166">Request</span></span>

<span data-ttu-id="e81cb-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e81cb-167">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="e81cb-168">响应</span><span class="sxs-lookup"><span data-stu-id="e81cb-168">Response</span></span>

<span data-ttu-id="e81cb-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e81cb-169">The following is an example of the response.</span></span> 

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
