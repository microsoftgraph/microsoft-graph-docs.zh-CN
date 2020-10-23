---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e03e4c1d31fec4fbcff4f3f610710c1120a6a47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722878"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="cc8fe-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc8fe-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="cc8fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc8fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc8fe-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc8fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc8fe-107">包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="cc8fe-108">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cc8fe-109">Methods</span><span class="sxs-lookup"><span data-stu-id="cc8fe-109">Methods</span></span>
|<span data-ttu-id="cc8fe-110">方法</span><span class="sxs-lookup"><span data-stu-id="cc8fe-110">Method</span></span>|<span data-ttu-id="cc8fe-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc8fe-111">Return Type</span></span>|<span data-ttu-id="cc8fe-112">说明</span><span class="sxs-lookup"><span data-stu-id="cc8fe-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc8fe-113">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="cc8fe-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="cc8fe-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc8fe-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="cc8fe-115">列出 [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="cc8fe-116">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cc8fe-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="cc8fe-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cc8fe-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="cc8fe-118">读取 [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc8fe-119">属性</span><span class="sxs-lookup"><span data-stu-id="cc8fe-119">Properties</span></span>
|<span data-ttu-id="cc8fe-120">属性</span><span class="sxs-lookup"><span data-stu-id="cc8fe-120">Property</span></span>|<span data-ttu-id="cc8fe-121">类型</span><span class="sxs-lookup"><span data-stu-id="cc8fe-121">Type</span></span>|<span data-ttu-id="cc8fe-122">说明</span><span class="sxs-lookup"><span data-stu-id="cc8fe-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8fe-123">id</span><span class="sxs-lookup"><span data-stu-id="cc8fe-123">id</span></span>|<span data-ttu-id="cc8fe-124">String</span><span class="sxs-lookup"><span data-stu-id="cc8fe-124">String</span></span>|<span data-ttu-id="cc8fe-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="cc8fe-126">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-126">System generated value assigned when created.</span></span> <span data-ttu-id="cc8fe-127">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="cc8fe-128">uniqueName</span></span>|<span data-ttu-id="cc8fe-129">String</span><span class="sxs-lookup"><span data-stu-id="cc8fe-129">String</span></span>|<span data-ttu-id="cc8fe-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-130">Unique name for the management condition.</span></span> <span data-ttu-id="cc8fe-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-131">Used in management condition expressions.</span></span> <span data-ttu-id="cc8fe-132">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cc8fe-133">displayName</span></span>|<span data-ttu-id="cc8fe-134">String</span><span class="sxs-lookup"><span data-stu-id="cc8fe-134">String</span></span>|<span data-ttu-id="cc8fe-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="cc8fe-136">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-137">说明</span><span class="sxs-lookup"><span data-stu-id="cc8fe-137">description</span></span>|<span data-ttu-id="cc8fe-138">String</span><span class="sxs-lookup"><span data-stu-id="cc8fe-138">String</span></span>|<span data-ttu-id="cc8fe-139">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="cc8fe-140">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc8fe-141">createdDateTime</span></span>|<span data-ttu-id="cc8fe-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc8fe-142">DateTimeOffset</span></span>|<span data-ttu-id="cc8fe-143">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-143">The time the management condition was created.</span></span> <span data-ttu-id="cc8fe-144">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-144">Generated service side.</span></span> <span data-ttu-id="cc8fe-145">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc8fe-146">modifiedDateTime</span></span>|<span data-ttu-id="cc8fe-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc8fe-147">DateTimeOffset</span></span>|<span data-ttu-id="cc8fe-148">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-148">The time the management condition was last modified.</span></span> <span data-ttu-id="cc8fe-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-149">Updated service side.</span></span> <span data-ttu-id="cc8fe-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-151">eTag</span><span class="sxs-lookup"><span data-stu-id="cc8fe-151">eTag</span></span>|<span data-ttu-id="cc8fe-152">String</span><span class="sxs-lookup"><span data-stu-id="cc8fe-152">String</span></span>|<span data-ttu-id="cc8fe-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-153">ETag of the management condition.</span></span> <span data-ttu-id="cc8fe-154">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-154">Updated service side.</span></span> <span data-ttu-id="cc8fe-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc8fe-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cc8fe-156">applicablePlatforms</span></span>|<span data-ttu-id="cc8fe-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc8fe-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cc8fe-158">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="cc8fe-159">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc8fe-160">关系</span><span class="sxs-lookup"><span data-stu-id="cc8fe-160">Relationships</span></span>
|<span data-ttu-id="cc8fe-161">关系</span><span class="sxs-lookup"><span data-stu-id="cc8fe-161">Relationship</span></span>|<span data-ttu-id="cc8fe-162">类型</span><span class="sxs-lookup"><span data-stu-id="cc8fe-162">Type</span></span>|<span data-ttu-id="cc8fe-163">说明</span><span class="sxs-lookup"><span data-stu-id="cc8fe-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8fe-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="cc8fe-164">managementConditionStatements</span></span>|<span data-ttu-id="cc8fe-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc8fe-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="cc8fe-166">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="cc8fe-167">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc8fe-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc8fe-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc8fe-168">JSON Representation</span></span>
<span data-ttu-id="cc8fe-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc8fe-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
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





