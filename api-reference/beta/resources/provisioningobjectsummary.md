---
title: provisioningObjectSummary 资源类型
description: 表示 Azure AD 预配服务及其关联属性执行的操作。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e51a3a5e184fae0c5c35e01b5a0b23494f63edc7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135371"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="6a224-103">provisioningObjectSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a224-103">provisioningObjectSummary resource type</span></span>

<span data-ttu-id="6a224-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a224-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a224-105">表示 Azure AD 预配服务及其关联属性执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6a224-105">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="6a224-106">方法</span><span class="sxs-lookup"><span data-stu-id="6a224-106">Methods</span></span>

| <span data-ttu-id="6a224-107">方法</span><span class="sxs-lookup"><span data-stu-id="6a224-107">Method</span></span>  | <span data-ttu-id="6a224-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a224-108">Return Type</span></span> | <span data-ttu-id="6a224-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a224-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6a224-110">列出 provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="6a224-110">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="6a224-111">provisioningObjectSummary</span><span class="sxs-lookup"><span data-stu-id="6a224-111">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="6a224-112">获取租户中发生的所有预配事件的列表。</span><span class="sxs-lookup"><span data-stu-id="6a224-112">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="6a224-113">属性</span><span class="sxs-lookup"><span data-stu-id="6a224-113">Properties</span></span>

| <span data-ttu-id="6a224-114">属性</span><span class="sxs-lookup"><span data-stu-id="6a224-114">Property</span></span>     | <span data-ttu-id="6a224-115">类型</span><span class="sxs-lookup"><span data-stu-id="6a224-115">Type</span></span>        | <span data-ttu-id="6a224-116">说明</span><span class="sxs-lookup"><span data-stu-id="6a224-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a224-117">action</span><span class="sxs-lookup"><span data-stu-id="6a224-117">action</span></span>|<span data-ttu-id="6a224-118">字符串</span><span class="sxs-lookup"><span data-stu-id="6a224-118">String</span></span>|<span data-ttu-id="6a224-119">指示活动名称或操作名称 (例如，创建用户，将成员添加到组) 。</span><span class="sxs-lookup"><span data-stu-id="6a224-119">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="6a224-120">有关记录的活动列表，请参阅 Azure AD 活动列表。</span><span class="sxs-lookup"><span data-stu-id="6a224-120">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="6a224-121">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6a224-121">activityDateTime</span></span>|<span data-ttu-id="6a224-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a224-122">DateTimeOffset</span></span>|<span data-ttu-id="6a224-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6a224-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6a224-125">changeId</span><span class="sxs-lookup"><span data-stu-id="6a224-125">changeId</span></span>|<span data-ttu-id="6a224-126">字符串</span><span class="sxs-lookup"><span data-stu-id="6a224-126">String</span></span>|<span data-ttu-id="6a224-127">此周期中此更改的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6a224-127">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="6a224-128">cycleId</span><span class="sxs-lookup"><span data-stu-id="6a224-128">cycleId</span></span>|<span data-ttu-id="6a224-129">字符串</span><span class="sxs-lookup"><span data-stu-id="6a224-129">String</span></span>|<span data-ttu-id="6a224-130">每个作业迭代的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6a224-130">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="6a224-131">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="6a224-131">durationInMilliseconds</span></span>|<span data-ttu-id="6a224-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6a224-132">Int32</span></span>|<span data-ttu-id="6a224-133">指示完成此设置操作所需要的时间。</span><span class="sxs-lookup"><span data-stu-id="6a224-133">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="6a224-134">以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="6a224-134">Measured in milliseconds.</span></span>|
|<span data-ttu-id="6a224-135">id</span><span class="sxs-lookup"><span data-stu-id="6a224-135">id</span></span>|<span data-ttu-id="6a224-136">String</span><span class="sxs-lookup"><span data-stu-id="6a224-136">String</span></span>| <span data-ttu-id="6a224-137">指示活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6a224-137">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="6a224-138">这是只读 GUID。</span><span class="sxs-lookup"><span data-stu-id="6a224-138">This is a read-only GUID.</span></span>|
|<span data-ttu-id="6a224-139">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6a224-139">initiatedBy</span></span>|[<span data-ttu-id="6a224-140">initiator</span><span class="sxs-lookup"><span data-stu-id="6a224-140">initiator</span></span>](initiator.md)|<span data-ttu-id="6a224-141">此预配的发起人的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-141">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="6a224-142">jobId</span><span class="sxs-lookup"><span data-stu-id="6a224-142">jobId</span></span>|<span data-ttu-id="6a224-143">字符串</span><span class="sxs-lookup"><span data-stu-id="6a224-143">String</span></span>|<span data-ttu-id="6a224-144">整个预配作业的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6a224-144">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="6a224-145">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="6a224-145">modifiedProperties</span></span>|<span data-ttu-id="6a224-146">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a224-146">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="6a224-147">在此对象的此设置操作中修改的每个属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-147">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="6a224-148">provisioningSteps</span><span class="sxs-lookup"><span data-stu-id="6a224-148">provisioningSteps</span></span>|<span data-ttu-id="6a224-149">[provisioningStep](provisioningstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a224-149">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="6a224-150">预配中每个步骤的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-150">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="6a224-151">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="6a224-151">servicePrincipal</span></span>|<span data-ttu-id="6a224-152">[servicePrincipal](serviceprincipal.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a224-152">[servicePrincipal](serviceprincipal.md) collection</span></span>|<span data-ttu-id="6a224-153">表示用于预配的服务主体。</span><span class="sxs-lookup"><span data-stu-id="6a224-153">Represents the service principal used for provisioning.</span></span>|
|<span data-ttu-id="6a224-154">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="6a224-154">sourceIdentity</span></span>|[<span data-ttu-id="6a224-155">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="6a224-155">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="6a224-156">要预配的源对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-156">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="6a224-157">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="6a224-157">sourceSystem</span></span>|[<span data-ttu-id="6a224-158">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="6a224-158">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="6a224-159">要设置的对象的源系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-159">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="6a224-160">statusInfo</span><span class="sxs-lookup"><span data-stu-id="6a224-160">statusInfo</span></span>|[<span data-ttu-id="6a224-161">statusBase</span><span class="sxs-lookup"><span data-stu-id="6a224-161">statusBase</span></span>](statusbase.md)|<span data-ttu-id="6a224-162">设置状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-162">Details of provisioning status.</span></span>|
|<span data-ttu-id="6a224-163">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="6a224-163">targetIdentity</span></span>|[<span data-ttu-id="6a224-164">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="6a224-164">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="6a224-165">要设置的目标对象的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-165">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="6a224-166">targetSystem</span><span class="sxs-lookup"><span data-stu-id="6a224-166">targetSystem</span></span>|[<span data-ttu-id="6a224-167">provisioningSystemDetails</span><span class="sxs-lookup"><span data-stu-id="6a224-167">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="6a224-168">要设置的对象的目标系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6a224-168">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="6a224-169">tenantId</span><span class="sxs-lookup"><span data-stu-id="6a224-169">tenantId</span></span>|<span data-ttu-id="6a224-170">字符串</span><span class="sxs-lookup"><span data-stu-id="6a224-170">String</span></span>|<span data-ttu-id="6a224-171">唯一的 Azure AD 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="6a224-171">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a224-172">关系</span><span class="sxs-lookup"><span data-stu-id="6a224-172">Relationships</span></span>

<span data-ttu-id="6a224-173">无。</span><span class="sxs-lookup"><span data-stu-id="6a224-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a224-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a224-174">JSON representation</span></span>

<span data-ttu-id="6a224-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a224-175">The following is a JSON representation of the resource.</span></span>

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


