---
title: circularGeofenceManagementCondition 资源类型
description: 包含用于定义圆形地域防护管理条件（要监视的感兴趣的区域）的信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a62787fb8cdfffb81ede87f9881ede576af7fffe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031401"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a><span data-ttu-id="13a4d-103">circularGeofenceManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="13a4d-103">circularGeofenceManagementCondition resource type</span></span>

<span data-ttu-id="13a4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13a4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13a4d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13a4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13a4d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13a4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a4d-107">包含用于定义圆形地域防护管理条件（要监视的感兴趣的区域）的信息。</span><span class="sxs-lookup"><span data-stu-id="13a4d-107">Contains the information to define a circular geo-fence management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="13a4d-108">继承自 [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-108">Inherits from [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="13a4d-109">方法</span><span class="sxs-lookup"><span data-stu-id="13a4d-109">Methods</span></span>
|<span data-ttu-id="13a4d-110">方法</span><span class="sxs-lookup"><span data-stu-id="13a4d-110">Method</span></span>|<span data-ttu-id="13a4d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="13a4d-111">Return Type</span></span>|<span data-ttu-id="13a4d-112">说明</span><span class="sxs-lookup"><span data-stu-id="13a4d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13a4d-113">列出 circularGeofenceManagementConditions</span><span class="sxs-lookup"><span data-stu-id="13a4d-113">List circularGeofenceManagementConditions</span></span>](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|<span data-ttu-id="13a4d-114">[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13a4d-114">[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) collection</span></span>|<span data-ttu-id="13a4d-115">列出 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13a4d-115">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="13a4d-116">获取 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-116">Get circularGeofenceManagementCondition</span></span>](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[<span data-ttu-id="13a4d-117">circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-117">circularGeofenceManagementCondition</span></span>](../resources/intune-fencing-circulargeofencemanagementcondition.md)|<span data-ttu-id="13a4d-118">读取 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13a4d-118">Read properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>|
|[<span data-ttu-id="13a4d-119">创建 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-119">Create circularGeofenceManagementCondition</span></span>](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[<span data-ttu-id="13a4d-120">circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-120">circularGeofenceManagementCondition</span></span>](../resources/intune-fencing-circulargeofencemanagementcondition.md)|<span data-ttu-id="13a4d-121">创建新的 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13a4d-121">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>|
|[<span data-ttu-id="13a4d-122">删除 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-122">Delete circularGeofenceManagementCondition</span></span>](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|<span data-ttu-id="13a4d-123">无</span><span class="sxs-lookup"><span data-stu-id="13a4d-123">None</span></span>|<span data-ttu-id="13a4d-124">删除 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="13a4d-124">Deletes a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>|
|[<span data-ttu-id="13a4d-125">更新 circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-125">Update circularGeofenceManagementCondition</span></span>](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[<span data-ttu-id="13a4d-126">circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="13a4d-126">circularGeofenceManagementCondition</span></span>](../resources/intune-fencing-circulargeofencemanagementcondition.md)|<span data-ttu-id="13a4d-127">更新 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13a4d-127">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13a4d-128">属性</span><span class="sxs-lookup"><span data-stu-id="13a4d-128">Properties</span></span>
|<span data-ttu-id="13a4d-129">属性</span><span class="sxs-lookup"><span data-stu-id="13a4d-129">Property</span></span>|<span data-ttu-id="13a4d-130">类型</span><span class="sxs-lookup"><span data-stu-id="13a4d-130">Type</span></span>|<span data-ttu-id="13a4d-131">说明</span><span class="sxs-lookup"><span data-stu-id="13a4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a4d-132">id</span><span class="sxs-lookup"><span data-stu-id="13a4d-132">id</span></span>|<span data-ttu-id="13a4d-133">String</span><span class="sxs-lookup"><span data-stu-id="13a4d-133">String</span></span>|<span data-ttu-id="13a4d-134">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="13a4d-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="13a4d-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="13a4d-135">System generated value assigned when created.</span></span> <span data-ttu-id="13a4d-136">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="13a4d-137">uniqueName</span></span>|<span data-ttu-id="13a4d-138">String</span><span class="sxs-lookup"><span data-stu-id="13a4d-138">String</span></span>|<span data-ttu-id="13a4d-139">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="13a4d-139">Unique name for the management condition.</span></span> <span data-ttu-id="13a4d-140">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="13a4d-140">Used in management condition expressions.</span></span> <span data-ttu-id="13a4d-141">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="13a4d-142">displayName</span></span>|<span data-ttu-id="13a4d-143">String</span><span class="sxs-lookup"><span data-stu-id="13a4d-143">String</span></span>|<span data-ttu-id="13a4d-144">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="13a4d-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="13a4d-145">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-146">description</span><span class="sxs-lookup"><span data-stu-id="13a4d-146">description</span></span>|<span data-ttu-id="13a4d-147">String</span><span class="sxs-lookup"><span data-stu-id="13a4d-147">String</span></span>|<span data-ttu-id="13a4d-148">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="13a4d-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="13a4d-149">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13a4d-150">createdDateTime</span></span>|<span data-ttu-id="13a4d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13a4d-151">DateTimeOffset</span></span>|<span data-ttu-id="13a4d-152">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="13a4d-152">The time the management condition was created.</span></span> <span data-ttu-id="13a4d-153">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="13a4d-153">Generated service side.</span></span> <span data-ttu-id="13a4d-154">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13a4d-155">modifiedDateTime</span></span>|<span data-ttu-id="13a4d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13a4d-156">DateTimeOffset</span></span>|<span data-ttu-id="13a4d-157">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="13a4d-157">The time the management condition was last modified.</span></span> <span data-ttu-id="13a4d-158">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="13a4d-158">Updated service side.</span></span> <span data-ttu-id="13a4d-159">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-160">eTag</span><span class="sxs-lookup"><span data-stu-id="13a4d-160">eTag</span></span>|<span data-ttu-id="13a4d-161">String</span><span class="sxs-lookup"><span data-stu-id="13a4d-161">String</span></span>|<span data-ttu-id="13a4d-162">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="13a4d-162">ETag of the management condition.</span></span> <span data-ttu-id="13a4d-163">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="13a4d-163">Updated service side.</span></span> <span data-ttu-id="13a4d-164">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="13a4d-165">applicablePlatforms</span></span>|<span data-ttu-id="13a4d-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13a4d-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="13a4d-167">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="13a4d-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="13a4d-168">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="13a4d-169">latitude</span><span class="sxs-lookup"><span data-stu-id="13a4d-169">latitude</span></span>|<span data-ttu-id="13a4d-170">Double</span><span class="sxs-lookup"><span data-stu-id="13a4d-170">Double</span></span>|<span data-ttu-id="13a4d-171">以度为单位的纬度，介于-90 和 + 90 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="13a4d-171">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="13a4d-172">longitude</span><span class="sxs-lookup"><span data-stu-id="13a4d-172">longitude</span></span>|<span data-ttu-id="13a4d-173">Double</span><span class="sxs-lookup"><span data-stu-id="13a4d-173">Double</span></span>|<span data-ttu-id="13a4d-174">以度为单位的经度，介于-180 和 + 180 之间（含）。</span><span class="sxs-lookup"><span data-stu-id="13a4d-174">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="13a4d-175">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="13a4d-175">radiusInMeters</span></span>|<span data-ttu-id="13a4d-176">单一</span><span class="sxs-lookup"><span data-stu-id="13a4d-176">Single</span></span>|<span data-ttu-id="13a4d-177">以米为单位的半径。</span><span class="sxs-lookup"><span data-stu-id="13a4d-177">Radius in meters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13a4d-178">关系</span><span class="sxs-lookup"><span data-stu-id="13a4d-178">Relationships</span></span>
|<span data-ttu-id="13a4d-179">关系</span><span class="sxs-lookup"><span data-stu-id="13a4d-179">Relationship</span></span>|<span data-ttu-id="13a4d-180">类型</span><span class="sxs-lookup"><span data-stu-id="13a4d-180">Type</span></span>|<span data-ttu-id="13a4d-181">说明</span><span class="sxs-lookup"><span data-stu-id="13a4d-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a4d-182">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="13a4d-182">managementConditionStatements</span></span>|<span data-ttu-id="13a4d-183">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13a4d-183">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="13a4d-184">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="13a4d-184">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="13a4d-185">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="13a4d-185">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13a4d-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13a4d-186">JSON Representation</span></span>
<span data-ttu-id="13a4d-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13a4d-187">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "4.2",
  "longitude": "4.2",
  "radiusInMeters": 4.2
}
```






