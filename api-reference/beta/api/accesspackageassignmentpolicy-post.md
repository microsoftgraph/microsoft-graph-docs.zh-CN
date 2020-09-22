---
title: 创建 accessPackageAssignmentPolicy
description: 使用此 API 创建新的 accessPackageAssignmentPolicy。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b4ffb8b887daea27c3409db25471873e7efb47f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983870"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="136df-103">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="136df-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="136df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="136df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="136df-105">在 [AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，创建一个新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="136df-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="136df-106">权限</span><span class="sxs-lookup"><span data-stu-id="136df-106">Permissions</span></span>

<span data-ttu-id="136df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="136df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="136df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="136df-109">Permission type</span></span>                        | <span data-ttu-id="136df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="136df-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="136df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="136df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="136df-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136df-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="136df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="136df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="136df-114">Not supported.</span></span> |
| <span data-ttu-id="136df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="136df-115">Application</span></span>                            | <span data-ttu-id="136df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="136df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="136df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="136df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="136df-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="136df-118">Request headers</span></span>

| <span data-ttu-id="136df-119">名称</span><span class="sxs-lookup"><span data-stu-id="136df-119">Name</span></span>          | <span data-ttu-id="136df-120">说明</span><span class="sxs-lookup"><span data-stu-id="136df-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="136df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="136df-121">Authorization</span></span> | <span data-ttu-id="136df-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="136df-122">Bearer \{token\}.</span></span> <span data-ttu-id="136df-123">必需。</span><span class="sxs-lookup"><span data-stu-id="136df-123">Required.</span></span> |
| <span data-ttu-id="136df-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="136df-124">Content-Type</span></span>  | <span data-ttu-id="136df-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="136df-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="136df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="136df-127">Request body</span></span>

<span data-ttu-id="136df-128">在请求正文中，提供 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="136df-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="136df-129">响应</span><span class="sxs-lookup"><span data-stu-id="136df-129">Response</span></span>

<span data-ttu-id="136df-130">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="136df-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="136df-131">示例</span><span class="sxs-lookup"><span data-stu-id="136df-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="136df-132">示例1：创建直接分配策略</span><span class="sxs-lookup"><span data-stu-id="136df-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="136df-133">当 access 程序包分配请求将仅由管理员创建，而不是由用户自己创建时，直接分配策略非常有用。</span><span class="sxs-lookup"><span data-stu-id="136df-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="136df-134">请求</span><span class="sxs-lookup"><span data-stu-id="136df-134">Request</span></span>

<span data-ttu-id="136df-135">以下示例显示了创建访问包分配策略的请求。</span><span class="sxs-lookup"><span data-stu-id="136df-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="136df-136">在此策略中，任何用户都不能请求，无需进行审批，也不会进行任何访问审核。</span><span class="sxs-lookup"><span data-stu-id="136df-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="136df-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="136df-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "NoSubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```
# <a name="c"></a>[<span data-ttu-id="136df-138">C#</span><span class="sxs-lookup"><span data-stu-id="136df-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="136df-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="136df-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="136df-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="136df-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="136df-141">响应</span><span class="sxs-lookup"><span data-stu-id="136df-141">Response</span></span>

<span data-ttu-id="136df-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="136df-142">The following is an example of the response.</span></span>

> <span data-ttu-id="136df-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="136df-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator"
}
```

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="136df-145">示例2：为来自其他组织的用户创建策略以请求</span><span class="sxs-lookup"><span data-stu-id="136df-145">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="136df-146">下面的示例展示了一个更复杂的策略，其中包含两个阶段的批准和访问审查。</span><span class="sxs-lookup"><span data-stu-id="136df-146">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="136df-147">请求</span><span class="sxs-lookup"><span data-stu-id="136df-147">Request</span></span>

<span data-ttu-id="136df-148">下面是创建访问包分配策略的请求示例。</span><span class="sxs-lookup"><span data-stu-id="136df-148">The following is an example of the request to create an access package assignment policy.</span></span> 


# <a name="http"></a>[<span data-ttu-id="136df-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="136df-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies_multistage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
    "accessPackageId": "string (identifier)",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true,
        "allowedRequestors": []
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "Serial",
        "approvalStages": [
            {
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ],
                "escalationApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "user if the external sponsor does not respond"
                    }
                ]
            },
            {
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "group for users from connected organizations which have no internal sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.internalSponsors",
                        "isBackup": false
                    }
                ],
                "escalationApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "user if the internal sponsor does not respond"
                    }
                ]
            }
        ]
    },
    "accessReviewSettings": {
        "isEnabled": true,
        "recurrenceType": "quarterly",
        "reviewerType": "Self",
        "startDateTime": "2020-04-01T07:59:59.998Z",
        "durationInDays": 25,
        "reviewers": []
    }
}
```
# <a name="c"></a>[<span data-ttu-id="136df-150">C#</span><span class="sxs-lookup"><span data-stu-id="136df-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="136df-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="136df-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="136df-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="136df-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="136df-153">响应</span><span class="sxs-lookup"><span data-stu-id="136df-153">Response</span></span>

<span data-ttu-id="136df-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="136df-154">The following is an example of the response.</span></span>

> <span data-ttu-id="136df-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="136df-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "string (identifier)",
  "displayName": "Users from connected organizations can request",
  "description": "Allow users from configured connected organizations to request and be approved by their sponsors"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


