---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定使用者可以通过访问包分配请求或分配访问包的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08fcefafe9a354a57415a7d05bee1ec57ffdc138
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331302"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="962be-103">accessPackageAssignmentPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="962be-103">accessPackageAssignmentPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="962be-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配策略指定了主题可以通过访问包分配请求或分配访问包的策略。</span><span class="sxs-lookup"><span data-stu-id="962be-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="962be-105">访问包可以有零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="962be-105">An access package can have zero or more policies.</span></span> <span data-ttu-id="962be-106">收到来自主题的请求时，主题将与每个策略相匹配，以查找包含该主题的 requestorSettings 策略（如果有）。</span><span class="sxs-lookup"><span data-stu-id="962be-106">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="962be-107">然后，该策略将确定请求是否需要审批、访问包分配的持续时间以及是否需要定期查看工作分配。</span><span class="sxs-lookup"><span data-stu-id="962be-107">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="962be-108">若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="962be-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="962be-109">Methods</span><span class="sxs-lookup"><span data-stu-id="962be-109">Methods</span></span>

| <span data-ttu-id="962be-110">方法</span><span class="sxs-lookup"><span data-stu-id="962be-110">Method</span></span>       | <span data-ttu-id="962be-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="962be-111">Return Type</span></span> | <span data-ttu-id="962be-112">说明</span><span class="sxs-lookup"><span data-stu-id="962be-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="962be-113">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="962be-113">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="962be-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="962be-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="962be-115">检索 accessPackageAssignmentPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="962be-115">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="962be-116">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="962be-116">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="962be-117">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="962be-117">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="962be-118">创建新的 accessPackageAssignmentPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="962be-118">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="962be-119">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="962be-119">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="962be-120">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="962be-120">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="962be-121">读取 accessPackageAssignmentPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="962be-121">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="962be-122">删除 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="962be-122">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="962be-123">删除 accessPackageAssignmentPolicy。</span><span class="sxs-lookup"><span data-stu-id="962be-123">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="962be-124">属性</span><span class="sxs-lookup"><span data-stu-id="962be-124">Properties</span></span>

| <span data-ttu-id="962be-125">属性</span><span class="sxs-lookup"><span data-stu-id="962be-125">Property</span></span>     | <span data-ttu-id="962be-126">类型</span><span class="sxs-lookup"><span data-stu-id="962be-126">Type</span></span>        | <span data-ttu-id="962be-127">说明</span><span class="sxs-lookup"><span data-stu-id="962be-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="962be-128">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="962be-128">accessPackageId</span></span>|<span data-ttu-id="962be-129">String</span><span class="sxs-lookup"><span data-stu-id="962be-129">String</span></span>|<span data-ttu-id="962be-130">访问包的 ID。</span><span class="sxs-lookup"><span data-stu-id="962be-130">ID of the access package.</span></span>|
|<span data-ttu-id="962be-131">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="962be-131">accessReviewSettings</span></span>|[<span data-ttu-id="962be-132">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="962be-132">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="962be-133">必须对此策略中的访问包的分配以及这些工作分配的频率。</span><span class="sxs-lookup"><span data-stu-id="962be-133">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="962be-134">如果不需要进行审核，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="962be-134">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="962be-135">canExtend</span><span class="sxs-lookup"><span data-stu-id="962be-135">canExtend</span></span>|<span data-ttu-id="962be-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="962be-136">Boolean</span></span>|<span data-ttu-id="962be-137">指示用户是否可以在批准后扩展访问包分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="962be-137">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="962be-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="962be-138">createdBy</span></span>|<span data-ttu-id="962be-139">String</span><span class="sxs-lookup"><span data-stu-id="962be-139">String</span></span>|<span data-ttu-id="962be-140">只读。</span><span class="sxs-lookup"><span data-stu-id="962be-140">Read-only.</span></span>|
|<span data-ttu-id="962be-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="962be-141">createdDateTime</span></span>|<span data-ttu-id="962be-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="962be-142">DateTimeOffset</span></span>|<span data-ttu-id="962be-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="962be-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="962be-145">说明</span><span class="sxs-lookup"><span data-stu-id="962be-145">description</span></span>|<span data-ttu-id="962be-146">String</span><span class="sxs-lookup"><span data-stu-id="962be-146">String</span></span>|<span data-ttu-id="962be-147">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="962be-147">The description of the policy.</span></span>|
|<span data-ttu-id="962be-148">displayName</span><span class="sxs-lookup"><span data-stu-id="962be-148">displayName</span></span>|<span data-ttu-id="962be-149">String</span><span class="sxs-lookup"><span data-stu-id="962be-149">String</span></span>|<span data-ttu-id="962be-150">策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="962be-150">The display name of the policy.</span></span>|
|<span data-ttu-id="962be-151">durationInDays</span><span class="sxs-lookup"><span data-stu-id="962be-151">durationInDays</span></span>|<span data-ttu-id="962be-152">Int32</span><span class="sxs-lookup"><span data-stu-id="962be-152">Int32</span></span>|<span data-ttu-id="962be-153">此策略中的工作分配在过期之前持续的天数。</span><span class="sxs-lookup"><span data-stu-id="962be-153">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="962be-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="962be-154">expirationDateTime</span></span>|<span data-ttu-id="962be-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="962be-155">DateTimeOffset</span></span>|<span data-ttu-id="962be-156">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="962be-156">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="962be-157">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="962be-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="962be-158">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="962be-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="962be-159">id</span><span class="sxs-lookup"><span data-stu-id="962be-159">id</span></span>|<span data-ttu-id="962be-160">字符串</span><span class="sxs-lookup"><span data-stu-id="962be-160">String</span></span>| <span data-ttu-id="962be-161">只读。</span><span class="sxs-lookup"><span data-stu-id="962be-161">Read-only.</span></span>|
|<span data-ttu-id="962be-162">isDenyPolicy</span><span class="sxs-lookup"><span data-stu-id="962be-162">isDenyPolicy</span></span>|<span data-ttu-id="962be-163">布尔值</span><span class="sxs-lookup"><span data-stu-id="962be-163">Boolean</span></span>|<span data-ttu-id="962be-164">如果为 true，策略将不允许访问。</span><span class="sxs-lookup"><span data-stu-id="962be-164">If true, the policy will not permit access.</span></span> <span data-ttu-id="962be-165">只读。</span><span class="sxs-lookup"><span data-stu-id="962be-165">Read only.</span></span>|
|<span data-ttu-id="962be-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="962be-166">modifiedBy</span></span>|<span data-ttu-id="962be-167">String</span><span class="sxs-lookup"><span data-stu-id="962be-167">String</span></span>|<span data-ttu-id="962be-168">只读。</span><span class="sxs-lookup"><span data-stu-id="962be-168">Read-only.</span></span>|
|<span data-ttu-id="962be-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="962be-169">modifiedDateTime</span></span>|<span data-ttu-id="962be-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="962be-170">DateTimeOffset</span></span>|<span data-ttu-id="962be-p106">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="962be-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="962be-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="962be-173">requestApprovalSettings</span></span>|[<span data-ttu-id="962be-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="962be-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="962be-175">必须在此策略中批准访问包的请求。</span><span class="sxs-lookup"><span data-stu-id="962be-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="962be-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="962be-176">requestorSettings</span></span>|[<span data-ttu-id="962be-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="962be-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="962be-178">可从该策略请求此访问包的人。</span><span class="sxs-lookup"><span data-stu-id="962be-178">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="962be-179">关系</span><span class="sxs-lookup"><span data-stu-id="962be-179">Relationships</span></span>

| <span data-ttu-id="962be-180">关系</span><span class="sxs-lookup"><span data-stu-id="962be-180">Relationship</span></span> | <span data-ttu-id="962be-181">类型</span><span class="sxs-lookup"><span data-stu-id="962be-181">Type</span></span>        | <span data-ttu-id="962be-182">说明</span><span class="sxs-lookup"><span data-stu-id="962be-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="962be-183">accessPackage</span><span class="sxs-lookup"><span data-stu-id="962be-183">accessPackage</span></span>|[<span data-ttu-id="962be-184">accessPackage</span><span class="sxs-lookup"><span data-stu-id="962be-184">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="962be-185">具有此策略的访问包。</span><span class="sxs-lookup"><span data-stu-id="962be-185">The access package with this policy.</span></span> <span data-ttu-id="962be-186">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="962be-186">Read-only.</span></span> <span data-ttu-id="962be-187">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="962be-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="962be-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="962be-188">JSON representation</span></span>

<span data-ttu-id="962be-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="962be-189">The following is a JSON representation of the resource.</span></span>

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
