---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定主题可通过访问包分配请求或分配访问包的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34716752715399d1e16f7edeb609eace4c9b9b0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155610"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="f8bea-103">accessPackageAssignmentPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8bea-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="f8bea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8bea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8bea-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配策略指定主题可通过访问包分配请求或分配访问包的策略。</span><span class="sxs-lookup"><span data-stu-id="f8bea-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="f8bea-106">访问包可以具有零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="f8bea-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="f8bea-107">收到主题的请求时，将针对每个策略匹配主题，以查找策略 (如果有包含该) requestorSettings 的策略。</span><span class="sxs-lookup"><span data-stu-id="f8bea-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="f8bea-108">然后，该策略确定请求是否需要审批、访问包分配的持续时间以及分配是否需要定期审阅。</span><span class="sxs-lookup"><span data-stu-id="f8bea-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="f8bea-109">若要将用户分配给访问包，请创建引用访问包和访问包分配策略的[accessPackageAssignmentRequest。](../api/accesspackageassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="f8bea-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="f8bea-110">方法</span><span class="sxs-lookup"><span data-stu-id="f8bea-110">Methods</span></span>

| <span data-ttu-id="f8bea-111">方法</span><span class="sxs-lookup"><span data-stu-id="f8bea-111">Method</span></span>       | <span data-ttu-id="f8bea-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8bea-112">Return Type</span></span> | <span data-ttu-id="f8bea-113">说明</span><span class="sxs-lookup"><span data-stu-id="f8bea-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f8bea-114">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="f8bea-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="f8bea-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8bea-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="f8bea-116">检索 accessPackageAssignmentPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f8bea-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="f8bea-117">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="f8bea-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="f8bea-119">创建新的 accessPackageAssignmentPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="f8bea-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="f8bea-120">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="f8bea-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="f8bea-122">读取 accessPackageAssignmentPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f8bea-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="f8bea-123">更新 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="f8bea-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="f8bea-125">更新 accessPackageAssignmentPolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8bea-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="f8bea-126">删除 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f8bea-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="f8bea-127">删除 accessPackageAssignmentPolicy。</span><span class="sxs-lookup"><span data-stu-id="f8bea-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="f8bea-128">属性</span><span class="sxs-lookup"><span data-stu-id="f8bea-128">Properties</span></span>

| <span data-ttu-id="f8bea-129">属性</span><span class="sxs-lookup"><span data-stu-id="f8bea-129">Property</span></span>     | <span data-ttu-id="f8bea-130">类型</span><span class="sxs-lookup"><span data-stu-id="f8bea-130">Type</span></span>        | <span data-ttu-id="f8bea-131">说明</span><span class="sxs-lookup"><span data-stu-id="f8bea-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8bea-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="f8bea-132">accessPackageId</span></span>|<span data-ttu-id="f8bea-133">String</span><span class="sxs-lookup"><span data-stu-id="f8bea-133">String</span></span>|<span data-ttu-id="f8bea-134">访问包的 ID。</span><span class="sxs-lookup"><span data-stu-id="f8bea-134">ID of the access package.</span></span>|
|<span data-ttu-id="f8bea-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="f8bea-135">accessReviewSettings</span></span>|[<span data-ttu-id="f8bea-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="f8bea-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="f8bea-137">谁必须查看此策略中对访问包的分配以及查看其分配多久。</span><span class="sxs-lookup"><span data-stu-id="f8bea-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="f8bea-138">如果不需要审阅，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="f8bea-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="f8bea-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="f8bea-139">canExtend</span></span>|<span data-ttu-id="f8bea-140">布尔</span><span class="sxs-lookup"><span data-stu-id="f8bea-140">Boolean</span></span>|<span data-ttu-id="f8bea-141">指示用户是否可以在审批后延长访问包分配持续时间。</span><span class="sxs-lookup"><span data-stu-id="f8bea-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="f8bea-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="f8bea-142">createdBy</span></span>|<span data-ttu-id="f8bea-143">String</span><span class="sxs-lookup"><span data-stu-id="f8bea-143">String</span></span>|<span data-ttu-id="f8bea-144">只读。</span><span class="sxs-lookup"><span data-stu-id="f8bea-144">Read-only.</span></span>|
|<span data-ttu-id="f8bea-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8bea-145">createdDateTime</span></span>|<span data-ttu-id="f8bea-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8bea-146">DateTimeOffset</span></span>|<span data-ttu-id="f8bea-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f8bea-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f8bea-149">说明</span><span class="sxs-lookup"><span data-stu-id="f8bea-149">description</span></span>|<span data-ttu-id="f8bea-150">String</span><span class="sxs-lookup"><span data-stu-id="f8bea-150">String</span></span>|<span data-ttu-id="f8bea-151">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="f8bea-151">The description of the policy.</span></span>|
|<span data-ttu-id="f8bea-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f8bea-152">displayName</span></span>|<span data-ttu-id="f8bea-153">String</span><span class="sxs-lookup"><span data-stu-id="f8bea-153">String</span></span>|<span data-ttu-id="f8bea-154">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="f8bea-154">The display name of the policy.</span></span>|
|<span data-ttu-id="f8bea-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="f8bea-155">durationInDays</span></span>|<span data-ttu-id="f8bea-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f8bea-156">Int32</span></span>|<span data-ttu-id="f8bea-157">此策略中的分配最后一次到期的天数。</span><span class="sxs-lookup"><span data-stu-id="f8bea-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="f8bea-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f8bea-158">expirationDateTime</span></span>|<span data-ttu-id="f8bea-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8bea-159">DateTimeOffset</span></span>|<span data-ttu-id="f8bea-160">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="f8bea-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="f8bea-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f8bea-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f8bea-162">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f8bea-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f8bea-163">id</span><span class="sxs-lookup"><span data-stu-id="f8bea-163">id</span></span>|<span data-ttu-id="f8bea-164">String</span><span class="sxs-lookup"><span data-stu-id="f8bea-164">String</span></span>| <span data-ttu-id="f8bea-165">只读。</span><span class="sxs-lookup"><span data-stu-id="f8bea-165">Read-only.</span></span>|
|<span data-ttu-id="f8bea-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="f8bea-166">modifiedBy</span></span>|<span data-ttu-id="f8bea-167">String</span><span class="sxs-lookup"><span data-stu-id="f8bea-167">String</span></span>|<span data-ttu-id="f8bea-168">只读。</span><span class="sxs-lookup"><span data-stu-id="f8bea-168">Read-only.</span></span>|
|<span data-ttu-id="f8bea-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8bea-169">modifiedDateTime</span></span>|<span data-ttu-id="f8bea-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8bea-170">DateTimeOffset</span></span>|<span data-ttu-id="f8bea-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f8bea-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f8bea-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="f8bea-173">requestApprovalSettings</span></span>|[<span data-ttu-id="f8bea-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="f8bea-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="f8bea-175">谁必须批准此策略中的访问包请求。</span><span class="sxs-lookup"><span data-stu-id="f8bea-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="f8bea-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="f8bea-176">requestorSettings</span></span>|[<span data-ttu-id="f8bea-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="f8bea-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="f8bea-178">谁能从此策略请求此访问包。</span><span class="sxs-lookup"><span data-stu-id="f8bea-178">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="f8bea-179">问题</span><span class="sxs-lookup"><span data-stu-id="f8bea-179">questions</span></span>|<span data-ttu-id="f8bea-180">[accessPackageQuestion](accesspackagequestion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8bea-180">[accessPackageQuestion](accesspackagequestion.md) collection</span></span>|<span data-ttu-id="f8bea-181">向请求者提出的问题。</span><span class="sxs-lookup"><span data-stu-id="f8bea-181">Questions that are posed to the  requestor.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f8bea-182">关系</span><span class="sxs-lookup"><span data-stu-id="f8bea-182">Relationships</span></span>

| <span data-ttu-id="f8bea-183">关系</span><span class="sxs-lookup"><span data-stu-id="f8bea-183">Relationship</span></span> | <span data-ttu-id="f8bea-184">类型</span><span class="sxs-lookup"><span data-stu-id="f8bea-184">Type</span></span>        | <span data-ttu-id="f8bea-185">说明</span><span class="sxs-lookup"><span data-stu-id="f8bea-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8bea-186">accessPackage</span><span class="sxs-lookup"><span data-stu-id="f8bea-186">accessPackage</span></span>|[<span data-ttu-id="f8bea-187">accessPackage</span><span class="sxs-lookup"><span data-stu-id="f8bea-187">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="f8bea-188">具有此策略的访问包。</span><span class="sxs-lookup"><span data-stu-id="f8bea-188">The access package with this policy.</span></span> <span data-ttu-id="f8bea-189">只读。</span><span class="sxs-lookup"><span data-stu-id="f8bea-189">Read-only.</span></span> <span data-ttu-id="f8bea-190">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f8bea-190">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8bea-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8bea-191">JSON representation</span></span>

<span data-ttu-id="f8bea-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8bea-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "string",
    "accessPackageId": "string",
    "displayName": "string",
    "description": "string",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings": {
        "scopeType": "string",
        "acceptRequests": true,
        "allowedRequestors": [{
            "@odata.type": "#microsoft.graph.userSet"
        }]
    },
    "requestApprovalSettings": {
        "isApprovalRequired": false,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": false,
        "approvalMode": "string",
        "approvalStages": [{
            "approvalStageTimeOutInDays": 14,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 11520,
            "primaryApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }],
            "escalationApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }]
        }]
    },
    "accessReviewSettings": null,
    "questions": [{
        "@odata.type": "#microsoft.graph.question"
    }]
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

