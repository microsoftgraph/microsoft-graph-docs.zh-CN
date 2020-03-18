---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56e9c10d8d9d53a9e0009b6a70210da6d7873065
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783254"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="7e4da-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e4da-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="7e4da-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e4da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e4da-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e4da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e4da-106">包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。</span><span class="sxs-lookup"><span data-stu-id="7e4da-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="7e4da-107">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7e4da-108">方法</span><span class="sxs-lookup"><span data-stu-id="7e4da-108">Methods</span></span>
|<span data-ttu-id="7e4da-109">方法</span><span class="sxs-lookup"><span data-stu-id="7e4da-109">Method</span></span>|<span data-ttu-id="7e4da-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e4da-110">Return Type</span></span>|<span data-ttu-id="7e4da-111">说明</span><span class="sxs-lookup"><span data-stu-id="7e4da-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e4da-112">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="7e4da-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="7e4da-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e4da-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="7e4da-114">列出[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e4da-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="7e4da-115">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="7e4da-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="7e4da-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="7e4da-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="7e4da-117">读取[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e4da-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e4da-118">属性</span><span class="sxs-lookup"><span data-stu-id="7e4da-118">Properties</span></span>
|<span data-ttu-id="7e4da-119">属性</span><span class="sxs-lookup"><span data-stu-id="7e4da-119">Property</span></span>|<span data-ttu-id="7e4da-120">类型</span><span class="sxs-lookup"><span data-stu-id="7e4da-120">Type</span></span>|<span data-ttu-id="7e4da-121">说明</span><span class="sxs-lookup"><span data-stu-id="7e4da-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e4da-122">id</span><span class="sxs-lookup"><span data-stu-id="7e4da-122">id</span></span>|<span data-ttu-id="7e4da-123">字符串</span><span class="sxs-lookup"><span data-stu-id="7e4da-123">String</span></span>|<span data-ttu-id="7e4da-124">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7e4da-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="7e4da-125">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="7e4da-125">System generated value assigned when created.</span></span> <span data-ttu-id="7e4da-126">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="7e4da-127">uniqueName</span></span>|<span data-ttu-id="7e4da-128">String</span><span class="sxs-lookup"><span data-stu-id="7e4da-128">String</span></span>|<span data-ttu-id="7e4da-129">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="7e4da-129">Unique name for the management condition.</span></span> <span data-ttu-id="7e4da-130">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="7e4da-130">Used in management condition expressions.</span></span> <span data-ttu-id="7e4da-131">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7e4da-132">displayName</span></span>|<span data-ttu-id="7e4da-133">String</span><span class="sxs-lookup"><span data-stu-id="7e4da-133">String</span></span>|<span data-ttu-id="7e4da-134">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="7e4da-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="7e4da-135">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-136">说明</span><span class="sxs-lookup"><span data-stu-id="7e4da-136">description</span></span>|<span data-ttu-id="7e4da-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7e4da-137">String</span></span>|<span data-ttu-id="7e4da-138">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="7e4da-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="7e4da-139">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e4da-140">createdDateTime</span></span>|<span data-ttu-id="7e4da-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e4da-141">DateTimeOffset</span></span>|<span data-ttu-id="7e4da-142">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="7e4da-142">The time the management condition was created.</span></span> <span data-ttu-id="7e4da-143">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="7e4da-143">Generated service side.</span></span> <span data-ttu-id="7e4da-144">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e4da-145">modifiedDateTime</span></span>|<span data-ttu-id="7e4da-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e4da-146">DateTimeOffset</span></span>|<span data-ttu-id="7e4da-147">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="7e4da-147">The time the management condition was last modified.</span></span> <span data-ttu-id="7e4da-148">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="7e4da-148">Updated service side.</span></span> <span data-ttu-id="7e4da-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-150">eTag</span><span class="sxs-lookup"><span data-stu-id="7e4da-150">eTag</span></span>|<span data-ttu-id="7e4da-151">String</span><span class="sxs-lookup"><span data-stu-id="7e4da-151">String</span></span>|<span data-ttu-id="7e4da-152">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="7e4da-152">ETag of the management condition.</span></span> <span data-ttu-id="7e4da-153">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="7e4da-153">Updated service side.</span></span> <span data-ttu-id="7e4da-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7e4da-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="7e4da-155">applicablePlatforms</span></span>|<span data-ttu-id="7e4da-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e4da-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="7e4da-157">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="7e4da-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="7e4da-158">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e4da-159">关系</span><span class="sxs-lookup"><span data-stu-id="7e4da-159">Relationships</span></span>
|<span data-ttu-id="7e4da-160">关系</span><span class="sxs-lookup"><span data-stu-id="7e4da-160">Relationship</span></span>|<span data-ttu-id="7e4da-161">类型</span><span class="sxs-lookup"><span data-stu-id="7e4da-161">Type</span></span>|<span data-ttu-id="7e4da-162">说明</span><span class="sxs-lookup"><span data-stu-id="7e4da-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e4da-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="7e4da-163">managementConditionStatements</span></span>|<span data-ttu-id="7e4da-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e4da-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="7e4da-165">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="7e4da-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="7e4da-166">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7e4da-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e4da-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e4da-167">JSON Representation</span></span>
<span data-ttu-id="7e4da-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e4da-168">Here is a JSON representation of the resource.</span></span>
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



