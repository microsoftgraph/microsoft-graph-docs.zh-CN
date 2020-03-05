---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbbeec236d51d7e7a21321ba0386a473312a4b05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524523"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="92dc4-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="92dc4-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="92dc4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="92dc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92dc4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92dc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92dc4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92dc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92dc4-107">包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。</span><span class="sxs-lookup"><span data-stu-id="92dc4-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="92dc4-108">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="92dc4-109">方法</span><span class="sxs-lookup"><span data-stu-id="92dc4-109">Methods</span></span>
|<span data-ttu-id="92dc4-110">方法</span><span class="sxs-lookup"><span data-stu-id="92dc4-110">Method</span></span>|<span data-ttu-id="92dc4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="92dc4-111">Return Type</span></span>|<span data-ttu-id="92dc4-112">说明</span><span class="sxs-lookup"><span data-stu-id="92dc4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92dc4-113">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="92dc4-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="92dc4-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="92dc4-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="92dc4-115">列出[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92dc4-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="92dc4-116">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="92dc4-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="92dc4-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="92dc4-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="92dc4-118">读取[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92dc4-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="92dc4-119">属性</span><span class="sxs-lookup"><span data-stu-id="92dc4-119">Properties</span></span>
|<span data-ttu-id="92dc4-120">属性</span><span class="sxs-lookup"><span data-stu-id="92dc4-120">Property</span></span>|<span data-ttu-id="92dc4-121">类型</span><span class="sxs-lookup"><span data-stu-id="92dc4-121">Type</span></span>|<span data-ttu-id="92dc4-122">说明</span><span class="sxs-lookup"><span data-stu-id="92dc4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92dc4-123">id</span><span class="sxs-lookup"><span data-stu-id="92dc4-123">id</span></span>|<span data-ttu-id="92dc4-124">字符串</span><span class="sxs-lookup"><span data-stu-id="92dc4-124">String</span></span>|<span data-ttu-id="92dc4-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="92dc4-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="92dc4-126">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="92dc4-126">System generated value assigned when created.</span></span> <span data-ttu-id="92dc4-127">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="92dc4-128">uniqueName</span></span>|<span data-ttu-id="92dc4-129">String</span><span class="sxs-lookup"><span data-stu-id="92dc4-129">String</span></span>|<span data-ttu-id="92dc4-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="92dc4-130">Unique name for the management condition.</span></span> <span data-ttu-id="92dc4-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="92dc4-131">Used in management condition expressions.</span></span> <span data-ttu-id="92dc4-132">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="92dc4-133">displayName</span></span>|<span data-ttu-id="92dc4-134">String</span><span class="sxs-lookup"><span data-stu-id="92dc4-134">String</span></span>|<span data-ttu-id="92dc4-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="92dc4-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="92dc4-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-137">说明</span><span class="sxs-lookup"><span data-stu-id="92dc4-137">description</span></span>|<span data-ttu-id="92dc4-138">字符串</span><span class="sxs-lookup"><span data-stu-id="92dc4-138">String</span></span>|<span data-ttu-id="92dc4-139">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="92dc4-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="92dc4-140">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92dc4-141">createdDateTime</span></span>|<span data-ttu-id="92dc4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92dc4-142">DateTimeOffset</span></span>|<span data-ttu-id="92dc4-143">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="92dc4-143">The time the management condition was created.</span></span> <span data-ttu-id="92dc4-144">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="92dc4-144">Generated service side.</span></span> <span data-ttu-id="92dc4-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92dc4-146">modifiedDateTime</span></span>|<span data-ttu-id="92dc4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92dc4-147">DateTimeOffset</span></span>|<span data-ttu-id="92dc4-148">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="92dc4-148">The time the management condition was last modified.</span></span> <span data-ttu-id="92dc4-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="92dc4-149">Updated service side.</span></span> <span data-ttu-id="92dc4-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-151">eTag</span><span class="sxs-lookup"><span data-stu-id="92dc4-151">eTag</span></span>|<span data-ttu-id="92dc4-152">String</span><span class="sxs-lookup"><span data-stu-id="92dc4-152">String</span></span>|<span data-ttu-id="92dc4-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="92dc4-153">ETag of the management condition.</span></span> <span data-ttu-id="92dc4-154">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="92dc4-154">Updated service side.</span></span> <span data-ttu-id="92dc4-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="92dc4-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="92dc4-156">applicablePlatforms</span></span>|<span data-ttu-id="92dc4-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="92dc4-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="92dc4-158">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="92dc4-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="92dc4-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="92dc4-160">关系</span><span class="sxs-lookup"><span data-stu-id="92dc4-160">Relationships</span></span>
|<span data-ttu-id="92dc4-161">关系</span><span class="sxs-lookup"><span data-stu-id="92dc4-161">Relationship</span></span>|<span data-ttu-id="92dc4-162">类型</span><span class="sxs-lookup"><span data-stu-id="92dc4-162">Type</span></span>|<span data-ttu-id="92dc4-163">说明</span><span class="sxs-lookup"><span data-stu-id="92dc4-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92dc4-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="92dc4-164">managementConditionStatements</span></span>|<span data-ttu-id="92dc4-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="92dc4-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="92dc4-166">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="92dc4-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="92dc4-167">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="92dc4-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92dc4-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92dc4-168">JSON Representation</span></span>
<span data-ttu-id="92dc4-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92dc4-169">Here is a JSON representation of the resource.</span></span>
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



