---
title: privilegedApproval 资源类型
description: 代表用于获取到角色特权标识管理中请求审批。
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516887"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="496a7-103">privilegedApproval 资源类型</span><span class="sxs-lookup"><span data-stu-id="496a7-103">privilegedApproval resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="496a7-104">代表用于获取到角色特权标识管理中请求审批。</span><span class="sxs-lookup"><span data-stu-id="496a7-104">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="496a7-105">方法</span><span class="sxs-lookup"><span data-stu-id="496a7-105">Methods</span></span>

| <span data-ttu-id="496a7-106">方法</span><span class="sxs-lookup"><span data-stu-id="496a7-106">Method</span></span>           | <span data-ttu-id="496a7-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="496a7-107">Return Type</span></span>    |<span data-ttu-id="496a7-108">说明</span><span class="sxs-lookup"><span data-stu-id="496a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="496a7-109">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-109">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="496a7-110">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-110">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="496a7-111">读取属性和 privilegedApproval 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="496a7-111">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="496a7-112">列表 privilegedApproval 对象</span><span class="sxs-lookup"><span data-stu-id="496a7-112">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="496a7-113">[privilegedApproval](privilegedapproval.md)集合</span><span class="sxs-lookup"><span data-stu-id="496a7-113">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="496a7-114">获取 privilegedApproval 的集合。</span><span class="sxs-lookup"><span data-stu-id="496a7-114">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="496a7-115">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-115">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="496a7-116">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-116">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="496a7-117">创建 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="496a7-117">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="496a7-118">更新 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-118">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="496a7-119">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-119">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="496a7-120">更新 privilegedApproval 对象。</span><span class="sxs-lookup"><span data-stu-id="496a7-120">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="496a7-121">Myrequests</span><span class="sxs-lookup"><span data-stu-id="496a7-121">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="496a7-122">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="496a7-122">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="496a7-123">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="496a7-123">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="496a7-124">属性</span><span class="sxs-lookup"><span data-stu-id="496a7-124">Properties</span></span>
| <span data-ttu-id="496a7-125">属性</span><span class="sxs-lookup"><span data-stu-id="496a7-125">Property</span></span>     | <span data-ttu-id="496a7-126">类型</span><span class="sxs-lookup"><span data-stu-id="496a7-126">Type</span></span>   |<span data-ttu-id="496a7-127">说明</span><span class="sxs-lookup"><span data-stu-id="496a7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="496a7-128">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="496a7-128">approvalDuration</span></span>|<span data-ttu-id="496a7-129">持续时间</span><span class="sxs-lookup"><span data-stu-id="496a7-129">Duration</span></span>||
|<span data-ttu-id="496a7-130">approvalState</span><span class="sxs-lookup"><span data-stu-id="496a7-130">approvalState</span></span>|<span data-ttu-id="496a7-131">string</span><span class="sxs-lookup"><span data-stu-id="496a7-131">string</span></span>| <span data-ttu-id="496a7-132">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="496a7-132">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="496a7-133">approvalType</span><span class="sxs-lookup"><span data-stu-id="496a7-133">approvalType</span></span>|<span data-ttu-id="496a7-134">String</span><span class="sxs-lookup"><span data-stu-id="496a7-134">String</span></span>||
|<span data-ttu-id="496a7-135">approverReason</span><span class="sxs-lookup"><span data-stu-id="496a7-135">approverReason</span></span>|<span data-ttu-id="496a7-136">String</span><span class="sxs-lookup"><span data-stu-id="496a7-136">String</span></span>||
|<span data-ttu-id="496a7-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="496a7-137">endDateTime</span></span>|<span data-ttu-id="496a7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="496a7-138">DateTimeOffset</span></span>|<span data-ttu-id="496a7-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="496a7-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="496a7-141">id</span><span class="sxs-lookup"><span data-stu-id="496a7-141">id</span></span>|<span data-ttu-id="496a7-142">String</span><span class="sxs-lookup"><span data-stu-id="496a7-142">String</span></span>| <span data-ttu-id="496a7-143">只读。</span><span class="sxs-lookup"><span data-stu-id="496a7-143">Read-only.</span></span>|
|<span data-ttu-id="496a7-144">requestorReason</span><span class="sxs-lookup"><span data-stu-id="496a7-144">requestorReason</span></span>|<span data-ttu-id="496a7-145">String</span><span class="sxs-lookup"><span data-stu-id="496a7-145">String</span></span>||
|<span data-ttu-id="496a7-146">roleId</span><span class="sxs-lookup"><span data-stu-id="496a7-146">roleId</span></span>|<span data-ttu-id="496a7-147">String</span><span class="sxs-lookup"><span data-stu-id="496a7-147">String</span></span>||
|<span data-ttu-id="496a7-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="496a7-148">startDateTime</span></span>|<span data-ttu-id="496a7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="496a7-149">DateTimeOffset</span></span>|<span data-ttu-id="496a7-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="496a7-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="496a7-152">userId</span><span class="sxs-lookup"><span data-stu-id="496a7-152">userId</span></span>|<span data-ttu-id="496a7-153">String</span><span class="sxs-lookup"><span data-stu-id="496a7-153">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="496a7-154">关系</span><span class="sxs-lookup"><span data-stu-id="496a7-154">Relationships</span></span>
| <span data-ttu-id="496a7-155">关系</span><span class="sxs-lookup"><span data-stu-id="496a7-155">Relationship</span></span> | <span data-ttu-id="496a7-156">类型</span><span class="sxs-lookup"><span data-stu-id="496a7-156">Type</span></span>   |<span data-ttu-id="496a7-157">说明</span><span class="sxs-lookup"><span data-stu-id="496a7-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="496a7-158">roleInfo</span><span class="sxs-lookup"><span data-stu-id="496a7-158">roleInfo</span></span>|[<span data-ttu-id="496a7-159">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="496a7-159">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="496a7-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="496a7-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="496a7-162">请求</span><span class="sxs-lookup"><span data-stu-id="496a7-162">request</span></span>|[<span data-ttu-id="496a7-163">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="496a7-163">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="496a7-164">只读。</span><span class="sxs-lookup"><span data-stu-id="496a7-164">Read-only.</span></span> <span data-ttu-id="496a7-165">对此审批对象的角色分配请求</span><span class="sxs-lookup"><span data-stu-id="496a7-165">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="496a7-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="496a7-166">JSON representation</span></span>
<span data-ttu-id="496a7-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="496a7-167">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
