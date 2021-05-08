---
title: provisioningObjectSummary 资源类型
description: 表示 Azure AD 预配服务及其关联属性执行的操作。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7004a611c3fe36e2ce2d32824a5e9b78e53e61bd
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231911"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="34ed3-103">provisioningObjectSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="34ed3-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="34ed3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34ed3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION]
><span data-ttu-id="34ed3-105">**action** 和 **statusInfo** 属性已弃用。</span><span class="sxs-lookup"><span data-stu-id="34ed3-105">The **action** and **statusInfo** properties are deprecated.</span></span> <span data-ttu-id="34ed3-106">属性 **操作** 应替换为 **provisioningAction**。</span><span class="sxs-lookup"><span data-stu-id="34ed3-106">Property **action** should be replaced by **provisioningAction**.</span></span> <span data-ttu-id="34ed3-107">属性 **statusInfo** 应替换为 **provisioningStatusInfo**。</span><span class="sxs-lookup"><span data-stu-id="34ed3-107">Property **statusInfo** should be replaced by **provisioningStatusInfo**.</span></span>

<span data-ttu-id="34ed3-108">表示 Azure AD 预配服务及其关联属性执行的操作。</span><span class="sxs-lookup"><span data-stu-id="34ed3-108">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="34ed3-109">方法</span><span class="sxs-lookup"><span data-stu-id="34ed3-109">Methods</span></span>

| <span data-ttu-id="34ed3-110">方法</span><span class="sxs-lookup"><span data-stu-id="34ed3-110">Method</span></span>  | <span data-ttu-id="34ed3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="34ed3-111">Return Type</span></span> | <span data-ttu-id="34ed3-112">说明</span><span class="sxs-lookup"><span data-stu-id="34ed3-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="34ed3-113">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="34ed3-113">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="34ed3-114">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="34ed3-114">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="34ed3-115">获取租户中发生的所有预配事件的列表。</span><span class="sxs-lookup"><span data-stu-id="34ed3-115">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="34ed3-116">属性</span><span class="sxs-lookup"><span data-stu-id="34ed3-116">Properties</span></span>

| <span data-ttu-id="34ed3-117">属性</span><span class="sxs-lookup"><span data-stu-id="34ed3-117">Property</span></span>     | <span data-ttu-id="34ed3-118">类型</span><span class="sxs-lookup"><span data-stu-id="34ed3-118">Type</span></span>        | <span data-ttu-id="34ed3-119">说明</span><span class="sxs-lookup"><span data-stu-id="34ed3-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34ed3-120">provisioningAction</span><span class="sxs-lookup"><span data-stu-id="34ed3-120">provisioningAction</span></span>|<span data-ttu-id="34ed3-121">string</span><span class="sxs-lookup"><span data-stu-id="34ed3-121">string</span></span>|<span data-ttu-id="34ed3-122">指示活动名称或操作名称。</span><span class="sxs-lookup"><span data-stu-id="34ed3-122">Indicates the activity name or the operation name.</span></span> <span data-ttu-id="34ed3-123">可能的值是 `create` `update` `delete` ：、、、、 `stageddelete` `disable` 和 `other` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="34ed3-123">Possible values are: `create`, `update`, `delete`, `stageddelete`, `disable`, `other` and `unknownFutureValue`.</span></span> <span data-ttu-id="34ed3-124">有关记录的活动列表，请参阅 Azure AD 活动列表。</span><span class="sxs-lookup"><span data-stu-id="34ed3-124">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="34ed3-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="34ed3-125">activityDateTime</span></span>|<span data-ttu-id="34ed3-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ed3-126">DateTimeOffset</span></span>|<span data-ttu-id="34ed3-127">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="34ed3-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34ed3-128">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="34ed3-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="34ed3-129">changeId</span><span class="sxs-lookup"><span data-stu-id="34ed3-129">changeId</span></span>|<span data-ttu-id="34ed3-130">String</span><span class="sxs-lookup"><span data-stu-id="34ed3-130">String</span></span>|<span data-ttu-id="34ed3-131">此周期中此更改的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="34ed3-131">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="34ed3-132">cycleId</span><span class="sxs-lookup"><span data-stu-id="34ed3-132">cycleId</span></span>|<span data-ttu-id="34ed3-133">String</span><span class="sxs-lookup"><span data-stu-id="34ed3-133">String</span></span>|<span data-ttu-id="34ed3-134">每个作业迭代的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="34ed3-134">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="34ed3-135">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="34ed3-135">durationInMilliseconds</span></span>|<span data-ttu-id="34ed3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="34ed3-136">Int32</span></span>|<span data-ttu-id="34ed3-137">指示完成此预配操作所需要的时间。</span><span class="sxs-lookup"><span data-stu-id="34ed3-137">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="34ed3-138">以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="34ed3-138">Measured in milliseconds.</span></span>|
|<span data-ttu-id="34ed3-139">id</span><span class="sxs-lookup"><span data-stu-id="34ed3-139">id</span></span>|<span data-ttu-id="34ed3-140">String</span><span class="sxs-lookup"><span data-stu-id="34ed3-140">String</span></span>| <span data-ttu-id="34ed3-141">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="34ed3-141">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="34ed3-142">这是只读 GUID。</span><span class="sxs-lookup"><span data-stu-id="34ed3-142">This is a read-only GUID.</span></span>|
|<span data-ttu-id="34ed3-143">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="34ed3-143">initiatedBy</span></span>|[<span data-ttu-id="34ed3-144">initiator</span><span class="sxs-lookup"><span data-stu-id="34ed3-144">initiator</span></span>](initiator.md)|<span data-ttu-id="34ed3-145">此预配的发起人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-145">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="34ed3-146">jobId</span><span class="sxs-lookup"><span data-stu-id="34ed3-146">jobId</span></span>|<span data-ttu-id="34ed3-147">String</span><span class="sxs-lookup"><span data-stu-id="34ed3-147">String</span></span>|<span data-ttu-id="34ed3-148">整个预配作业的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="34ed3-148">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="34ed3-149">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="34ed3-149">modifiedProperties</span></span>|<span data-ttu-id="34ed3-150">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ed3-150">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="34ed3-151">在此对象的此设置操作中修改的每个属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-151">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="34ed3-152">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="34ed3-152">provisioningSteps</span></span>|<span data-ttu-id="34ed3-153">[provisioningStep](provisioningstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ed3-153">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="34ed3-154">预配中每个步骤的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-154">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="34ed3-155">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="34ed3-155">servicePrincipal</span></span>|<span data-ttu-id="34ed3-156">[servicePrincipal](serviceprincipal.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34ed3-156">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="34ed3-157">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="34ed3-157">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="34ed3-158">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="34ed3-158">sourceIdentity</span></span>|[<span data-ttu-id="34ed3-159">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="34ed3-159">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="34ed3-160">要预配的源对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-160">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="34ed3-161">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="34ed3-161">sourceSystem</span></span>|[<span data-ttu-id="34ed3-162">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="34ed3-162">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="34ed3-163">要设置的对象的源系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-163">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="34ed3-164">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="34ed3-164">provisioningStatusInfo</span></span>|[<span data-ttu-id="34ed3-165">provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="34ed3-165">provisioningStatusInfo</span></span>](provisioningstatusinfo.md)|<span data-ttu-id="34ed3-166">设置状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-166">Details of provisioning status.</span></span>|
|<span data-ttu-id="34ed3-167">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="34ed3-167">targetIdentity</span></span>|[<span data-ttu-id="34ed3-168">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="34ed3-168">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="34ed3-169">正在设置的目标对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-169">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="34ed3-170">targetSystem</span><span class="sxs-lookup"><span data-stu-id="34ed3-170">targetSystem</span></span>|[<span data-ttu-id="34ed3-171">provisioningSystem</span><span class="sxs-lookup"><span data-stu-id="34ed3-171">provisioningSystem</span></span>](provisioningsystem.md)|<span data-ttu-id="34ed3-172">要设置的对象的目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-172">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="34ed3-173">tenantId</span><span class="sxs-lookup"><span data-stu-id="34ed3-173">tenantId</span></span>|<span data-ttu-id="34ed3-174">String</span><span class="sxs-lookup"><span data-stu-id="34ed3-174">String</span></span>|<span data-ttu-id="34ed3-175">唯一的 Azure AD 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="34ed3-175">Unique Azure AD tenant ID.</span></span>|
|<span data-ttu-id="34ed3-176">action (deprecated) </span><span class="sxs-lookup"><span data-stu-id="34ed3-176">action (deprecated)</span></span>|<span data-ttu-id="34ed3-177">String</span><span class="sxs-lookup"><span data-stu-id="34ed3-177">String</span></span>|<span data-ttu-id="34ed3-178">指示活动名称或操作名称 (例如，创建用户、将成员添加到组) 。</span><span class="sxs-lookup"><span data-stu-id="34ed3-178">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="34ed3-179">有关记录的活动列表，请参阅 Azure AD 活动列表。</span><span class="sxs-lookup"><span data-stu-id="34ed3-179">For a list of activities logged, refer to Azure AD activity list.</span></span> <span data-ttu-id="34ed3-180">这已弃用。</span><span class="sxs-lookup"><span data-stu-id="34ed3-180">This is deprecated.</span></span> <span data-ttu-id="34ed3-181">请改为使用 provisioningAction。</span><span class="sxs-lookup"><span data-stu-id="34ed3-181">Please use provisioningAction instead.</span></span>|
|<span data-ttu-id="34ed3-182">statusInfo (已弃) </span><span class="sxs-lookup"><span data-stu-id="34ed3-182">statusInfo (deprecated)</span></span>|[<span data-ttu-id="34ed3-183">statusBase</span><span class="sxs-lookup"><span data-stu-id="34ed3-183">statusBase</span></span>](statusbase.md)|<span data-ttu-id="34ed3-184">设置状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="34ed3-184">Details of provisioning status.</span></span> <span data-ttu-id="34ed3-185">这已弃用。</span><span class="sxs-lookup"><span data-stu-id="34ed3-185">This is deprecated.</span></span> <span data-ttu-id="34ed3-186">请改为使用 provisioningStatusInfo。</span><span class="sxs-lookup"><span data-stu-id="34ed3-186">Please use provisioningStatusInfo instead.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34ed3-187">关系</span><span class="sxs-lookup"><span data-stu-id="34ed3-187">Relationships</span></span>

<span data-ttu-id="34ed3-188">无。</span><span class="sxs-lookup"><span data-stu-id="34ed3-188">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34ed3-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34ed3-189">JSON representation</span></span>

<span data-ttu-id="34ed3-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34ed3-190">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
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
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
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


