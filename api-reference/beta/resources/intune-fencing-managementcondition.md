---
title: managementCondition 资源类型
description: 管理条件是可以动态触发的事件，如地域时限、时限和网络时限。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24aca3452d6dcb6dd43290c8ce2359551db65331
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382650"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="4f4b5-103">managementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f4b5-103">managementCondition resource type</span></span>

<span data-ttu-id="4f4b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f4b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f4b5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f4b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f4b5-107">管理条件是可以动态触发的事件，如地域时限、时限和网络时限。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="4f4b5-108">方法</span><span class="sxs-lookup"><span data-stu-id="4f4b5-108">Methods</span></span>
|<span data-ttu-id="4f4b5-109">方法</span><span class="sxs-lookup"><span data-stu-id="4f4b5-109">Method</span></span>|<span data-ttu-id="4f4b5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f4b5-110">Return Type</span></span>|<span data-ttu-id="4f4b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f4b5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f4b5-112">列出 managementConditions</span><span class="sxs-lookup"><span data-stu-id="4f4b5-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="4f4b5-113">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f4b5-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="4f4b5-114">列出[managementCondition](../resources/intune-fencing-managementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="4f4b5-115">获取 managementCondition</span><span class="sxs-lookup"><span data-stu-id="4f4b5-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="4f4b5-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="4f4b5-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="4f4b5-117">读取[managementCondition](../resources/intune-fencing-managementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="4f4b5-118">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="4f4b5-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="4f4b5-119">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f4b5-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="4f4b5-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4f4b5-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4f4b5-121">属性</span><span class="sxs-lookup"><span data-stu-id="4f4b5-121">Properties</span></span>
|<span data-ttu-id="4f4b5-122">属性</span><span class="sxs-lookup"><span data-stu-id="4f4b5-122">Property</span></span>|<span data-ttu-id="4f4b5-123">类型</span><span class="sxs-lookup"><span data-stu-id="4f4b5-123">Type</span></span>|<span data-ttu-id="4f4b5-124">说明</span><span class="sxs-lookup"><span data-stu-id="4f4b5-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f4b5-125">id</span><span class="sxs-lookup"><span data-stu-id="4f4b5-125">id</span></span>|<span data-ttu-id="4f4b5-126">字符串</span><span class="sxs-lookup"><span data-stu-id="4f4b5-126">String</span></span>|<span data-ttu-id="4f4b5-127">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="4f4b5-128">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="4f4b5-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="4f4b5-129">uniqueName</span></span>|<span data-ttu-id="4f4b5-130">字符串</span><span class="sxs-lookup"><span data-stu-id="4f4b5-130">String</span></span>|<span data-ttu-id="4f4b5-131">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-131">Unique name for the management condition.</span></span> <span data-ttu-id="4f4b5-132">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="4f4b5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4f4b5-133">displayName</span></span>|<span data-ttu-id="4f4b5-134">String</span><span class="sxs-lookup"><span data-stu-id="4f4b5-134">String</span></span>|<span data-ttu-id="4f4b5-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="4f4b5-136">description</span><span class="sxs-lookup"><span data-stu-id="4f4b5-136">description</span></span>|<span data-ttu-id="4f4b5-137">字符串</span><span class="sxs-lookup"><span data-stu-id="4f4b5-137">String</span></span>|<span data-ttu-id="4f4b5-138">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="4f4b5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f4b5-139">createdDateTime</span></span>|<span data-ttu-id="4f4b5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f4b5-140">DateTimeOffset</span></span>|<span data-ttu-id="4f4b5-141">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-141">The time the management condition was created.</span></span> <span data-ttu-id="4f4b5-142">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-142">Generated service side.</span></span>|
|<span data-ttu-id="4f4b5-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f4b5-143">modifiedDateTime</span></span>|<span data-ttu-id="4f4b5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f4b5-144">DateTimeOffset</span></span>|<span data-ttu-id="4f4b5-145">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-145">The time the management condition was last modified.</span></span> <span data-ttu-id="4f4b5-146">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-146">Updated service side.</span></span>|
|<span data-ttu-id="4f4b5-147">eTag</span><span class="sxs-lookup"><span data-stu-id="4f4b5-147">eTag</span></span>|<span data-ttu-id="4f4b5-148">String</span><span class="sxs-lookup"><span data-stu-id="4f4b5-148">String</span></span>|<span data-ttu-id="4f4b5-149">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-149">ETag of the management condition.</span></span> <span data-ttu-id="4f4b5-150">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-150">Updated service side.</span></span>|
|<span data-ttu-id="4f4b5-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="4f4b5-151">applicablePlatforms</span></span>|<span data-ttu-id="4f4b5-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f4b5-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="4f4b5-153">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f4b5-154">关系</span><span class="sxs-lookup"><span data-stu-id="4f4b5-154">Relationships</span></span>
|<span data-ttu-id="4f4b5-155">关系</span><span class="sxs-lookup"><span data-stu-id="4f4b5-155">Relationship</span></span>|<span data-ttu-id="4f4b5-156">类型</span><span class="sxs-lookup"><span data-stu-id="4f4b5-156">Type</span></span>|<span data-ttu-id="4f4b5-157">说明</span><span class="sxs-lookup"><span data-stu-id="4f4b5-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f4b5-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="4f4b5-158">managementConditionStatements</span></span>|<span data-ttu-id="4f4b5-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f4b5-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="4f4b5-160">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f4b5-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f4b5-161">JSON Representation</span></span>
<span data-ttu-id="4f4b5-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f4b5-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



