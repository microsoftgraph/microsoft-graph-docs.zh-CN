---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定使用者可以通过访问包分配请求或分配访问包的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dd70512db17df29685c4af2d8aa4c410a78642b0
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534444"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="3e0c3-103">accessPackageAssignmentPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e0c3-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="3e0c3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3e0c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e0c3-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配策略指定了主题可以通过访问包分配请求或分配访问包的策略。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="3e0c3-106">访问包可以有零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="3e0c3-107">收到来自主题的请求时，主题将与每个策略相匹配，以查找包含该主题的 requestorSettings 策略（如果有）。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="3e0c3-108">然后，该策略将确定请求是否需要审批、访问包分配的持续时间以及是否需要定期查看工作分配。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="3e0c3-109">若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="3e0c3-110">方法</span><span class="sxs-lookup"><span data-stu-id="3e0c3-110">Methods</span></span>

| <span data-ttu-id="3e0c3-111">方法</span><span class="sxs-lookup"><span data-stu-id="3e0c3-111">Method</span></span>       | <span data-ttu-id="3e0c3-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e0c3-112">Return Type</span></span> | <span data-ttu-id="3e0c3-113">说明</span><span class="sxs-lookup"><span data-stu-id="3e0c3-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e0c3-114">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="3e0c3-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="3e0c3-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e0c3-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="3e0c3-116">检索 accessPackageAssignmentPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="3e0c3-117">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="3e0c3-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="3e0c3-119">创建新的 accessPackageAssignmentPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="3e0c3-120">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="3e0c3-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="3e0c3-122">读取 accessPackageAssignmentPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="3e0c3-123">删除 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-123">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="3e0c3-124">删除 accessPackageAssignmentPolicy。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-124">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e0c3-125">属性</span><span class="sxs-lookup"><span data-stu-id="3e0c3-125">Properties</span></span>

| <span data-ttu-id="3e0c3-126">属性</span><span class="sxs-lookup"><span data-stu-id="3e0c3-126">Property</span></span>     | <span data-ttu-id="3e0c3-127">类型</span><span class="sxs-lookup"><span data-stu-id="3e0c3-127">Type</span></span>        | <span data-ttu-id="3e0c3-128">说明</span><span class="sxs-lookup"><span data-stu-id="3e0c3-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e0c3-129">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="3e0c3-129">accessPackageId</span></span>|<span data-ttu-id="3e0c3-130">String</span><span class="sxs-lookup"><span data-stu-id="3e0c3-130">String</span></span>|<span data-ttu-id="3e0c3-131">访问包的 ID。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-131">ID of the access package.</span></span>|
|<span data-ttu-id="3e0c3-132">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="3e0c3-132">accessReviewSettings</span></span>|[<span data-ttu-id="3e0c3-133">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="3e0c3-133">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="3e0c3-134">必须对此策略中的访问包的分配以及这些工作分配的频率。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-134">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="3e0c3-135">如果不需要进行审核，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-135">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="3e0c3-136">canExtend</span><span class="sxs-lookup"><span data-stu-id="3e0c3-136">canExtend</span></span>|<span data-ttu-id="3e0c3-137">布尔</span><span class="sxs-lookup"><span data-stu-id="3e0c3-137">Boolean</span></span>|<span data-ttu-id="3e0c3-138">指示用户是否可以在批准后扩展访问包分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-138">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="3e0c3-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-139">createdBy</span></span>|<span data-ttu-id="3e0c3-140">String</span><span class="sxs-lookup"><span data-stu-id="3e0c3-140">String</span></span>|<span data-ttu-id="3e0c3-141">只读。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-141">Read-only.</span></span>|
|<span data-ttu-id="3e0c3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e0c3-142">createdDateTime</span></span>|<span data-ttu-id="3e0c3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e0c3-143">DateTimeOffset</span></span>|<span data-ttu-id="3e0c3-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e0c3-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e0c3-146">说明</span><span class="sxs-lookup"><span data-stu-id="3e0c3-146">description</span></span>|<span data-ttu-id="3e0c3-147">String</span><span class="sxs-lookup"><span data-stu-id="3e0c3-147">String</span></span>|<span data-ttu-id="3e0c3-148">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-148">The description of the policy.</span></span>|
|<span data-ttu-id="3e0c3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="3e0c3-149">displayName</span></span>|<span data-ttu-id="3e0c3-150">String</span><span class="sxs-lookup"><span data-stu-id="3e0c3-150">String</span></span>|<span data-ttu-id="3e0c3-151">策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-151">The display name of the policy.</span></span>|
|<span data-ttu-id="3e0c3-152">durationInDays</span><span class="sxs-lookup"><span data-stu-id="3e0c3-152">durationInDays</span></span>|<span data-ttu-id="3e0c3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3e0c3-153">Int32</span></span>|<span data-ttu-id="3e0c3-154">此策略中的工作分配在过期之前持续的天数。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-154">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="3e0c3-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3e0c3-155">expirationDateTime</span></span>|<span data-ttu-id="3e0c3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e0c3-156">DateTimeOffset</span></span>|<span data-ttu-id="3e0c3-157">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-157">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="3e0c3-158">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3e0c3-159">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e0c3-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e0c3-160">id</span><span class="sxs-lookup"><span data-stu-id="3e0c3-160">id</span></span>|<span data-ttu-id="3e0c3-161">字符串</span><span class="sxs-lookup"><span data-stu-id="3e0c3-161">String</span></span>| <span data-ttu-id="3e0c3-162">只读。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-162">Read-only.</span></span>|
|<span data-ttu-id="3e0c3-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="3e0c3-163">modifiedBy</span></span>|<span data-ttu-id="3e0c3-164">String</span><span class="sxs-lookup"><span data-stu-id="3e0c3-164">String</span></span>|<span data-ttu-id="3e0c3-165">只读。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-165">Read-only.</span></span>|
|<span data-ttu-id="3e0c3-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e0c3-166">modifiedDateTime</span></span>|<span data-ttu-id="3e0c3-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e0c3-167">DateTimeOffset</span></span>|<span data-ttu-id="3e0c3-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e0c3-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e0c3-170">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="3e0c3-170">requestApprovalSettings</span></span>|[<span data-ttu-id="3e0c3-171">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="3e0c3-171">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="3e0c3-172">必须在此策略中批准访问包的请求。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-172">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="3e0c3-173">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="3e0c3-173">requestorSettings</span></span>|[<span data-ttu-id="3e0c3-174">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="3e0c3-174">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="3e0c3-175">可从该策略请求此访问包的人。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-175">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3e0c3-176">关系</span><span class="sxs-lookup"><span data-stu-id="3e0c3-176">Relationships</span></span>

| <span data-ttu-id="3e0c3-177">关系</span><span class="sxs-lookup"><span data-stu-id="3e0c3-177">Relationship</span></span> | <span data-ttu-id="3e0c3-178">类型</span><span class="sxs-lookup"><span data-stu-id="3e0c3-178">Type</span></span>        | <span data-ttu-id="3e0c3-179">说明</span><span class="sxs-lookup"><span data-stu-id="3e0c3-179">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e0c3-180">accessPackage</span><span class="sxs-lookup"><span data-stu-id="3e0c3-180">accessPackage</span></span>|[<span data-ttu-id="3e0c3-181">accessPackage</span><span class="sxs-lookup"><span data-stu-id="3e0c3-181">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="3e0c3-182">具有此策略的访问包。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-182">The access package with this policy.</span></span> <span data-ttu-id="3e0c3-183">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-183">Read-only.</span></span> <span data-ttu-id="3e0c3-184">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e0c3-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e0c3-185">JSON representation</span></span>

<span data-ttu-id="3e0c3-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e0c3-186">The following is a JSON representation of the resource.</span></span>

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
