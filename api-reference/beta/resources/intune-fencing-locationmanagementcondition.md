---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件 (要监视的感兴趣的区域) 的信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07bf05fa8ab6f7f7f1ce6e1978645f289ea57a2f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143307"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="56543-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="56543-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="56543-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56543-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56543-106">包含用于定义位置管理条件 (要监视的感兴趣的区域) 的信息。</span><span class="sxs-lookup"><span data-stu-id="56543-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="56543-107">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="56543-108">方法</span><span class="sxs-lookup"><span data-stu-id="56543-108">Methods</span></span>
|<span data-ttu-id="56543-109">方法</span><span class="sxs-lookup"><span data-stu-id="56543-109">Method</span></span>|<span data-ttu-id="56543-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="56543-110">Return Type</span></span>|<span data-ttu-id="56543-111">说明</span><span class="sxs-lookup"><span data-stu-id="56543-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56543-112">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="56543-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="56543-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="56543-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="56543-114">列出[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56543-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="56543-115">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="56543-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="56543-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="56543-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="56543-117">读取[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56543-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56543-118">属性</span><span class="sxs-lookup"><span data-stu-id="56543-118">Properties</span></span>
|<span data-ttu-id="56543-119">属性</span><span class="sxs-lookup"><span data-stu-id="56543-119">Property</span></span>|<span data-ttu-id="56543-120">类型</span><span class="sxs-lookup"><span data-stu-id="56543-120">Type</span></span>|<span data-ttu-id="56543-121">说明</span><span class="sxs-lookup"><span data-stu-id="56543-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56543-122">id</span><span class="sxs-lookup"><span data-stu-id="56543-122">id</span></span>|<span data-ttu-id="56543-123">字串符号</span><span class="sxs-lookup"><span data-stu-id="56543-123">String</span></span>|<span data-ttu-id="56543-124">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="56543-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="56543-125">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="56543-125">System generated value assigned when created.</span></span> <span data-ttu-id="56543-126">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="56543-127">uniqueName</span></span>|<span data-ttu-id="56543-128">字符串</span><span class="sxs-lookup"><span data-stu-id="56543-128">String</span></span>|<span data-ttu-id="56543-129">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="56543-129">Unique name for the management condition.</span></span> <span data-ttu-id="56543-130">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="56543-130">Used in management condition expressions.</span></span> <span data-ttu-id="56543-131">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-132">displayName</span><span class="sxs-lookup"><span data-stu-id="56543-132">displayName</span></span>|<span data-ttu-id="56543-133">字符串</span><span class="sxs-lookup"><span data-stu-id="56543-133">String</span></span>|<span data-ttu-id="56543-134">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="56543-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="56543-135">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-136">说明</span><span class="sxs-lookup"><span data-stu-id="56543-136">description</span></span>|<span data-ttu-id="56543-137">字符串</span><span class="sxs-lookup"><span data-stu-id="56543-137">String</span></span>|<span data-ttu-id="56543-138">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="56543-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="56543-139">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56543-140">createdDateTime</span></span>|<span data-ttu-id="56543-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56543-141">DateTimeOffset</span></span>|<span data-ttu-id="56543-142">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="56543-142">The time the management condition was created.</span></span> <span data-ttu-id="56543-143">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="56543-143">Generated service side.</span></span> <span data-ttu-id="56543-144">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56543-145">modifiedDateTime</span></span>|<span data-ttu-id="56543-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56543-146">DateTimeOffset</span></span>|<span data-ttu-id="56543-147">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="56543-147">The time the management condition was last modified.</span></span> <span data-ttu-id="56543-148">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="56543-148">Updated service side.</span></span> <span data-ttu-id="56543-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-150">eTag</span><span class="sxs-lookup"><span data-stu-id="56543-150">eTag</span></span>|<span data-ttu-id="56543-151">String</span><span class="sxs-lookup"><span data-stu-id="56543-151">String</span></span>|<span data-ttu-id="56543-152">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="56543-152">ETag of the management condition.</span></span> <span data-ttu-id="56543-153">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="56543-153">Updated service side.</span></span> <span data-ttu-id="56543-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="56543-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="56543-155">applicablePlatforms</span></span>|<span data-ttu-id="56543-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="56543-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="56543-157">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="56543-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="56543-158">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="56543-159">关系</span><span class="sxs-lookup"><span data-stu-id="56543-159">Relationships</span></span>
|<span data-ttu-id="56543-160">关系</span><span class="sxs-lookup"><span data-stu-id="56543-160">Relationship</span></span>|<span data-ttu-id="56543-161">类型</span><span class="sxs-lookup"><span data-stu-id="56543-161">Type</span></span>|<span data-ttu-id="56543-162">说明</span><span class="sxs-lookup"><span data-stu-id="56543-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56543-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="56543-163">managementConditionStatements</span></span>|<span data-ttu-id="56543-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="56543-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="56543-165">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="56543-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="56543-166">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="56543-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56543-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56543-167">JSON Representation</span></span>
<span data-ttu-id="56543-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56543-168">Here is a JSON representation of the resource.</span></span>
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




