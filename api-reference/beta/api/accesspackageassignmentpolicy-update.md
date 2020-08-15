---
title: 更新 accessPackageAssignmentPolicy
description: 更新 accessPackageAssignmentPolicy 对象的属性。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a0d83dc1ca17baf5fd179efe225af8694b5ea6bb
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757413"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="2a116-103">更新 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="2a116-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="2a116-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a116-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a116-105">更新现有 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象以更改其一个或多个属性，如显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="2a116-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a116-106">权限</span><span class="sxs-lookup"><span data-stu-id="2a116-106">Permissions</span></span>
<span data-ttu-id="2a116-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2a116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="2a116-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a116-109">Permission type</span></span>|<span data-ttu-id="2a116-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a116-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a116-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a116-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a116-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a116-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="2a116-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a116-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a116-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a116-114">Not supported.</span></span> |
|<span data-ttu-id="2a116-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a116-115">Application</span></span>                            | <span data-ttu-id="2a116-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a116-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a116-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a116-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="2a116-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a116-118">Request headers</span></span>
|<span data-ttu-id="2a116-119">名称</span><span class="sxs-lookup"><span data-stu-id="2a116-119">Name</span></span>|<span data-ttu-id="2a116-120">说明</span><span class="sxs-lookup"><span data-stu-id="2a116-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a116-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a116-121">Authorization</span></span>|<span data-ttu-id="2a116-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a116-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a116-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a116-124">Content-Type</span></span>|<span data-ttu-id="2a116-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2a116-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a116-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a116-127">Request body</span></span>
<span data-ttu-id="2a116-128">在请求正文中，提供 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a116-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="2a116-129">下表显示了在更新 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a116-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="2a116-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a116-130">Property</span></span>|<span data-ttu-id="2a116-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a116-131">Type</span></span>|<span data-ttu-id="2a116-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a116-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a116-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2a116-133">displayName</span></span>|<span data-ttu-id="2a116-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2a116-134">String</span></span>|<span data-ttu-id="2a116-135">策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2a116-135">The display name of the policy.</span></span>|
|<span data-ttu-id="2a116-136">说明</span><span class="sxs-lookup"><span data-stu-id="2a116-136">description</span></span>|<span data-ttu-id="2a116-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2a116-137">String</span></span>|<span data-ttu-id="2a116-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="2a116-138">The description of the policy.</span></span>|
|<span data-ttu-id="2a116-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="2a116-139">canExtend</span></span>|<span data-ttu-id="2a116-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a116-140">Boolean</span></span>|<span data-ttu-id="2a116-141">指示用户是否可以在批准后扩展访问包分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="2a116-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="2a116-142">durationInDays</span><span class="sxs-lookup"><span data-stu-id="2a116-142">durationInDays</span></span>|<span data-ttu-id="2a116-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2a116-143">Int32</span></span>|<span data-ttu-id="2a116-144">此策略中的工作分配在过期之前持续的天数。</span><span class="sxs-lookup"><span data-stu-id="2a116-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="2a116-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2a116-145">expirationDateTime</span></span>|<span data-ttu-id="2a116-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a116-146">DateTimeOffset</span></span>|<span data-ttu-id="2a116-147">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="2a116-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="2a116-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2a116-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a116-149">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2a116-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2a116-150">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="2a116-150">requestorSettings</span></span>|[<span data-ttu-id="2a116-151">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="2a116-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="2a116-152">可从该策略请求此访问包的人。</span><span class="sxs-lookup"><span data-stu-id="2a116-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="2a116-153">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="2a116-153">requestApprovalSettings</span></span>|[<span data-ttu-id="2a116-154">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="2a116-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="2a116-155">必须在此策略中批准访问包的请求。</span><span class="sxs-lookup"><span data-stu-id="2a116-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="2a116-156">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="2a116-156">accessReviewSettings</span></span>|[<span data-ttu-id="2a116-157">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="2a116-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="2a116-158">必须对此策略中的访问包的分配以及这些工作分配的频率。</span><span class="sxs-lookup"><span data-stu-id="2a116-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="2a116-159">如果不需要进行审核，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="2a116-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="2a116-160">响应</span><span class="sxs-lookup"><span data-stu-id="2a116-160">Response</span></span>
<span data-ttu-id="2a116-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a116-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="2a116-162">示例</span><span class="sxs-lookup"><span data-stu-id="2a116-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a116-163">请求</span><span class="sxs-lookup"><span data-stu-id="2a116-163">Request</span></span>
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
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "requestorSettings" : {
    "scopeType": "AllExistingDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings" : {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  },
  "accessReviewSettings" : null
}
```


### <a name="response"></a><span data-ttu-id="2a116-164">响应</span><span class="sxs-lookup"><span data-stu-id="2a116-164">Response</span></span>
<span data-ttu-id="2a116-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2a116-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings" : null
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
