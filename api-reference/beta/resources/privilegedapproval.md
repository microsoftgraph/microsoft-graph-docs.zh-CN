---
title: privilegedApproval 资源类型
description: 表示在用于获取角色的特权标识管理中请求的审批。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: cd6f352ad114307933682f4d6df22408b54ebc73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070581"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="03a53-103">privilegedApproval 资源类型</span><span class="sxs-lookup"><span data-stu-id="03a53-103">privilegedApproval resource type</span></span>

<span data-ttu-id="03a53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03a53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a53-105">表示在用于获取角色的特权标识管理中请求的审批。</span><span class="sxs-lookup"><span data-stu-id="03a53-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="03a53-106">方法</span><span class="sxs-lookup"><span data-stu-id="03a53-106">Methods</span></span>

| <span data-ttu-id="03a53-107">方法</span><span class="sxs-lookup"><span data-stu-id="03a53-107">Method</span></span>           | <span data-ttu-id="03a53-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="03a53-108">Return Type</span></span>    |<span data-ttu-id="03a53-109">说明</span><span class="sxs-lookup"><span data-stu-id="03a53-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03a53-110">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="03a53-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="03a53-112">读取 privilegedApproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03a53-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="03a53-113">列出 privilegedApproval 对象</span><span class="sxs-lookup"><span data-stu-id="03a53-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="03a53-114">[privilegedApproval](privilegedapproval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03a53-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="03a53-115">获取 privilegedApproval 的集合。</span><span class="sxs-lookup"><span data-stu-id="03a53-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="03a53-116">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="03a53-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="03a53-118">创建 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="03a53-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="03a53-119">更新 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="03a53-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="03a53-121">更新 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="03a53-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="03a53-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="03a53-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="03a53-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="03a53-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="03a53-124">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="03a53-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="03a53-125">属性</span><span class="sxs-lookup"><span data-stu-id="03a53-125">Properties</span></span>
| <span data-ttu-id="03a53-126">属性</span><span class="sxs-lookup"><span data-stu-id="03a53-126">Property</span></span>     | <span data-ttu-id="03a53-127">类型</span><span class="sxs-lookup"><span data-stu-id="03a53-127">Type</span></span>   |<span data-ttu-id="03a53-128">说明</span><span class="sxs-lookup"><span data-stu-id="03a53-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03a53-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="03a53-129">approvalDuration</span></span>|<span data-ttu-id="03a53-130">持续时间</span><span class="sxs-lookup"><span data-stu-id="03a53-130">Duration</span></span>||
|<span data-ttu-id="03a53-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="03a53-131">approvalState</span></span>|<span data-ttu-id="03a53-132">string</span><span class="sxs-lookup"><span data-stu-id="03a53-132">string</span></span>| <span data-ttu-id="03a53-133">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="03a53-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="03a53-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="03a53-134">approvalType</span></span>|<span data-ttu-id="03a53-135">String</span><span class="sxs-lookup"><span data-stu-id="03a53-135">String</span></span>||
|<span data-ttu-id="03a53-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="03a53-136">approverReason</span></span>|<span data-ttu-id="03a53-137">String</span><span class="sxs-lookup"><span data-stu-id="03a53-137">String</span></span>||
|<span data-ttu-id="03a53-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="03a53-138">endDateTime</span></span>|<span data-ttu-id="03a53-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03a53-139">DateTimeOffset</span></span>|<span data-ttu-id="03a53-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="03a53-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="03a53-142">id</span><span class="sxs-lookup"><span data-stu-id="03a53-142">id</span></span>|<span data-ttu-id="03a53-143">String</span><span class="sxs-lookup"><span data-stu-id="03a53-143">String</span></span>| <span data-ttu-id="03a53-144">只读。</span><span class="sxs-lookup"><span data-stu-id="03a53-144">Read-only.</span></span>|
|<span data-ttu-id="03a53-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="03a53-145">requestorReason</span></span>|<span data-ttu-id="03a53-146">String</span><span class="sxs-lookup"><span data-stu-id="03a53-146">String</span></span>||
|<span data-ttu-id="03a53-147">roleId</span><span class="sxs-lookup"><span data-stu-id="03a53-147">roleId</span></span>|<span data-ttu-id="03a53-148">String</span><span class="sxs-lookup"><span data-stu-id="03a53-148">String</span></span>||
|<span data-ttu-id="03a53-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="03a53-149">startDateTime</span></span>|<span data-ttu-id="03a53-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03a53-150">DateTimeOffset</span></span>|<span data-ttu-id="03a53-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="03a53-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="03a53-153">userId</span><span class="sxs-lookup"><span data-stu-id="03a53-153">userId</span></span>|<span data-ttu-id="03a53-154">String</span><span class="sxs-lookup"><span data-stu-id="03a53-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="03a53-155">关系</span><span class="sxs-lookup"><span data-stu-id="03a53-155">Relationships</span></span>
| <span data-ttu-id="03a53-156">关系</span><span class="sxs-lookup"><span data-stu-id="03a53-156">Relationship</span></span> | <span data-ttu-id="03a53-157">类型</span><span class="sxs-lookup"><span data-stu-id="03a53-157">Type</span></span>   |<span data-ttu-id="03a53-158">说明</span><span class="sxs-lookup"><span data-stu-id="03a53-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03a53-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="03a53-159">roleInfo</span></span>|[<span data-ttu-id="03a53-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="03a53-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="03a53-161">只读。</span><span class="sxs-lookup"><span data-stu-id="03a53-161">Read-only.</span></span> <span data-ttu-id="03a53-162">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="03a53-162">Nullable.</span></span>|
|<span data-ttu-id="03a53-163">申请</span><span class="sxs-lookup"><span data-stu-id="03a53-163">request</span></span>|[<span data-ttu-id="03a53-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="03a53-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="03a53-165">只读。</span><span class="sxs-lookup"><span data-stu-id="03a53-165">Read-only.</span></span> <span data-ttu-id="03a53-166">此审批对象的角色分配请求</span><span class="sxs-lookup"><span data-stu-id="03a53-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03a53-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03a53-167">JSON representation</span></span>
<span data-ttu-id="03a53-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03a53-168">Here is a JSON representation of the resource.</span></span>

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


