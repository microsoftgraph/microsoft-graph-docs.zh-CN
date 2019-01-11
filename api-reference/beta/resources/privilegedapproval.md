---
title: privilegedApproval 资源类型
description: 代表用于获取到角色特权标识管理中请求审批。
localization_priority: Normal
ms.openlocfilehash: dee8cffba02270308c6786b2549b66aa5ad9dfa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868346"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="38e7b-103">privilegedApproval 资源类型</span><span class="sxs-lookup"><span data-stu-id="38e7b-103">privilegedApproval resource type</span></span>

> <span data-ttu-id="38e7b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38e7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38e7b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38e7b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38e7b-106">代表用于获取到角色特权标识管理中请求审批。</span><span class="sxs-lookup"><span data-stu-id="38e7b-106">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="38e7b-107">方法</span><span class="sxs-lookup"><span data-stu-id="38e7b-107">Methods</span></span>

| <span data-ttu-id="38e7b-108">方法</span><span class="sxs-lookup"><span data-stu-id="38e7b-108">Method</span></span>           | <span data-ttu-id="38e7b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="38e7b-109">Return Type</span></span>    |<span data-ttu-id="38e7b-110">说明</span><span class="sxs-lookup"><span data-stu-id="38e7b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38e7b-111">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-111">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="38e7b-112">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-112">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="38e7b-113">读取属性和 privilegedApproval 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="38e7b-113">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="38e7b-114">列表 privilegedApproval 对象</span><span class="sxs-lookup"><span data-stu-id="38e7b-114">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="38e7b-115">[privilegedApproval](privilegedapproval.md)集合</span><span class="sxs-lookup"><span data-stu-id="38e7b-115">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="38e7b-116">获取 privilegedApproval 的集合。</span><span class="sxs-lookup"><span data-stu-id="38e7b-116">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="38e7b-117">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-117">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="38e7b-118">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-118">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="38e7b-119">创建 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="38e7b-119">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="38e7b-120">更新 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-120">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="38e7b-121">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-121">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="38e7b-122">更新 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="38e7b-122">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="38e7b-123">Myrequests</span><span class="sxs-lookup"><span data-stu-id="38e7b-123">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="38e7b-124">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="38e7b-124">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="38e7b-125">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="38e7b-125">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="38e7b-126">属性</span><span class="sxs-lookup"><span data-stu-id="38e7b-126">Properties</span></span>
| <span data-ttu-id="38e7b-127">属性</span><span class="sxs-lookup"><span data-stu-id="38e7b-127">Property</span></span>     | <span data-ttu-id="38e7b-128">类型</span><span class="sxs-lookup"><span data-stu-id="38e7b-128">Type</span></span>   |<span data-ttu-id="38e7b-129">Description</span><span class="sxs-lookup"><span data-stu-id="38e7b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38e7b-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="38e7b-130">approvalDuration</span></span>|<span data-ttu-id="38e7b-131">Duration</span><span class="sxs-lookup"><span data-stu-id="38e7b-131">Duration</span></span>||
|<span data-ttu-id="38e7b-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="38e7b-132">approvalState</span></span>|<span data-ttu-id="38e7b-133">string</span><span class="sxs-lookup"><span data-stu-id="38e7b-133">string</span></span>| <span data-ttu-id="38e7b-134">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="38e7b-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="38e7b-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="38e7b-135">approvalType</span></span>|<span data-ttu-id="38e7b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="38e7b-136">String</span></span>||
|<span data-ttu-id="38e7b-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="38e7b-137">approverReason</span></span>|<span data-ttu-id="38e7b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="38e7b-138">String</span></span>||
|<span data-ttu-id="38e7b-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="38e7b-139">endDateTime</span></span>|<span data-ttu-id="38e7b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38e7b-140">DateTimeOffset</span></span>|<span data-ttu-id="38e7b-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="38e7b-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="38e7b-143">id</span><span class="sxs-lookup"><span data-stu-id="38e7b-143">id</span></span>|<span data-ttu-id="38e7b-144">String</span><span class="sxs-lookup"><span data-stu-id="38e7b-144">String</span></span>| <span data-ttu-id="38e7b-145">只读。</span><span class="sxs-lookup"><span data-stu-id="38e7b-145">Read-only.</span></span>|
|<span data-ttu-id="38e7b-146">requestorReason</span><span class="sxs-lookup"><span data-stu-id="38e7b-146">requestorReason</span></span>|<span data-ttu-id="38e7b-147">字符串</span><span class="sxs-lookup"><span data-stu-id="38e7b-147">String</span></span>||
|<span data-ttu-id="38e7b-148">roleId</span><span class="sxs-lookup"><span data-stu-id="38e7b-148">roleId</span></span>|<span data-ttu-id="38e7b-149">字符串</span><span class="sxs-lookup"><span data-stu-id="38e7b-149">String</span></span>||
|<span data-ttu-id="38e7b-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="38e7b-150">startDateTime</span></span>|<span data-ttu-id="38e7b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38e7b-151">DateTimeOffset</span></span>|<span data-ttu-id="38e7b-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="38e7b-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="38e7b-154">userId</span><span class="sxs-lookup"><span data-stu-id="38e7b-154">userId</span></span>|<span data-ttu-id="38e7b-155">String</span><span class="sxs-lookup"><span data-stu-id="38e7b-155">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="38e7b-156">Relationships</span><span class="sxs-lookup"><span data-stu-id="38e7b-156">Relationships</span></span>
| <span data-ttu-id="38e7b-157">关系</span><span class="sxs-lookup"><span data-stu-id="38e7b-157">Relationship</span></span> | <span data-ttu-id="38e7b-158">类型</span><span class="sxs-lookup"><span data-stu-id="38e7b-158">Type</span></span>   |<span data-ttu-id="38e7b-159">Description</span><span class="sxs-lookup"><span data-stu-id="38e7b-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38e7b-160">roleInfo</span><span class="sxs-lookup"><span data-stu-id="38e7b-160">roleInfo</span></span>|[<span data-ttu-id="38e7b-161">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="38e7b-161">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="38e7b-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="38e7b-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="38e7b-164">请求</span><span class="sxs-lookup"><span data-stu-id="38e7b-164">request</span></span>|[<span data-ttu-id="38e7b-165">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="38e7b-165">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="38e7b-166">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="38e7b-166">Read-only.</span></span> <span data-ttu-id="38e7b-167">对此审批对象的角色分配请求</span><span class="sxs-lookup"><span data-stu-id="38e7b-167">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38e7b-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38e7b-168">JSON representation</span></span>
<span data-ttu-id="38e7b-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38e7b-169">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
