---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 980c4b1e39c8804a8584d25d92acea2fc2c780dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031394"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="a9039-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9039-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="a9039-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9039-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9039-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9039-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9039-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9039-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9039-107">包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。</span><span class="sxs-lookup"><span data-stu-id="a9039-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="a9039-108">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a9039-109">方法</span><span class="sxs-lookup"><span data-stu-id="a9039-109">Methods</span></span>
|<span data-ttu-id="a9039-110">方法</span><span class="sxs-lookup"><span data-stu-id="a9039-110">Method</span></span>|<span data-ttu-id="a9039-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a9039-111">Return Type</span></span>|<span data-ttu-id="a9039-112">说明</span><span class="sxs-lookup"><span data-stu-id="a9039-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a9039-113">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="a9039-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="a9039-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9039-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="a9039-115">列出 [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9039-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="a9039-116">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a9039-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="a9039-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a9039-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="a9039-118">读取 [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9039-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9039-119">属性</span><span class="sxs-lookup"><span data-stu-id="a9039-119">Properties</span></span>
|<span data-ttu-id="a9039-120">属性</span><span class="sxs-lookup"><span data-stu-id="a9039-120">Property</span></span>|<span data-ttu-id="a9039-121">类型</span><span class="sxs-lookup"><span data-stu-id="a9039-121">Type</span></span>|<span data-ttu-id="a9039-122">说明</span><span class="sxs-lookup"><span data-stu-id="a9039-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9039-123">id</span><span class="sxs-lookup"><span data-stu-id="a9039-123">id</span></span>|<span data-ttu-id="a9039-124">String</span><span class="sxs-lookup"><span data-stu-id="a9039-124">String</span></span>|<span data-ttu-id="a9039-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a9039-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="a9039-126">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="a9039-126">System generated value assigned when created.</span></span> <span data-ttu-id="a9039-127">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="a9039-128">uniqueName</span></span>|<span data-ttu-id="a9039-129">String</span><span class="sxs-lookup"><span data-stu-id="a9039-129">String</span></span>|<span data-ttu-id="a9039-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="a9039-130">Unique name for the management condition.</span></span> <span data-ttu-id="a9039-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="a9039-131">Used in management condition expressions.</span></span> <span data-ttu-id="a9039-132">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a9039-133">displayName</span></span>|<span data-ttu-id="a9039-134">String</span><span class="sxs-lookup"><span data-stu-id="a9039-134">String</span></span>|<span data-ttu-id="a9039-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="a9039-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="a9039-136">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-137">description</span><span class="sxs-lookup"><span data-stu-id="a9039-137">description</span></span>|<span data-ttu-id="a9039-138">String</span><span class="sxs-lookup"><span data-stu-id="a9039-138">String</span></span>|<span data-ttu-id="a9039-139">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="a9039-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="a9039-140">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9039-141">createdDateTime</span></span>|<span data-ttu-id="a9039-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9039-142">DateTimeOffset</span></span>|<span data-ttu-id="a9039-143">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="a9039-143">The time the management condition was created.</span></span> <span data-ttu-id="a9039-144">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="a9039-144">Generated service side.</span></span> <span data-ttu-id="a9039-145">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9039-146">modifiedDateTime</span></span>|<span data-ttu-id="a9039-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9039-147">DateTimeOffset</span></span>|<span data-ttu-id="a9039-148">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="a9039-148">The time the management condition was last modified.</span></span> <span data-ttu-id="a9039-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="a9039-149">Updated service side.</span></span> <span data-ttu-id="a9039-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-151">eTag</span><span class="sxs-lookup"><span data-stu-id="a9039-151">eTag</span></span>|<span data-ttu-id="a9039-152">String</span><span class="sxs-lookup"><span data-stu-id="a9039-152">String</span></span>|<span data-ttu-id="a9039-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="a9039-153">ETag of the management condition.</span></span> <span data-ttu-id="a9039-154">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="a9039-154">Updated service side.</span></span> <span data-ttu-id="a9039-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a9039-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a9039-156">applicablePlatforms</span></span>|<span data-ttu-id="a9039-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9039-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a9039-158">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="a9039-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="a9039-159">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9039-160">关系</span><span class="sxs-lookup"><span data-stu-id="a9039-160">Relationships</span></span>
|<span data-ttu-id="a9039-161">关系</span><span class="sxs-lookup"><span data-stu-id="a9039-161">Relationship</span></span>|<span data-ttu-id="a9039-162">类型</span><span class="sxs-lookup"><span data-stu-id="a9039-162">Type</span></span>|<span data-ttu-id="a9039-163">说明</span><span class="sxs-lookup"><span data-stu-id="a9039-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9039-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="a9039-164">managementConditionStatements</span></span>|<span data-ttu-id="a9039-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a9039-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="a9039-166">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="a9039-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="a9039-167">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a9039-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9039-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9039-168">JSON Representation</span></span>
<span data-ttu-id="a9039-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9039-169">Here is a JSON representation of the resource.</span></span>
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






