---
title: 创建 accessPackageAssignmentPolicy
description: 使用此 API 创建新的 accessPackageAssignmentPolicy。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 707d3e7a11983f2ecc1ec9df9703582b01f33e2b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466955"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="75486-103">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="75486-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="75486-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75486-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75486-105">在 [Azure AD 权利管理中](../resources/entitlementmanagement-root.md)，创建新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75486-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75486-106">权限</span><span class="sxs-lookup"><span data-stu-id="75486-106">Permissions</span></span>

<span data-ttu-id="75486-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75486-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="75486-109">Permission type</span></span>                        | <span data-ttu-id="75486-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75486-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="75486-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75486-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75486-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75486-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="75486-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75486-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75486-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="75486-114">Not supported.</span></span> |
| <span data-ttu-id="75486-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="75486-115">Application</span></span>                            | <span data-ttu-id="75486-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75486-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75486-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75486-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="75486-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="75486-118">Request headers</span></span>

| <span data-ttu-id="75486-119">名称</span><span class="sxs-lookup"><span data-stu-id="75486-119">Name</span></span>          | <span data-ttu-id="75486-120">说明</span><span class="sxs-lookup"><span data-stu-id="75486-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="75486-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="75486-121">Authorization</span></span> | <span data-ttu-id="75486-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="75486-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="75486-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75486-124">Content-Type</span></span>  | <span data-ttu-id="75486-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="75486-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75486-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="75486-127">Request body</span></span>

<span data-ttu-id="75486-128">在请求正文中，提供 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75486-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="75486-129">响应</span><span class="sxs-lookup"><span data-stu-id="75486-129">Response</span></span>

<span data-ttu-id="75486-130">如果成功，此方法在响应正文中返回 200 系列响应代码和新 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75486-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75486-131">示例</span><span class="sxs-lookup"><span data-stu-id="75486-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="75486-132">示例 1：创建直接分配策略</span><span class="sxs-lookup"><span data-stu-id="75486-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="75486-133">如果访问包分配请求仅由管理员创建，而不是由用户自己创建，则直接分配策略非常有用。</span><span class="sxs-lookup"><span data-stu-id="75486-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="75486-134">请求</span><span class="sxs-lookup"><span data-stu-id="75486-134">Request</span></span>

<span data-ttu-id="75486-135">以下示例显示创建访问包分配策略的请求。</span><span class="sxs-lookup"><span data-stu-id="75486-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="75486-136">在此策略中，任何用户均无法请求，也不需要批准，也无需访问评审。</span><span class="sxs-lookup"><span data-stu-id="75486-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="75486-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="75486-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="75486-138">C#</span><span class="sxs-lookup"><span data-stu-id="75486-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75486-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75486-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75486-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75486-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75486-141">Java</span><span class="sxs-lookup"><span data-stu-id="75486-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="75486-142">响应</span><span class="sxs-lookup"><span data-stu-id="75486-142">Response</span></span>

<span data-ttu-id="75486-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="75486-143">The following is an example of the response.</span></span>

> <span data-ttu-id="75486-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="75486-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="75486-145">示例 2：为来自其他组织的用户创建策略以请求</span><span class="sxs-lookup"><span data-stu-id="75486-145">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="75486-146">以下示例显示了一个更复杂的策略，该策略具有两个阶段的审批和访问评审。</span><span class="sxs-lookup"><span data-stu-id="75486-146">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="75486-147">请求</span><span class="sxs-lookup"><span data-stu-id="75486-147">Request</span></span>

<span data-ttu-id="75486-148">下面是创建访问包分配策略的请求示例。</span><span class="sxs-lookup"><span data-stu-id="75486-148">The following is an example of the request to create an access package assignment policy.</span></span> 


# <a name="http"></a>[<span data-ttu-id="75486-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="75486-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="75486-150">C#</span><span class="sxs-lookup"><span data-stu-id="75486-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75486-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75486-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75486-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75486-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75486-153">Java</span><span class="sxs-lookup"><span data-stu-id="75486-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="75486-154">响应</span><span class="sxs-lookup"><span data-stu-id="75486-154">Response</span></span>

<span data-ttu-id="75486-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="75486-155">The following is an example of the response.</span></span>

> <span data-ttu-id="75486-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="75486-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-assignment-policy-with-questions"></a><span data-ttu-id="75486-157">示例 3：创建带问题的分配策略</span><span class="sxs-lookup"><span data-stu-id="75486-157">Example 3: Create assignment policy with questions</span></span>

<span data-ttu-id="75486-158">将在分配策略范围内向请求者提出在分配策略中配置的问题。</span><span class="sxs-lookup"><span data-stu-id="75486-158">Questions configured in an assignment policy will be asked to requestors in scope of the policy.</span></span> <span data-ttu-id="75486-159">他们的回答将显示给审批者。</span><span class="sxs-lookup"><span data-stu-id="75486-159">Their answers will be shown to their approvers.</span></span> <span data-ttu-id="75486-160">问题 ID 是只读的，并且默认包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="75486-160">Question IDs are read-only and are included in the response by default.</span></span>

#### <a name="request"></a><span data-ttu-id="75486-161">请求</span><span class="sxs-lookup"><span data-stu-id="75486-161">Request</span></span>

<span data-ttu-id="75486-162">以下示例显示创建访问包分配策略的请求。</span><span class="sxs-lookup"><span data-stu-id="75486-162">The following example shows a request to create an access package assignment policy.</span></span> 



# <a name="http"></a>[<span data-ttu-id="75486-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="75486-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies_questions"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
    "accessPackageId": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": false,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [{
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ]
            }
        ]
    },
    "questions": [{
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```
# <a name="c"></a>[<span data-ttu-id="75486-164">C#</span><span class="sxs-lookup"><span data-stu-id="75486-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75486-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75486-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75486-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75486-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75486-167">Java</span><span class="sxs-lookup"><span data-stu-id="75486-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---

#### <a name="response"></a><span data-ttu-id="75486-168">响应</span><span class="sxs-lookup"><span data-stu-id="75486-168">Response</span></span>

<span data-ttu-id="75486-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="75486-169">The following is an example of the response.</span></span>

> <span data-ttu-id="75486-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="75486-170">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
  "questions": [{
        "id" : "BD3F6B95-458D-4BC8-A9A6-8D4B29F64F3D",
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona?",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "id" : "F652C13C-A660-4E4C-A1E0-CE9FEC6EE57A",
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
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


