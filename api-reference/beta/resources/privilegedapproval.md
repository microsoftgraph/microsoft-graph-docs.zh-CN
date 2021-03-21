---
title: privilegedApproval 资源类型
description: 表示 Privileged Identity Management 中请求进入角色的审批。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8d092d6c877f9fa2bdce2d645ef56a84508c510d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962586"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="d8a7a-103">privilegedApproval 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8a7a-103">privilegedApproval resource type</span></span>

<span data-ttu-id="d8a7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8a7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8a7a-105">表示 Privileged Identity Management 中请求进入角色的审批。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="d8a7a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="d8a7a-106">Methods</span></span>

| <span data-ttu-id="d8a7a-107">方法</span><span class="sxs-lookup"><span data-stu-id="d8a7a-107">Method</span></span>           | <span data-ttu-id="d8a7a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8a7a-108">Return Type</span></span>    |<span data-ttu-id="d8a7a-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8a7a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a7a-110">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="d8a7a-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="d8a7a-112">读取 privilegedApproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="d8a7a-113">列出 privilegedApproval 对象</span><span class="sxs-lookup"><span data-stu-id="d8a7a-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="d8a7a-114">[privilegedApproval](privilegedapproval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8a7a-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="d8a7a-115">获取 privilegedApproval 的集合。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="d8a7a-116">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="d8a7a-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="d8a7a-118">创建 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="d8a7a-119">更新 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="d8a7a-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="d8a7a-121">更新 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="d8a7a-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="d8a7a-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="d8a7a-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d8a7a-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="d8a7a-124">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a7a-125">属性</span><span class="sxs-lookup"><span data-stu-id="d8a7a-125">Properties</span></span>
| <span data-ttu-id="d8a7a-126">属性</span><span class="sxs-lookup"><span data-stu-id="d8a7a-126">Property</span></span>     | <span data-ttu-id="d8a7a-127">类型</span><span class="sxs-lookup"><span data-stu-id="d8a7a-127">Type</span></span>   |<span data-ttu-id="d8a7a-128">说明</span><span class="sxs-lookup"><span data-stu-id="d8a7a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a7a-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="d8a7a-129">approvalDuration</span></span>|<span data-ttu-id="d8a7a-130">持续时间</span><span class="sxs-lookup"><span data-stu-id="d8a7a-130">Duration</span></span>||
|<span data-ttu-id="d8a7a-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="d8a7a-131">approvalState</span></span>|<span data-ttu-id="d8a7a-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="d8a7a-132">approvalState</span></span>| <span data-ttu-id="d8a7a-133">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="d8a7a-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="d8a7a-134">approvalType</span></span>|<span data-ttu-id="d8a7a-135">String</span><span class="sxs-lookup"><span data-stu-id="d8a7a-135">String</span></span>||
|<span data-ttu-id="d8a7a-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="d8a7a-136">approverReason</span></span>|<span data-ttu-id="d8a7a-137">String</span><span class="sxs-lookup"><span data-stu-id="d8a7a-137">String</span></span>||
|<span data-ttu-id="d8a7a-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a7a-138">endDateTime</span></span>|<span data-ttu-id="d8a7a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a7a-139">DateTimeOffset</span></span>|<span data-ttu-id="d8a7a-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8a7a-141">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d8a7a-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d8a7a-142">id</span><span class="sxs-lookup"><span data-stu-id="d8a7a-142">id</span></span>|<span data-ttu-id="d8a7a-143">String</span><span class="sxs-lookup"><span data-stu-id="d8a7a-143">String</span></span>| <span data-ttu-id="d8a7a-144">只读。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-144">Read-only.</span></span>|
|<span data-ttu-id="d8a7a-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="d8a7a-145">requestorReason</span></span>|<span data-ttu-id="d8a7a-146">String</span><span class="sxs-lookup"><span data-stu-id="d8a7a-146">String</span></span>||
|<span data-ttu-id="d8a7a-147">roleId</span><span class="sxs-lookup"><span data-stu-id="d8a7a-147">roleId</span></span>|<span data-ttu-id="d8a7a-148">String</span><span class="sxs-lookup"><span data-stu-id="d8a7a-148">String</span></span>||
|<span data-ttu-id="d8a7a-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a7a-149">startDateTime</span></span>|<span data-ttu-id="d8a7a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a7a-150">DateTimeOffset</span></span>|<span data-ttu-id="d8a7a-151">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8a7a-152">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d8a7a-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d8a7a-153">userId</span><span class="sxs-lookup"><span data-stu-id="d8a7a-153">userId</span></span>|<span data-ttu-id="d8a7a-154">String</span><span class="sxs-lookup"><span data-stu-id="d8a7a-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="d8a7a-155">关系</span><span class="sxs-lookup"><span data-stu-id="d8a7a-155">Relationships</span></span>
| <span data-ttu-id="d8a7a-156">关系</span><span class="sxs-lookup"><span data-stu-id="d8a7a-156">Relationship</span></span> | <span data-ttu-id="d8a7a-157">类型</span><span class="sxs-lookup"><span data-stu-id="d8a7a-157">Type</span></span>   |<span data-ttu-id="d8a7a-158">说明</span><span class="sxs-lookup"><span data-stu-id="d8a7a-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a7a-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="d8a7a-159">roleInfo</span></span>|[<span data-ttu-id="d8a7a-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d8a7a-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="d8a7a-161">只读。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-161">Read-only.</span></span> <span data-ttu-id="d8a7a-162">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-162">Nullable.</span></span>|
|<span data-ttu-id="d8a7a-163">request</span><span class="sxs-lookup"><span data-stu-id="d8a7a-163">request</span></span>|[<span data-ttu-id="d8a7a-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d8a7a-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="d8a7a-165">只读。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-165">Read-only.</span></span> <span data-ttu-id="d8a7a-166">此角色分配对象的请求</span><span class="sxs-lookup"><span data-stu-id="d8a7a-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8a7a-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8a7a-167">JSON representation</span></span>
<span data-ttu-id="d8a7a-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8a7a-168">Here is a JSON representation of the resource.</span></span>

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


