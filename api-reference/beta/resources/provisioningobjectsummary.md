---
title: provisioningObjectSummary 资源类型
description: 表示由 Azure AD 预配服务及其关联的属性执行的操作。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8bf8813b63d1d25d09c8ee9a8ff4bb5099728b77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993117"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="2137c-103">provisioningObjectSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="2137c-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="2137c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2137c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2137c-105">表示由 Azure AD 预配服务及其关联的属性执行的操作。</span><span class="sxs-lookup"><span data-stu-id="2137c-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="2137c-106">方法</span><span class="sxs-lookup"><span data-stu-id="2137c-106">Methods</span></span>

| <span data-ttu-id="2137c-107">方法</span><span class="sxs-lookup"><span data-stu-id="2137c-107">Method</span></span>  | <span data-ttu-id="2137c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2137c-108">Return Type</span></span> | <span data-ttu-id="2137c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2137c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2137c-110">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="2137c-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="2137c-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="2137c-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="2137c-112">获取租户中发生的所有设置事件的列表。</span><span class="sxs-lookup"><span data-stu-id="2137c-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="2137c-113">属性</span><span class="sxs-lookup"><span data-stu-id="2137c-113">Properties</span></span>

| <span data-ttu-id="2137c-114">属性</span><span class="sxs-lookup"><span data-stu-id="2137c-114">Property</span></span>     | <span data-ttu-id="2137c-115">类型</span><span class="sxs-lookup"><span data-stu-id="2137c-115">Type</span></span>        | <span data-ttu-id="2137c-116">说明</span><span class="sxs-lookup"><span data-stu-id="2137c-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2137c-117">action</span><span class="sxs-lookup"><span data-stu-id="2137c-117">action</span></span>|<span data-ttu-id="2137c-118">String</span><span class="sxs-lookup"><span data-stu-id="2137c-118">String</span></span>|<span data-ttu-id="2137c-119">指示活动名称或操作名称 (例如，创建用户，将 member 添加到 group) 中。</span><span class="sxs-lookup"><span data-stu-id="2137c-119">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="2137c-120">有关已记录活动的列表，请参阅 Azure AD 活动列表。</span><span class="sxs-lookup"><span data-stu-id="2137c-120">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="2137c-121">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="2137c-121">activityDateTime</span></span>|<span data-ttu-id="2137c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2137c-122">DateTimeOffset</span></span>|<span data-ttu-id="2137c-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2137c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2137c-125">changeId</span><span class="sxs-lookup"><span data-stu-id="2137c-125">changeId</span></span>|<span data-ttu-id="2137c-126">String</span><span class="sxs-lookup"><span data-stu-id="2137c-126">String</span></span>|<span data-ttu-id="2137c-127">此周期中的此更改的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2137c-127">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="2137c-128">cycleId</span><span class="sxs-lookup"><span data-stu-id="2137c-128">cycleId</span></span>|<span data-ttu-id="2137c-129">String</span><span class="sxs-lookup"><span data-stu-id="2137c-129">String</span></span>|<span data-ttu-id="2137c-130">每个作业迭代的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2137c-130">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="2137c-131">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="2137c-131">durationInMilliseconds</span></span>|<span data-ttu-id="2137c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="2137c-132">Int32</span></span>|<span data-ttu-id="2137c-133">指示此设置操作完成所花的时间。</span><span class="sxs-lookup"><span data-stu-id="2137c-133">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="2137c-134">以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="2137c-134">Measured in milliseconds.</span></span>|
|<span data-ttu-id="2137c-135">id</span><span class="sxs-lookup"><span data-stu-id="2137c-135">id</span></span>|<span data-ttu-id="2137c-136">String</span><span class="sxs-lookup"><span data-stu-id="2137c-136">String</span></span>| <span data-ttu-id="2137c-137">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2137c-137">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="2137c-138">这是只读的 GUID。</span><span class="sxs-lookup"><span data-stu-id="2137c-138">This is a read-only GUID.</span></span>|
|<span data-ttu-id="2137c-139">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="2137c-139">initiatedBy</span></span>|[<span data-ttu-id="2137c-140">initiator</span><span class="sxs-lookup"><span data-stu-id="2137c-140">initiator</span></span>](initiator.md)|<span data-ttu-id="2137c-141">启动此预配的参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-141">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="2137c-142">jobId</span><span class="sxs-lookup"><span data-stu-id="2137c-142">jobId</span></span>|<span data-ttu-id="2137c-143">String</span><span class="sxs-lookup"><span data-stu-id="2137c-143">String</span></span>|<span data-ttu-id="2137c-144">整个设置作业的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2137c-144">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="2137c-145">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="2137c-145">modifiedProperties</span></span>|<span data-ttu-id="2137c-146">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2137c-146">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="2137c-147">此对象上此设置操作中修改的每个属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-147">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="2137c-148">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="2137c-148">provisioningSteps</span></span>|<span data-ttu-id="2137c-149">[provisioningStep](provisioningstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2137c-149">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="2137c-150">设置中的每个步骤的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-150">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="2137c-151">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="2137c-151">servicePrincipal</span></span>|<span data-ttu-id="2137c-152">[servicePrincipal](serviceprincipal.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2137c-152">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="2137c-153">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="2137c-153">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="2137c-154">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="2137c-154">sourceIdentity</span></span>|[<span data-ttu-id="2137c-155">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="2137c-155">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="2137c-156">正在预配的源对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-156">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="2137c-157">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="2137c-157">sourceSystem</span></span>|[<span data-ttu-id="2137c-158">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="2137c-158">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="2137c-159">正在预配的对象的源系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-159">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="2137c-160">statusInfo</span><span class="sxs-lookup"><span data-stu-id="2137c-160">statusInfo</span></span>|[<span data-ttu-id="2137c-161">statusBase</span><span class="sxs-lookup"><span data-stu-id="2137c-161">statusBase</span></span>](statusbase.md)|<span data-ttu-id="2137c-162">设置状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-162">Details of provisioning status.</span></span>|
|<span data-ttu-id="2137c-163">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="2137c-163">targetIdentity</span></span>|[<span data-ttu-id="2137c-164">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="2137c-164">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="2137c-165">正在预配的目标对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-165">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="2137c-166">targetSystem</span><span class="sxs-lookup"><span data-stu-id="2137c-166">targetSystem</span></span>|[<span data-ttu-id="2137c-167">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="2137c-167">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="2137c-168">要设置的对象的目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2137c-168">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="2137c-169">tenantId</span><span class="sxs-lookup"><span data-stu-id="2137c-169">tenantId</span></span>|<span data-ttu-id="2137c-170">String</span><span class="sxs-lookup"><span data-stu-id="2137c-170">String</span></span>|<span data-ttu-id="2137c-171">唯一的 Azure AD 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="2137c-171">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2137c-172">关系</span><span class="sxs-lookup"><span data-stu-id="2137c-172">Relationships</span></span>

<span data-ttu-id="2137c-173">无。</span><span class="sxs-lookup"><span data-stu-id="2137c-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2137c-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2137c-174">JSON representation</span></span>

<span data-ttu-id="2137c-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2137c-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
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
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
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


