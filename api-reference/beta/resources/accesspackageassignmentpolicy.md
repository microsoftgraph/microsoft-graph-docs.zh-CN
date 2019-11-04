---
title: accessPackageAssignmentPolicy 资源类型
description: 访问包分配策略指定使用者可以通过访问包分配请求或分配访问包的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: acb7c7b355d2a03d78cad1127882f272135fc4a2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939206"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="df173-103">accessPackageAssignmentPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="df173-103">accessPackageAssignmentPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df173-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配策略指定了主题可以通过访问包分配请求或分配访问包的策略。</span><span class="sxs-lookup"><span data-stu-id="df173-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="df173-105">访问包可以有零个或多个策略。</span><span class="sxs-lookup"><span data-stu-id="df173-105">An access package can have zero or more policies.</span></span> <span data-ttu-id="df173-106">收到来自接受者的请求时，主题将与每个策略相匹配，以查找该主题的策略（如果有）。</span><span class="sxs-lookup"><span data-stu-id="df173-106">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) for that subject.</span></span> <span data-ttu-id="df173-107">然后，该策略将确定请求是否需要审批以及访问包分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="df173-107">The policy then determines whether the request requires approval, and the duration of the access package assignment.</span></span>

<span data-ttu-id="df173-108">若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="df173-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="df173-109">方法</span><span class="sxs-lookup"><span data-stu-id="df173-109">Methods</span></span>

| <span data-ttu-id="df173-110">方法</span><span class="sxs-lookup"><span data-stu-id="df173-110">Method</span></span>       | <span data-ttu-id="df173-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="df173-111">Return Type</span></span> | <span data-ttu-id="df173-112">说明</span><span class="sxs-lookup"><span data-stu-id="df173-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="df173-113">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="df173-113">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="df173-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="df173-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="df173-115">检索 accessPackageAssignmentPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="df173-115">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="df173-116">创建 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="df173-116">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="df173-117">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="df173-117">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="df173-118">创建新的 accessPackageAssignmentPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="df173-118">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="df173-119">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="df173-119">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="df173-120">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="df173-120">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="df173-121">读取 accessPackageAssignmentPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df173-121">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="df173-122">删除 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="df173-122">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="df173-123">删除 accessPackageAssignmentPolicy。</span><span class="sxs-lookup"><span data-stu-id="df173-123">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="df173-124">属性</span><span class="sxs-lookup"><span data-stu-id="df173-124">Properties</span></span>

| <span data-ttu-id="df173-125">属性</span><span class="sxs-lookup"><span data-stu-id="df173-125">Property</span></span>     | <span data-ttu-id="df173-126">类型</span><span class="sxs-lookup"><span data-stu-id="df173-126">Type</span></span>        | <span data-ttu-id="df173-127">描述</span><span class="sxs-lookup"><span data-stu-id="df173-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df173-128">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="df173-128">accessPackageId</span></span>|<span data-ttu-id="df173-129">字符串</span><span class="sxs-lookup"><span data-stu-id="df173-129">String</span></span>|<span data-ttu-id="df173-130">访问包的 ID。</span><span class="sxs-lookup"><span data-stu-id="df173-130">ID of the access package.</span></span>|
|<span data-ttu-id="df173-131">canExtend</span><span class="sxs-lookup"><span data-stu-id="df173-131">canExtend</span></span>|<span data-ttu-id="df173-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="df173-132">Boolean</span></span>|<span data-ttu-id="df173-133">指示用户是否可以在批准后扩展访问包分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="df173-133">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="df173-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="df173-134">createdBy</span></span>|<span data-ttu-id="df173-135">字符串</span><span class="sxs-lookup"><span data-stu-id="df173-135">String</span></span>|<span data-ttu-id="df173-136">只读。</span><span class="sxs-lookup"><span data-stu-id="df173-136">Read-only.</span></span>|
|<span data-ttu-id="df173-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df173-137">createdDateTime</span></span>|<span data-ttu-id="df173-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df173-138">DateTimeOffset</span></span>|<span data-ttu-id="df173-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="df173-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="df173-141">description</span><span class="sxs-lookup"><span data-stu-id="df173-141">description</span></span>|<span data-ttu-id="df173-142">String</span><span class="sxs-lookup"><span data-stu-id="df173-142">String</span></span>|<span data-ttu-id="df173-143">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="df173-143">The description of the policy.</span></span>|
|<span data-ttu-id="df173-144">displayName</span><span class="sxs-lookup"><span data-stu-id="df173-144">displayName</span></span>|<span data-ttu-id="df173-145">String</span><span class="sxs-lookup"><span data-stu-id="df173-145">String</span></span>|<span data-ttu-id="df173-146">策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="df173-146">The display name of the policy.</span></span>|
|<span data-ttu-id="df173-147">durationInDays</span><span class="sxs-lookup"><span data-stu-id="df173-147">durationInDays</span></span>|<span data-ttu-id="df173-148">Int32</span><span class="sxs-lookup"><span data-stu-id="df173-148">Int32</span></span>|<span data-ttu-id="df173-149">此策略中的工作分配在过期之前持续的天数。</span><span class="sxs-lookup"><span data-stu-id="df173-149">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="df173-150">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="df173-150">expirationDateTime</span></span>|<span data-ttu-id="df173-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df173-151">DateTimeOffset</span></span>|<span data-ttu-id="df173-152">在此策略中创建的工作分配的到期日期。</span><span class="sxs-lookup"><span data-stu-id="df173-152">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="df173-153">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="df173-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="df173-154">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="df173-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="df173-155">id</span><span class="sxs-lookup"><span data-stu-id="df173-155">id</span></span>|<span data-ttu-id="df173-156">字符串</span><span class="sxs-lookup"><span data-stu-id="df173-156">String</span></span>| <span data-ttu-id="df173-157">只读。</span><span class="sxs-lookup"><span data-stu-id="df173-157">Read-only.</span></span>|
|<span data-ttu-id="df173-158">isEnabled</span><span class="sxs-lookup"><span data-stu-id="df173-158">isEnabled</span></span>|<span data-ttu-id="df173-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="df173-159">Boolean</span></span>|<span data-ttu-id="df173-160">可以将此策略用于新的请求。</span><span class="sxs-lookup"><span data-stu-id="df173-160">Can this policy be used for new requests.</span></span>|
|<span data-ttu-id="df173-161">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="df173-161">modifiedBy</span></span>|<span data-ttu-id="df173-162">字符串</span><span class="sxs-lookup"><span data-stu-id="df173-162">String</span></span>|<span data-ttu-id="df173-163">只读。</span><span class="sxs-lookup"><span data-stu-id="df173-163">Read-only.</span></span>|
|<span data-ttu-id="df173-164">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df173-164">modifiedDateTime</span></span>|<span data-ttu-id="df173-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df173-165">DateTimeOffset</span></span>|<span data-ttu-id="df173-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="df173-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="df173-168">关系</span><span class="sxs-lookup"><span data-stu-id="df173-168">Relationships</span></span>

| <span data-ttu-id="df173-169">关系</span><span class="sxs-lookup"><span data-stu-id="df173-169">Relationship</span></span> | <span data-ttu-id="df173-170">类型</span><span class="sxs-lookup"><span data-stu-id="df173-170">Type</span></span>        | <span data-ttu-id="df173-171">描述</span><span class="sxs-lookup"><span data-stu-id="df173-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df173-172">accessPackage</span><span class="sxs-lookup"><span data-stu-id="df173-172">accessPackage</span></span>|[<span data-ttu-id="df173-173">accessPackage</span><span class="sxs-lookup"><span data-stu-id="df173-173">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="df173-174">具有此策略的访问包。</span><span class="sxs-lookup"><span data-stu-id="df173-174">The access package with this policy.</span></span> <span data-ttu-id="df173-175">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="df173-175">Read-only.</span></span> <span data-ttu-id="df173-176">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="df173-176">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df173-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df173-177">JSON representation</span></span>

<span data-ttu-id="df173-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df173-178">The following is a JSON representation of the resource.</span></span>

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
    "isEnabled": false,
    "canExtend": false,
    "durationInDays": 365
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
