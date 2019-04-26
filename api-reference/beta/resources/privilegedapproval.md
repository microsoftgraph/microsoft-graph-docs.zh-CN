---
title: privilegedApproval 资源类型
description: 表示在用于获取角色的特权标识管理中请求的审批。
localization_priority: Normal
ms.openlocfilehash: 754fcd9b61321db1675408172c945557e38dc0e0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344216"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="7d922-103">privilegedApproval 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d922-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d922-104">表示在用于获取角色的特权标识管理中请求的审批。</span><span class="sxs-lookup"><span data-stu-id="7d922-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="7d922-105">方法</span><span class="sxs-lookup"><span data-stu-id="7d922-105">Methods</span></span>

| <span data-ttu-id="7d922-106">方法</span><span class="sxs-lookup"><span data-stu-id="7d922-106">Method</span></span>           | <span data-ttu-id="7d922-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d922-107">Return Type</span></span>    |<span data-ttu-id="7d922-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d922-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d922-109">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="7d922-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="7d922-111">读取 privilegedApproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d922-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="7d922-112">列出 privilegedApproval 对象</span><span class="sxs-lookup"><span data-stu-id="7d922-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="7d922-113">[privilegedApproval](privilegedapproval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7d922-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="7d922-114">获取 privilegedApproval 的集合。</span><span class="sxs-lookup"><span data-stu-id="7d922-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="7d922-115">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="7d922-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="7d922-117">创建 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="7d922-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="7d922-118">更新 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="7d922-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="7d922-120">更新 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="7d922-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="7d922-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="7d922-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="7d922-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d922-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="7d922-123">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="7d922-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d922-124">属性</span><span class="sxs-lookup"><span data-stu-id="7d922-124">Properties</span></span>
| <span data-ttu-id="7d922-125">属性</span><span class="sxs-lookup"><span data-stu-id="7d922-125">Property</span></span>     | <span data-ttu-id="7d922-126">类型</span><span class="sxs-lookup"><span data-stu-id="7d922-126">Type</span></span>   |<span data-ttu-id="7d922-127">说明</span><span class="sxs-lookup"><span data-stu-id="7d922-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d922-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="7d922-128">approvalDuration</span></span>|<span data-ttu-id="7d922-129">持续时间</span><span class="sxs-lookup"><span data-stu-id="7d922-129">Duration</span></span>||
|<span data-ttu-id="7d922-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="7d922-130">approvalState</span></span>|<span data-ttu-id="7d922-131">string</span><span class="sxs-lookup"><span data-stu-id="7d922-131">string</span></span>| <span data-ttu-id="7d922-132">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="7d922-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="7d922-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="7d922-133">approvalType</span></span>|<span data-ttu-id="7d922-134">String</span><span class="sxs-lookup"><span data-stu-id="7d922-134">String</span></span>||
|<span data-ttu-id="7d922-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="7d922-135">approverReason</span></span>|<span data-ttu-id="7d922-136">String</span><span class="sxs-lookup"><span data-stu-id="7d922-136">String</span></span>||
|<span data-ttu-id="7d922-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7d922-137">endDateTime</span></span>|<span data-ttu-id="7d922-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d922-138">DateTimeOffset</span></span>|<span data-ttu-id="7d922-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7d922-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7d922-141">id</span><span class="sxs-lookup"><span data-stu-id="7d922-141">id</span></span>|<span data-ttu-id="7d922-142">String</span><span class="sxs-lookup"><span data-stu-id="7d922-142">String</span></span>| <span data-ttu-id="7d922-143">只读。</span><span class="sxs-lookup"><span data-stu-id="7d922-143">Read-only.</span></span>|
|<span data-ttu-id="7d922-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="7d922-144">requestorReason</span></span>|<span data-ttu-id="7d922-145">String</span><span class="sxs-lookup"><span data-stu-id="7d922-145">String</span></span>||
|<span data-ttu-id="7d922-146">roleId</span><span class="sxs-lookup"><span data-stu-id="7d922-146">roleId</span></span>|<span data-ttu-id="7d922-147">String</span><span class="sxs-lookup"><span data-stu-id="7d922-147">String</span></span>||
|<span data-ttu-id="7d922-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7d922-148">startDateTime</span></span>|<span data-ttu-id="7d922-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d922-149">DateTimeOffset</span></span>|<span data-ttu-id="7d922-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7d922-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7d922-152">userId</span><span class="sxs-lookup"><span data-stu-id="7d922-152">userId</span></span>|<span data-ttu-id="7d922-153">String</span><span class="sxs-lookup"><span data-stu-id="7d922-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="7d922-154">关系</span><span class="sxs-lookup"><span data-stu-id="7d922-154">Relationships</span></span>
| <span data-ttu-id="7d922-155">关系</span><span class="sxs-lookup"><span data-stu-id="7d922-155">Relationship</span></span> | <span data-ttu-id="7d922-156">类型</span><span class="sxs-lookup"><span data-stu-id="7d922-156">Type</span></span>   |<span data-ttu-id="7d922-157">说明</span><span class="sxs-lookup"><span data-stu-id="7d922-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d922-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="7d922-158">roleInfo</span></span>|[<span data-ttu-id="7d922-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="7d922-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="7d922-160">只读。</span><span class="sxs-lookup"><span data-stu-id="7d922-160">Read-only.</span></span> <span data-ttu-id="7d922-161">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7d922-161">Nullable.</span></span>|
|<span data-ttu-id="7d922-162">申请</span><span class="sxs-lookup"><span data-stu-id="7d922-162">request</span></span>|[<span data-ttu-id="7d922-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7d922-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="7d922-164">只读。</span><span class="sxs-lookup"><span data-stu-id="7d922-164">Read-only.</span></span> <span data-ttu-id="7d922-165">此审批对象的角色分配请求</span><span class="sxs-lookup"><span data-stu-id="7d922-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d922-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d922-166">JSON representation</span></span>
<span data-ttu-id="7d922-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d922-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
