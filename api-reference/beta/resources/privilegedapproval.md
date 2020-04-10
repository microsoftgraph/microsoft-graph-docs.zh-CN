---
title: privilegedApproval 资源类型
description: 表示在用于获取角色的特权标识管理中请求的审批。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c4148e5740c9b31368be336a615524ced426a560
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219226"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="bcf77-103">privilegedApproval 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcf77-103">privilegedApproval resource type</span></span>

<span data-ttu-id="bcf77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcf77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf77-105">表示在用于获取角色的特权标识管理中请求的审批。</span><span class="sxs-lookup"><span data-stu-id="bcf77-105">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="bcf77-106">Methods</span><span class="sxs-lookup"><span data-stu-id="bcf77-106">Methods</span></span>

| <span data-ttu-id="bcf77-107">方法</span><span class="sxs-lookup"><span data-stu-id="bcf77-107">Method</span></span>           | <span data-ttu-id="bcf77-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bcf77-108">Return Type</span></span>    |<span data-ttu-id="bcf77-109">说明</span><span class="sxs-lookup"><span data-stu-id="bcf77-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bcf77-110">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-110">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="bcf77-111">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-111">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="bcf77-112">读取 privilegedApproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bcf77-112">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="bcf77-113">列出 privilegedApproval 对象</span><span class="sxs-lookup"><span data-stu-id="bcf77-113">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="bcf77-114">[privilegedApproval](privilegedapproval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bcf77-114">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="bcf77-115">获取 privilegedApproval 的集合。</span><span class="sxs-lookup"><span data-stu-id="bcf77-115">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="bcf77-116">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-116">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="bcf77-117">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-117">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="bcf77-118">创建 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="bcf77-118">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="bcf77-119">更新 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-119">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="bcf77-120">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-120">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="bcf77-121">更新 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="bcf77-121">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="bcf77-122">Myrequests</span><span class="sxs-lookup"><span data-stu-id="bcf77-122">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="bcf77-123">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="bcf77-123">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="bcf77-124">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="bcf77-124">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcf77-125">属性</span><span class="sxs-lookup"><span data-stu-id="bcf77-125">Properties</span></span>
| <span data-ttu-id="bcf77-126">属性</span><span class="sxs-lookup"><span data-stu-id="bcf77-126">Property</span></span>     | <span data-ttu-id="bcf77-127">类型</span><span class="sxs-lookup"><span data-stu-id="bcf77-127">Type</span></span>   |<span data-ttu-id="bcf77-128">说明</span><span class="sxs-lookup"><span data-stu-id="bcf77-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcf77-129">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="bcf77-129">approvalDuration</span></span>|<span data-ttu-id="bcf77-130">持续时间</span><span class="sxs-lookup"><span data-stu-id="bcf77-130">Duration</span></span>||
|<span data-ttu-id="bcf77-131">approvalState</span><span class="sxs-lookup"><span data-stu-id="bcf77-131">approvalState</span></span>|<span data-ttu-id="bcf77-132">string</span><span class="sxs-lookup"><span data-stu-id="bcf77-132">string</span></span>| <span data-ttu-id="bcf77-133">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="bcf77-133">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="bcf77-134">approvalType</span><span class="sxs-lookup"><span data-stu-id="bcf77-134">approvalType</span></span>|<span data-ttu-id="bcf77-135">字符串</span><span class="sxs-lookup"><span data-stu-id="bcf77-135">String</span></span>||
|<span data-ttu-id="bcf77-136">approverReason</span><span class="sxs-lookup"><span data-stu-id="bcf77-136">approverReason</span></span>|<span data-ttu-id="bcf77-137">字符串</span><span class="sxs-lookup"><span data-stu-id="bcf77-137">String</span></span>||
|<span data-ttu-id="bcf77-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bcf77-138">endDateTime</span></span>|<span data-ttu-id="bcf77-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcf77-139">DateTimeOffset</span></span>|<span data-ttu-id="bcf77-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bcf77-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcf77-142">id</span><span class="sxs-lookup"><span data-stu-id="bcf77-142">id</span></span>|<span data-ttu-id="bcf77-143">字符串</span><span class="sxs-lookup"><span data-stu-id="bcf77-143">String</span></span>| <span data-ttu-id="bcf77-144">只读。</span><span class="sxs-lookup"><span data-stu-id="bcf77-144">Read-only.</span></span>|
|<span data-ttu-id="bcf77-145">requestorReason</span><span class="sxs-lookup"><span data-stu-id="bcf77-145">requestorReason</span></span>|<span data-ttu-id="bcf77-146">字符串</span><span class="sxs-lookup"><span data-stu-id="bcf77-146">String</span></span>||
|<span data-ttu-id="bcf77-147">roleId</span><span class="sxs-lookup"><span data-stu-id="bcf77-147">roleId</span></span>|<span data-ttu-id="bcf77-148">字符串</span><span class="sxs-lookup"><span data-stu-id="bcf77-148">String</span></span>||
|<span data-ttu-id="bcf77-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bcf77-149">startDateTime</span></span>|<span data-ttu-id="bcf77-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcf77-150">DateTimeOffset</span></span>|<span data-ttu-id="bcf77-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bcf77-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcf77-153">userId</span><span class="sxs-lookup"><span data-stu-id="bcf77-153">userId</span></span>|<span data-ttu-id="bcf77-154">String</span><span class="sxs-lookup"><span data-stu-id="bcf77-154">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="bcf77-155">关系</span><span class="sxs-lookup"><span data-stu-id="bcf77-155">Relationships</span></span>
| <span data-ttu-id="bcf77-156">关系</span><span class="sxs-lookup"><span data-stu-id="bcf77-156">Relationship</span></span> | <span data-ttu-id="bcf77-157">类型</span><span class="sxs-lookup"><span data-stu-id="bcf77-157">Type</span></span>   |<span data-ttu-id="bcf77-158">说明</span><span class="sxs-lookup"><span data-stu-id="bcf77-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcf77-159">roleInfo</span><span class="sxs-lookup"><span data-stu-id="bcf77-159">roleInfo</span></span>|[<span data-ttu-id="bcf77-160">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="bcf77-160">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="bcf77-161">只读。</span><span class="sxs-lookup"><span data-stu-id="bcf77-161">Read-only.</span></span> <span data-ttu-id="bcf77-162">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="bcf77-162">Nullable.</span></span>|
|<span data-ttu-id="bcf77-163">申请</span><span class="sxs-lookup"><span data-stu-id="bcf77-163">request</span></span>|[<span data-ttu-id="bcf77-164">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="bcf77-164">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="bcf77-165">只读。</span><span class="sxs-lookup"><span data-stu-id="bcf77-165">Read-only.</span></span> <span data-ttu-id="bcf77-166">此审批对象的角色分配请求</span><span class="sxs-lookup"><span data-stu-id="bcf77-166">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcf77-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcf77-167">JSON representation</span></span>
<span data-ttu-id="bcf77-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcf77-168">Here is a JSON representation of the resource.</span></span>

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
