---
title: provisioningObjectSummary 资源类型
description: 表示 Azure AD 预配服务及其关联属性执行的操作。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d9852745ed14cacd47389da5031cb83af306e2d0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241494"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="615dc-103">provisioningObjectSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="615dc-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="615dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615dc-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="615dc-105">表示 Azure AD 预配服务及其关联属性执行的操作。</span><span class="sxs-lookup"><span data-stu-id="615dc-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="615dc-106">方法</span><span class="sxs-lookup"><span data-stu-id="615dc-106">Methods</span></span>

| <span data-ttu-id="615dc-107">方法</span><span class="sxs-lookup"><span data-stu-id="615dc-107">Method</span></span>  | <span data-ttu-id="615dc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="615dc-108">Return Type</span></span> | <span data-ttu-id="615dc-109">说明</span><span class="sxs-lookup"><span data-stu-id="615dc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="615dc-110">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="615dc-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="615dc-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="615dc-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="615dc-112">获取租户中发生的所有预配事件的列表。</span><span class="sxs-lookup"><span data-stu-id="615dc-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="615dc-113">属性</span><span class="sxs-lookup"><span data-stu-id="615dc-113">Properties</span></span>

| <span data-ttu-id="615dc-114">属性</span><span class="sxs-lookup"><span data-stu-id="615dc-114">Property</span></span>     | <span data-ttu-id="615dc-115">类型</span><span class="sxs-lookup"><span data-stu-id="615dc-115">Type</span></span>        | <span data-ttu-id="615dc-116">说明</span><span class="sxs-lookup"><span data-stu-id="615dc-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="615dc-117">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="615dc-117">provisioningAction</span></span>|<span data-ttu-id="615dc-118">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="615dc-118">provisioningAction</span></span>|<span data-ttu-id="615dc-119">指示活动名称或操作名称。</span><span class="sxs-lookup"><span data-stu-id="615dc-119">Indicates the activity name or the operation name.</span></span> <span data-ttu-id="615dc-120">可能的值是 `create` `update` `delete` ：、、、、 `stageddelete` `disable` 和 `other` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="615dc-120">Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`.</span></span> <span data-ttu-id="615dc-121">有关记录的活动列表，请参阅 Azure AD 活动列表。</span><span class="sxs-lookup"><span data-stu-id="615dc-121">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="615dc-122">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="615dc-122">activityDateTime</span></span>|<span data-ttu-id="615dc-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615dc-123">DateTimeOffset</span></span>|<span data-ttu-id="615dc-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="615dc-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="615dc-125">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="615dc-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="615dc-126">changeId</span><span class="sxs-lookup"><span data-stu-id="615dc-126">changeId</span></span>|<span data-ttu-id="615dc-127">String</span><span class="sxs-lookup"><span data-stu-id="615dc-127">String</span></span>|<span data-ttu-id="615dc-128">此周期中此更改的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="615dc-128">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="615dc-129">cycleId</span><span class="sxs-lookup"><span data-stu-id="615dc-129">cycleId</span></span>|<span data-ttu-id="615dc-130">String</span><span class="sxs-lookup"><span data-stu-id="615dc-130">String</span></span>|<span data-ttu-id="615dc-131">每个作业迭代的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="615dc-131">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="615dc-132">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="615dc-132">durationInMilliseconds</span></span>|<span data-ttu-id="615dc-133">Int32</span><span class="sxs-lookup"><span data-stu-id="615dc-133">Int32</span></span>|<span data-ttu-id="615dc-134">指示完成此预配操作所需要的时间。</span><span class="sxs-lookup"><span data-stu-id="615dc-134">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="615dc-135">以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="615dc-135">Measured in milliseconds.</span></span>|
|<span data-ttu-id="615dc-136">id</span><span class="sxs-lookup"><span data-stu-id="615dc-136">id</span></span>|<span data-ttu-id="615dc-137">String</span><span class="sxs-lookup"><span data-stu-id="615dc-137">String</span></span>| <span data-ttu-id="615dc-138">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="615dc-138">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="615dc-139">这是只读 GUID。</span><span class="sxs-lookup"><span data-stu-id="615dc-139">This is a read-only GUID.</span></span>|
|<span data-ttu-id="615dc-140">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="615dc-140">initiatedBy</span></span>|[<span data-ttu-id="615dc-141">initiator</span><span class="sxs-lookup"><span data-stu-id="615dc-141">initiator</span></span>](initiator.md)|<span data-ttu-id="615dc-142">此预配的发起人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-142">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="615dc-143">jobId</span><span class="sxs-lookup"><span data-stu-id="615dc-143">jobId</span></span>|<span data-ttu-id="615dc-144">String</span><span class="sxs-lookup"><span data-stu-id="615dc-144">String</span></span>|<span data-ttu-id="615dc-145">整个预配作业的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="615dc-145">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="615dc-146">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="615dc-146">modifiedProperties</span></span>|<span data-ttu-id="615dc-147">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="615dc-147">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="615dc-148">在此对象的此设置操作中修改的每个属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-148">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="615dc-149">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="615dc-149">provisioningSteps</span></span>|<span data-ttu-id="615dc-150">[provisioningStep](provisioningstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="615dc-150">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="615dc-151">预配中每个步骤的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-151">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="615dc-152">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="615dc-152">servicePrincipal</span></span>|<span data-ttu-id="615dc-153">[servicePrincipal](provisioningserviceprincipal.md) 集合</span><span class="sxs-lookup"><span data-stu-id="615dc-153">[servicePrincipal](provisioningserviceprincipal.md) collection</span></span>|<span data-ttu-id="615dc-154">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="615dc-154">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="615dc-155">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="615dc-155">sourceIdentity</span></span>|[<span data-ttu-id="615dc-156">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="615dc-156">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="615dc-157">要预配的源对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-157">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="615dc-158">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="615dc-158">sourceSystem</span></span>|[<span data-ttu-id="615dc-159">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="615dc-159">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="615dc-160">要设置的对象的源系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-160">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="615dc-161">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="615dc-161">provisioningStatusInfo</span></span>|[<span data-ttu-id="615dc-162">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="615dc-162">provisioningStatusInfo</span></span>](provisioningstatusinfo.md)|<span data-ttu-id="615dc-163">设置状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-163">Details of provisioning status.</span></span>|
|<span data-ttu-id="615dc-164">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="615dc-164">targetIdentity</span></span>|[<span data-ttu-id="615dc-165">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="615dc-165">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="615dc-166">正在设置的目标对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-166">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="615dc-167">targetSystem</span><span class="sxs-lookup"><span data-stu-id="615dc-167">targetSystem</span></span>|[<span data-ttu-id="615dc-168">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="615dc-168">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="615dc-169">要设置的对象的目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="615dc-169">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="615dc-170">tenantId</span><span class="sxs-lookup"><span data-stu-id="615dc-170">tenantId</span></span>|<span data-ttu-id="615dc-171">String</span><span class="sxs-lookup"><span data-stu-id="615dc-171">String</span></span>|<span data-ttu-id="615dc-172">唯一的 Azure AD 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="615dc-172">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="615dc-173">关系</span><span class="sxs-lookup"><span data-stu-id="615dc-173">Relationships</span></span>

<span data-ttu-id="615dc-174">无。</span><span class="sxs-lookup"><span data-stu-id="615dc-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="615dc-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="615dc-175">JSON representation</span></span>

<span data-ttu-id="615dc-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="615dc-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "provisioningAction":  "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "servicePrincipal": [{"@odata.type": "microsoft.graph.provisioningServicePrincipal"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "provisioningStatusInfo": {"@odata.type": "microsoft.graph.provisioningStatusInfo"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystem"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


