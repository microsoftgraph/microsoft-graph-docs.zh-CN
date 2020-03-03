---
title: provisioningObjectSummary 资源类型
description: 表示由 Azure AD 预配服务及其关联的属性执行的操作。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eabbb0c0cd1cd692ad6ebc5a346c46473161b1
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394594"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="6fd61-103">provisioningObjectSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fd61-103">provisioningObjectSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd61-104">表示由 Azure AD 预配服务及其关联的属性执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6fd61-104">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="6fd61-105">方法</span><span class="sxs-lookup"><span data-stu-id="6fd61-105">Methods</span></span>

| <span data-ttu-id="6fd61-106">方法</span><span class="sxs-lookup"><span data-stu-id="6fd61-106">Method</span></span>       | <span data-ttu-id="6fd61-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fd61-107">Return Type</span></span> | <span data-ttu-id="6fd61-108">说明</span><span class="sxs-lookup"><span data-stu-id="6fd61-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6fd61-109">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="6fd61-109">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="6fd61-110">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="6fd61-110">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="6fd61-111">获取租户中发生的所有设置事件的列表。</span><span class="sxs-lookup"><span data-stu-id="6fd61-111">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="6fd61-112">属性</span><span class="sxs-lookup"><span data-stu-id="6fd61-112">Properties</span></span>

| <span data-ttu-id="6fd61-113">属性</span><span class="sxs-lookup"><span data-stu-id="6fd61-113">Property</span></span>     | <span data-ttu-id="6fd61-114">类型</span><span class="sxs-lookup"><span data-stu-id="6fd61-114">Type</span></span>        | <span data-ttu-id="6fd61-115">说明</span><span class="sxs-lookup"><span data-stu-id="6fd61-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fd61-116">action</span><span class="sxs-lookup"><span data-stu-id="6fd61-116">action</span></span>|<span data-ttu-id="6fd61-117">String</span><span class="sxs-lookup"><span data-stu-id="6fd61-117">String</span></span>|<span data-ttu-id="6fd61-118">指示活动名称或操作名称（例如，"创建用户"、"将成员添加到组"）。</span><span class="sxs-lookup"><span data-stu-id="6fd61-118">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="6fd61-119">有关已记录活动的列表，请参阅 Azure AD 活动列表。</span><span class="sxs-lookup"><span data-stu-id="6fd61-119">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="6fd61-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6fd61-120">activityDateTime</span></span>|<span data-ttu-id="6fd61-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fd61-121">DateTimeOffset</span></span>|<span data-ttu-id="6fd61-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6fd61-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6fd61-124">changeId</span><span class="sxs-lookup"><span data-stu-id="6fd61-124">changeId</span></span>|<span data-ttu-id="6fd61-125">String</span><span class="sxs-lookup"><span data-stu-id="6fd61-125">String</span></span>|<span data-ttu-id="6fd61-126">此周期中的此更改的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd61-126">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="6fd61-127">cycleId</span><span class="sxs-lookup"><span data-stu-id="6fd61-127">cycleId</span></span>|<span data-ttu-id="6fd61-128">String</span><span class="sxs-lookup"><span data-stu-id="6fd61-128">String</span></span>|<span data-ttu-id="6fd61-129">每个作业迭代的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd61-129">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="6fd61-130">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="6fd61-130">durationInMilliseconds</span></span>|<span data-ttu-id="6fd61-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6fd61-131">Int32</span></span>|<span data-ttu-id="6fd61-132">指示此设置操作完成所花的时间。</span><span class="sxs-lookup"><span data-stu-id="6fd61-132">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="6fd61-133">以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="6fd61-133">Measured in milliseconds.</span></span>|
|<span data-ttu-id="6fd61-134">id</span><span class="sxs-lookup"><span data-stu-id="6fd61-134">id</span></span>|<span data-ttu-id="6fd61-135">String</span><span class="sxs-lookup"><span data-stu-id="6fd61-135">String</span></span>| <span data-ttu-id="6fd61-136">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd61-136">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="6fd61-137">这是只读的 GUID。</span><span class="sxs-lookup"><span data-stu-id="6fd61-137">This is a read-only GUID.</span></span>|
|<span data-ttu-id="6fd61-138">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6fd61-138">initiatedBy</span></span>|[<span data-ttu-id="6fd61-139">initiator</span><span class="sxs-lookup"><span data-stu-id="6fd61-139">initiator</span></span>](initiator.md)|<span data-ttu-id="6fd61-140">启动此预配的参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-140">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="6fd61-141">jobId</span><span class="sxs-lookup"><span data-stu-id="6fd61-141">jobId</span></span>|<span data-ttu-id="6fd61-142">String</span><span class="sxs-lookup"><span data-stu-id="6fd61-142">String</span></span>|<span data-ttu-id="6fd61-143">整个设置作业的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd61-143">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="6fd61-144">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="6fd61-144">modifiedProperties</span></span>|<span data-ttu-id="6fd61-145">[modifiedProperty](modifiedproperty.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fd61-145">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="6fd61-146">此对象上此设置操作中修改的每个属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-146">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="6fd61-147">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="6fd61-147">provisioningSteps</span></span>|<span data-ttu-id="6fd61-148">[provisioningStep](provisioningstep.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fd61-148">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="6fd61-149">设置中的每个步骤的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-149">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="6fd61-150">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6fd61-150">servicePrincipal</span></span>|<span data-ttu-id="6fd61-151">[servicePrincipal](serviceprincipal.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fd61-151">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="6fd61-152">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="6fd61-152">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="6fd61-153">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="6fd61-153">sourceIdentity</span></span>|[<span data-ttu-id="6fd61-154">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="6fd61-154">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="6fd61-155">正在预配的源对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-155">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="6fd61-156">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="6fd61-156">sourceSystem</span></span>|[<span data-ttu-id="6fd61-157">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="6fd61-157">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="6fd61-158">正在预配的对象的源系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-158">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="6fd61-159">statusInfo</span><span class="sxs-lookup"><span data-stu-id="6fd61-159">statusInfo</span></span>|[<span data-ttu-id="6fd61-160">statusBase</span><span class="sxs-lookup"><span data-stu-id="6fd61-160">statusBase</span></span>](statusbase.md)|<span data-ttu-id="6fd61-161">设置状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-161">Details of provisioning status.</span></span>|
|<span data-ttu-id="6fd61-162">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="6fd61-162">targetIdentity</span></span>|[<span data-ttu-id="6fd61-163">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="6fd61-163">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="6fd61-164">正在预配的目标对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-164">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="6fd61-165">targetSystem</span><span class="sxs-lookup"><span data-stu-id="6fd61-165">targetSystem</span></span>|[<span data-ttu-id="6fd61-166">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="6fd61-166">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="6fd61-167">要设置的对象的目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fd61-167">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="6fd61-168">tenantId</span><span class="sxs-lookup"><span data-stu-id="6fd61-168">tenantId</span></span>|<span data-ttu-id="6fd61-169">String</span><span class="sxs-lookup"><span data-stu-id="6fd61-169">String</span></span>|<span data-ttu-id="6fd61-170">唯一的 Azure AD 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd61-170">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fd61-171">关系</span><span class="sxs-lookup"><span data-stu-id="6fd61-171">Relationships</span></span>

<span data-ttu-id="6fd61-172">无。</span><span class="sxs-lookup"><span data-stu-id="6fd61-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fd61-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fd61-173">JSON representation</span></span>

<span data-ttu-id="6fd61-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fd61-174">The following is a JSON representation of the resource.</span></span>

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
