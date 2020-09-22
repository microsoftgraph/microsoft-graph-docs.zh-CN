---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定使用者可以通过访问包分配请求或分配访问包的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccf3e1bb94bb1f6186e39cdaa91fa2dbe3a4344d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031731"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="15006-103">accessPackageAssignmentPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="15006-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="15006-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15006-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15006-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配策略指定了主题可以通过访问包分配请求或分配访问包的策略。</span><span class="sxs-lookup"><span data-stu-id="15006-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="15006-106">访问包可以有零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="15006-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="15006-107">收到来自主题的请求时，主体将与每个策略相匹配，以查找策略 (如果任何包含该主题的 requestorSettings) 。</span><span class="sxs-lookup"><span data-stu-id="15006-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="15006-108">然后，该策略将确定请求是否需要审批、访问包分配的持续时间以及是否需要定期查看工作分配。</span><span class="sxs-lookup"><span data-stu-id="15006-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="15006-109">若要将用户分配到访问包，请 [创建一个](../api/accesspackageassignmentrequest-post.md) 引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="15006-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="15006-110">方法</span><span class="sxs-lookup"><span data-stu-id="15006-110">Methods</span></span>

| <span data-ttu-id="15006-111">方法</span><span class="sxs-lookup"><span data-stu-id="15006-111">Method</span></span>       | <span data-ttu-id="15006-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="15006-112">Return Type</span></span> | <span data-ttu-id="15006-113">说明</span><span class="sxs-lookup"><span data-stu-id="15006-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="15006-114">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="15006-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="15006-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15006-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="15006-116">检索 accessPackageAssignmentPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="15006-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="15006-117">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="15006-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="15006-119">创建新的 accessPackageAssignmentPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="15006-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="15006-120">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="15006-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="15006-122">读取 accessPackageAssignmentPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="15006-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="15006-123">更新 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="15006-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="15006-125">更新 accessPackageAssignmentPolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="15006-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="15006-126">删除 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="15006-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="15006-127">删除 accessPackageAssignmentPolicy。</span><span class="sxs-lookup"><span data-stu-id="15006-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="15006-128">属性</span><span class="sxs-lookup"><span data-stu-id="15006-128">Properties</span></span>

| <span data-ttu-id="15006-129">属性</span><span class="sxs-lookup"><span data-stu-id="15006-129">Property</span></span>     | <span data-ttu-id="15006-130">类型</span><span class="sxs-lookup"><span data-stu-id="15006-130">Type</span></span>        | <span data-ttu-id="15006-131">说明</span><span class="sxs-lookup"><span data-stu-id="15006-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="15006-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="15006-132">accessPackageId</span></span>|<span data-ttu-id="15006-133">String</span><span class="sxs-lookup"><span data-stu-id="15006-133">String</span></span>|<span data-ttu-id="15006-134">访问包的 ID。</span><span class="sxs-lookup"><span data-stu-id="15006-134">ID of the access package.</span></span>|
|<span data-ttu-id="15006-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="15006-135">accessReviewSettings</span></span>|[<span data-ttu-id="15006-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="15006-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="15006-137">必须对此策略中的访问包的分配以及这些工作分配的频率。</span><span class="sxs-lookup"><span data-stu-id="15006-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="15006-138">如果不需要进行审核，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="15006-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="15006-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="15006-139">canExtend</span></span>|<span data-ttu-id="15006-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="15006-140">Boolean</span></span>|<span data-ttu-id="15006-141">指示用户是否可以在批准后扩展访问包分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="15006-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="15006-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="15006-142">createdBy</span></span>|<span data-ttu-id="15006-143">String</span><span class="sxs-lookup"><span data-stu-id="15006-143">String</span></span>|<span data-ttu-id="15006-144">只读。</span><span class="sxs-lookup"><span data-stu-id="15006-144">Read-only.</span></span>|
|<span data-ttu-id="15006-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15006-145">createdDateTime</span></span>|<span data-ttu-id="15006-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15006-146">DateTimeOffset</span></span>|<span data-ttu-id="15006-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="15006-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="15006-149">description</span><span class="sxs-lookup"><span data-stu-id="15006-149">description</span></span>|<span data-ttu-id="15006-150">String</span><span class="sxs-lookup"><span data-stu-id="15006-150">String</span></span>|<span data-ttu-id="15006-151">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="15006-151">The description of the policy.</span></span>|
|<span data-ttu-id="15006-152">displayName</span><span class="sxs-lookup"><span data-stu-id="15006-152">displayName</span></span>|<span data-ttu-id="15006-153">String</span><span class="sxs-lookup"><span data-stu-id="15006-153">String</span></span>|<span data-ttu-id="15006-154">策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="15006-154">The display name of the policy.</span></span>|
|<span data-ttu-id="15006-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="15006-155">durationInDays</span></span>|<span data-ttu-id="15006-156">Int32</span><span class="sxs-lookup"><span data-stu-id="15006-156">Int32</span></span>|<span data-ttu-id="15006-157">此策略中的工作分配在过期之前持续的天数。</span><span class="sxs-lookup"><span data-stu-id="15006-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="15006-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="15006-158">expirationDateTime</span></span>|<span data-ttu-id="15006-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15006-159">DateTimeOffset</span></span>|<span data-ttu-id="15006-160">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="15006-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="15006-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="15006-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="15006-162">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="15006-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="15006-163">id</span><span class="sxs-lookup"><span data-stu-id="15006-163">id</span></span>|<span data-ttu-id="15006-164">String</span><span class="sxs-lookup"><span data-stu-id="15006-164">String</span></span>| <span data-ttu-id="15006-165">只读。</span><span class="sxs-lookup"><span data-stu-id="15006-165">Read-only.</span></span>|
|<span data-ttu-id="15006-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="15006-166">modifiedBy</span></span>|<span data-ttu-id="15006-167">String</span><span class="sxs-lookup"><span data-stu-id="15006-167">String</span></span>|<span data-ttu-id="15006-168">只读。</span><span class="sxs-lookup"><span data-stu-id="15006-168">Read-only.</span></span>|
|<span data-ttu-id="15006-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15006-169">modifiedDateTime</span></span>|<span data-ttu-id="15006-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15006-170">DateTimeOffset</span></span>|<span data-ttu-id="15006-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="15006-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="15006-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="15006-173">requestApprovalSettings</span></span>|[<span data-ttu-id="15006-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="15006-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="15006-175">必须在此策略中批准访问包的请求。</span><span class="sxs-lookup"><span data-stu-id="15006-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="15006-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="15006-176">requestorSettings</span></span>|[<span data-ttu-id="15006-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="15006-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="15006-178">可从该策略请求此访问包的人。</span><span class="sxs-lookup"><span data-stu-id="15006-178">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="15006-179">关系</span><span class="sxs-lookup"><span data-stu-id="15006-179">Relationships</span></span>

| <span data-ttu-id="15006-180">关系</span><span class="sxs-lookup"><span data-stu-id="15006-180">Relationship</span></span> | <span data-ttu-id="15006-181">类型</span><span class="sxs-lookup"><span data-stu-id="15006-181">Type</span></span>        | <span data-ttu-id="15006-182">说明</span><span class="sxs-lookup"><span data-stu-id="15006-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="15006-183">accessPackage</span><span class="sxs-lookup"><span data-stu-id="15006-183">accessPackage</span></span>|[<span data-ttu-id="15006-184">accessPackage</span><span class="sxs-lookup"><span data-stu-id="15006-184">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="15006-185">具有此策略的访问包。</span><span class="sxs-lookup"><span data-stu-id="15006-185">The access package with this policy.</span></span> <span data-ttu-id="15006-186">只读。</span><span class="sxs-lookup"><span data-stu-id="15006-186">Read-only.</span></span> <span data-ttu-id="15006-187">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="15006-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15006-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15006-188">JSON representation</span></span>

<span data-ttu-id="15006-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15006-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


