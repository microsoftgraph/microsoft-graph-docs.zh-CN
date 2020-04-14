---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f49359a9c3e527e30944030a8c0969c7c12ce9e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382729"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="9df4e-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="9df4e-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="9df4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9df4e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9df4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9df4e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9df4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9df4e-107">包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。</span><span class="sxs-lookup"><span data-stu-id="9df4e-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="9df4e-108">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9df4e-109">方法</span><span class="sxs-lookup"><span data-stu-id="9df4e-109">Methods</span></span>
|<span data-ttu-id="9df4e-110">方法</span><span class="sxs-lookup"><span data-stu-id="9df4e-110">Method</span></span>|<span data-ttu-id="9df4e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9df4e-111">Return Type</span></span>|<span data-ttu-id="9df4e-112">说明</span><span class="sxs-lookup"><span data-stu-id="9df4e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9df4e-113">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="9df4e-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="9df4e-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="9df4e-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="9df4e-115">列出[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9df4e-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="9df4e-116">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9df4e-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="9df4e-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9df4e-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="9df4e-118">读取[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9df4e-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9df4e-119">属性</span><span class="sxs-lookup"><span data-stu-id="9df4e-119">Properties</span></span>
|<span data-ttu-id="9df4e-120">属性</span><span class="sxs-lookup"><span data-stu-id="9df4e-120">Property</span></span>|<span data-ttu-id="9df4e-121">类型</span><span class="sxs-lookup"><span data-stu-id="9df4e-121">Type</span></span>|<span data-ttu-id="9df4e-122">说明</span><span class="sxs-lookup"><span data-stu-id="9df4e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9df4e-123">id</span><span class="sxs-lookup"><span data-stu-id="9df4e-123">id</span></span>|<span data-ttu-id="9df4e-124">字符串</span><span class="sxs-lookup"><span data-stu-id="9df4e-124">String</span></span>|<span data-ttu-id="9df4e-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9df4e-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="9df4e-126">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="9df4e-126">System generated value assigned when created.</span></span> <span data-ttu-id="9df4e-127">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="9df4e-128">uniqueName</span></span>|<span data-ttu-id="9df4e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="9df4e-129">String</span></span>|<span data-ttu-id="9df4e-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="9df4e-130">Unique name for the management condition.</span></span> <span data-ttu-id="9df4e-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="9df4e-131">Used in management condition expressions.</span></span> <span data-ttu-id="9df4e-132">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9df4e-133">displayName</span></span>|<span data-ttu-id="9df4e-134">String</span><span class="sxs-lookup"><span data-stu-id="9df4e-134">String</span></span>|<span data-ttu-id="9df4e-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="9df4e-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="9df4e-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-137">description</span><span class="sxs-lookup"><span data-stu-id="9df4e-137">description</span></span>|<span data-ttu-id="9df4e-138">字符串</span><span class="sxs-lookup"><span data-stu-id="9df4e-138">String</span></span>|<span data-ttu-id="9df4e-139">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="9df4e-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="9df4e-140">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9df4e-141">createdDateTime</span></span>|<span data-ttu-id="9df4e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df4e-142">DateTimeOffset</span></span>|<span data-ttu-id="9df4e-143">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="9df4e-143">The time the management condition was created.</span></span> <span data-ttu-id="9df4e-144">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="9df4e-144">Generated service side.</span></span> <span data-ttu-id="9df4e-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9df4e-146">modifiedDateTime</span></span>|<span data-ttu-id="9df4e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df4e-147">DateTimeOffset</span></span>|<span data-ttu-id="9df4e-148">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="9df4e-148">The time the management condition was last modified.</span></span> <span data-ttu-id="9df4e-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="9df4e-149">Updated service side.</span></span> <span data-ttu-id="9df4e-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-151">eTag</span><span class="sxs-lookup"><span data-stu-id="9df4e-151">eTag</span></span>|<span data-ttu-id="9df4e-152">String</span><span class="sxs-lookup"><span data-stu-id="9df4e-152">String</span></span>|<span data-ttu-id="9df4e-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="9df4e-153">ETag of the management condition.</span></span> <span data-ttu-id="9df4e-154">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="9df4e-154">Updated service side.</span></span> <span data-ttu-id="9df4e-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9df4e-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="9df4e-156">applicablePlatforms</span></span>|<span data-ttu-id="9df4e-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="9df4e-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="9df4e-158">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="9df4e-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="9df4e-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9df4e-160">关系</span><span class="sxs-lookup"><span data-stu-id="9df4e-160">Relationships</span></span>
|<span data-ttu-id="9df4e-161">关系</span><span class="sxs-lookup"><span data-stu-id="9df4e-161">Relationship</span></span>|<span data-ttu-id="9df4e-162">类型</span><span class="sxs-lookup"><span data-stu-id="9df4e-162">Type</span></span>|<span data-ttu-id="9df4e-163">说明</span><span class="sxs-lookup"><span data-stu-id="9df4e-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9df4e-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="9df4e-164">managementConditionStatements</span></span>|<span data-ttu-id="9df4e-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="9df4e-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="9df4e-166">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="9df4e-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="9df4e-167">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9df4e-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9df4e-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9df4e-168">JSON Representation</span></span>
<span data-ttu-id="9df4e-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9df4e-169">Here is a JSON representation of the resource.</span></span>
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



