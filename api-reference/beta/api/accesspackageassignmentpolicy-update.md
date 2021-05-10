---
title: 更新 accessPackageAssignmentPolicy
description: 更新 accessPackageAssignmentPolicy 对象的属性。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 32e93a6aa60793ba4fd30977d030dd2263a8c4c9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298339"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="a448d-103">更新 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="a448d-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="a448d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a448d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a448d-105">更新现有 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象以更改其一个或多个属性，如显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="a448d-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="a448d-106">权限</span><span class="sxs-lookup"><span data-stu-id="a448d-106">Permissions</span></span>
<span data-ttu-id="a448d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a448d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="a448d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a448d-109">Permission type</span></span>|<span data-ttu-id="a448d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a448d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a448d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a448d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a448d-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a448d-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="a448d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a448d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a448d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a448d-114">Not supported.</span></span> |
|<span data-ttu-id="a448d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a448d-115">Application</span></span>                            | <span data-ttu-id="a448d-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a448d-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a448d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a448d-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="a448d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a448d-118">Request headers</span></span>
|<span data-ttu-id="a448d-119">名称</span><span class="sxs-lookup"><span data-stu-id="a448d-119">Name</span></span>|<span data-ttu-id="a448d-120">说明</span><span class="sxs-lookup"><span data-stu-id="a448d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a448d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a448d-121">Authorization</span></span>|<span data-ttu-id="a448d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a448d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a448d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a448d-124">Content-Type</span></span>|<span data-ttu-id="a448d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a448d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a448d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a448d-127">Request body</span></span>
<span data-ttu-id="a448d-128">在请求正文中，提供 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a448d-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="a448d-129">下表显示更新 [accessPackageAssignmentPolicy 时所需的属性](../resources/accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="a448d-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="a448d-130">属性</span><span class="sxs-lookup"><span data-stu-id="a448d-130">Property</span></span>|<span data-ttu-id="a448d-131">类型</span><span class="sxs-lookup"><span data-stu-id="a448d-131">Type</span></span>|<span data-ttu-id="a448d-132">说明</span><span class="sxs-lookup"><span data-stu-id="a448d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a448d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a448d-133">displayName</span></span>|<span data-ttu-id="a448d-134">String</span><span class="sxs-lookup"><span data-stu-id="a448d-134">String</span></span>|<span data-ttu-id="a448d-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="a448d-135">The display name of the policy.</span></span>|
|<span data-ttu-id="a448d-136">说明</span><span class="sxs-lookup"><span data-stu-id="a448d-136">description</span></span>|<span data-ttu-id="a448d-137">String</span><span class="sxs-lookup"><span data-stu-id="a448d-137">String</span></span>|<span data-ttu-id="a448d-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a448d-138">The description of the policy.</span></span>|
|<span data-ttu-id="a448d-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="a448d-139">canExtend</span></span>|<span data-ttu-id="a448d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a448d-140">Boolean</span></span>|<span data-ttu-id="a448d-141">指示用户是否可以在审批后延长访问包分配持续时间。</span><span class="sxs-lookup"><span data-stu-id="a448d-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="a448d-142">durationInDays</span><span class="sxs-lookup"><span data-stu-id="a448d-142">durationInDays</span></span>|<span data-ttu-id="a448d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a448d-143">Int32</span></span>|<span data-ttu-id="a448d-144">此策略中的分配在到期之前持续等待的天数。</span><span class="sxs-lookup"><span data-stu-id="a448d-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="a448d-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a448d-145">expirationDateTime</span></span>|<span data-ttu-id="a448d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a448d-146">DateTimeOffset</span></span>|<span data-ttu-id="a448d-147">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="a448d-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="a448d-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a448d-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a448d-149">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a448d-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a448d-150">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="a448d-150">requestorSettings</span></span>|[<span data-ttu-id="a448d-151">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="a448d-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="a448d-152">Who从此策略请求此访问包。</span><span class="sxs-lookup"><span data-stu-id="a448d-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="a448d-153">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="a448d-153">requestApprovalSettings</span></span>|[<span data-ttu-id="a448d-154">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="a448d-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="a448d-155">Who必须批准此策略中的访问包请求。</span><span class="sxs-lookup"><span data-stu-id="a448d-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="a448d-156">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="a448d-156">accessReviewSettings</span></span>|[<span data-ttu-id="a448d-157">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="a448d-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="a448d-158">Who必须检查此策略中对访问包的分配以及分配时间。</span><span class="sxs-lookup"><span data-stu-id="a448d-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="a448d-159">如果不需要审阅，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="a448d-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="a448d-160">响应</span><span class="sxs-lookup"><span data-stu-id="a448d-160">Response</span></span>
<span data-ttu-id="a448d-161">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a448d-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="a448d-162">示例</span><span class="sxs-lookup"><span data-stu-id="a448d-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a448d-163">请求</span><span class="sxs-lookup"><span data-stu-id="a448d-163">Request</span></span>
<span data-ttu-id="a448d-164">在此策略更新中，已删除多选问题的选项之一。</span><span class="sxs-lookup"><span data-stu-id="a448d-164">In this policy update, one of the options for the multiple choice question was removed.</span></span> <span data-ttu-id="a448d-165">未来请求者将不再可以使用已删除的选项。</span><span class="sxs-lookup"><span data-stu-id="a448d-165">Future requestors will no longer have the removed option available to them.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf
Content-Type: application/json
Content-length: 1000

{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
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
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
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
    "accessReviewSettings": {
        "isEnabled": false
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


# <a name="java"></a>[<span data-ttu-id="a448d-166">Java</span><span class="sxs-lookup"><span data-stu-id="a448d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a448d-167">C#</span><span class="sxs-lookup"><span data-stu-id="a448d-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a448d-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a448d-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a448d-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a448d-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a448d-170">响应</span><span class="sxs-lookup"><span data-stu-id="a448d-170">Response</span></span>
> <span data-ttu-id="a448d-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a448d-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
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

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


