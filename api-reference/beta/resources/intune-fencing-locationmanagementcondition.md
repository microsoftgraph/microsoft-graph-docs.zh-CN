---
title: locationManagementCondition 资源类型
description: 包含定义位置管理条件，感兴趣，要监视的领域的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c2eddf43696bd9300cc8dcd3408dbcd6fc5a9e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422794"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="3de55-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="3de55-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="3de55-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3de55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3de55-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3de55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3de55-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3de55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de55-107">包含定义位置管理条件，感兴趣，要监视的领域的信息。</span><span class="sxs-lookup"><span data-stu-id="3de55-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="3de55-108">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3de55-109">方法</span><span class="sxs-lookup"><span data-stu-id="3de55-109">Methods</span></span>
|<span data-ttu-id="3de55-110">方法</span><span class="sxs-lookup"><span data-stu-id="3de55-110">Method</span></span>|<span data-ttu-id="3de55-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3de55-111">Return Type</span></span>|<span data-ttu-id="3de55-112">说明</span><span class="sxs-lookup"><span data-stu-id="3de55-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3de55-113">列表 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="3de55-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="3de55-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="3de55-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="3de55-115">列出属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="3de55-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="3de55-116">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="3de55-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="3de55-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="3de55-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="3de55-118">读取属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="3de55-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3de55-119">属性</span><span class="sxs-lookup"><span data-stu-id="3de55-119">Properties</span></span>
|<span data-ttu-id="3de55-120">属性</span><span class="sxs-lookup"><span data-stu-id="3de55-120">Property</span></span>|<span data-ttu-id="3de55-121">类型</span><span class="sxs-lookup"><span data-stu-id="3de55-121">Type</span></span>|<span data-ttu-id="3de55-122">说明</span><span class="sxs-lookup"><span data-stu-id="3de55-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de55-123">id</span><span class="sxs-lookup"><span data-stu-id="3de55-123">id</span></span>|<span data-ttu-id="3de55-124">String</span><span class="sxs-lookup"><span data-stu-id="3de55-124">String</span></span>|<span data-ttu-id="3de55-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3de55-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="3de55-126">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="3de55-126">System generated value assigned when created.</span></span> <span data-ttu-id="3de55-127">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-128">唯一名称</span><span class="sxs-lookup"><span data-stu-id="3de55-128">uniqueName</span></span>|<span data-ttu-id="3de55-129">String</span><span class="sxs-lookup"><span data-stu-id="3de55-129">String</span></span>|<span data-ttu-id="3de55-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="3de55-130">Unique name for the management condition.</span></span> <span data-ttu-id="3de55-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="3de55-131">Used in management condition expressions.</span></span> <span data-ttu-id="3de55-132">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3de55-133">displayName</span></span>|<span data-ttu-id="3de55-134">String</span><span class="sxs-lookup"><span data-stu-id="3de55-134">String</span></span>|<span data-ttu-id="3de55-135">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="3de55-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="3de55-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-137">说明</span><span class="sxs-lookup"><span data-stu-id="3de55-137">description</span></span>|<span data-ttu-id="3de55-138">String</span><span class="sxs-lookup"><span data-stu-id="3de55-138">String</span></span>|<span data-ttu-id="3de55-139">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="3de55-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="3de55-140">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3de55-141">createdDateTime</span></span>|<span data-ttu-id="3de55-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de55-142">DateTimeOffset</span></span>|<span data-ttu-id="3de55-143">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="3de55-143">The time the management condition was created.</span></span> <span data-ttu-id="3de55-144">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="3de55-144">Generated service side.</span></span> <span data-ttu-id="3de55-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3de55-146">modifiedDateTime</span></span>|<span data-ttu-id="3de55-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de55-147">DateTimeOffset</span></span>|<span data-ttu-id="3de55-148">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="3de55-148">The time the management condition was last modified.</span></span> <span data-ttu-id="3de55-149">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="3de55-149">Updated service side.</span></span> <span data-ttu-id="3de55-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-151">eTag</span><span class="sxs-lookup"><span data-stu-id="3de55-151">eTag</span></span>|<span data-ttu-id="3de55-152">String</span><span class="sxs-lookup"><span data-stu-id="3de55-152">String</span></span>|<span data-ttu-id="3de55-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="3de55-153">ETag of the management condition.</span></span> <span data-ttu-id="3de55-154">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="3de55-154">Updated service side.</span></span> <span data-ttu-id="3de55-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3de55-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="3de55-156">applicablePlatforms</span></span>|<span data-ttu-id="3de55-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="3de55-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="3de55-158">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="3de55-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="3de55-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3de55-160">关系</span><span class="sxs-lookup"><span data-stu-id="3de55-160">Relationships</span></span>
|<span data-ttu-id="3de55-161">关系</span><span class="sxs-lookup"><span data-stu-id="3de55-161">Relationship</span></span>|<span data-ttu-id="3de55-162">类型</span><span class="sxs-lookup"><span data-stu-id="3de55-162">Type</span></span>|<span data-ttu-id="3de55-163">说明</span><span class="sxs-lookup"><span data-stu-id="3de55-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de55-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="3de55-164">managementConditionStatements</span></span>|<span data-ttu-id="3de55-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="3de55-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="3de55-166">为管理 condition 相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="3de55-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="3de55-167">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3de55-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3de55-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3de55-168">JSON Representation</span></span>
<span data-ttu-id="3de55-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3de55-169">Here is a JSON representation of the resource.</span></span>
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




