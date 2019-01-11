---
title: locationManagementCondition 资源类型
description: 包含定义位置管理条件，感兴趣，要监视的领域的信息。
localization_priority: Normal
ms.openlocfilehash: 85d3b638c81990a98623501b8dcb3ad0705f2e6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832632"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="6bc81-103">locationManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bc81-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="6bc81-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6bc81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bc81-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6bc81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bc81-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6bc81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bc81-107">包含定义位置管理条件，感兴趣，要监视的领域的信息。</span><span class="sxs-lookup"><span data-stu-id="6bc81-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>

<span data-ttu-id="6bc81-108">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6bc81-109">方法</span><span class="sxs-lookup"><span data-stu-id="6bc81-109">Methods</span></span>
|<span data-ttu-id="6bc81-110">方法</span><span class="sxs-lookup"><span data-stu-id="6bc81-110">Method</span></span>|<span data-ttu-id="6bc81-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6bc81-111">Return Type</span></span>|<span data-ttu-id="6bc81-112">说明</span><span class="sxs-lookup"><span data-stu-id="6bc81-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bc81-113">列表 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="6bc81-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="6bc81-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bc81-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="6bc81-115">列出属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="6bc81-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="6bc81-116">获取 locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="6bc81-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="6bc81-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="6bc81-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="6bc81-118">读取属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="6bc81-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bc81-119">属性</span><span class="sxs-lookup"><span data-stu-id="6bc81-119">Properties</span></span>
|<span data-ttu-id="6bc81-120">属性</span><span class="sxs-lookup"><span data-stu-id="6bc81-120">Property</span></span>|<span data-ttu-id="6bc81-121">类型</span><span class="sxs-lookup"><span data-stu-id="6bc81-121">Type</span></span>|<span data-ttu-id="6bc81-122">说明</span><span class="sxs-lookup"><span data-stu-id="6bc81-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc81-123">id</span><span class="sxs-lookup"><span data-stu-id="6bc81-123">id</span></span>|<span data-ttu-id="6bc81-124">字符串</span><span class="sxs-lookup"><span data-stu-id="6bc81-124">String</span></span>|<span data-ttu-id="6bc81-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6bc81-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="6bc81-126">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="6bc81-126">System generated value assigned when created.</span></span> <span data-ttu-id="6bc81-127">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-128">唯一名称</span><span class="sxs-lookup"><span data-stu-id="6bc81-128">uniqueName</span></span>|<span data-ttu-id="6bc81-129">字符串</span><span class="sxs-lookup"><span data-stu-id="6bc81-129">String</span></span>|<span data-ttu-id="6bc81-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="6bc81-130">Unique name for the management condition.</span></span> <span data-ttu-id="6bc81-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="6bc81-131">Used in management condition expressions.</span></span> <span data-ttu-id="6bc81-132">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6bc81-133">displayName</span></span>|<span data-ttu-id="6bc81-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6bc81-134">String</span></span>|<span data-ttu-id="6bc81-135">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="6bc81-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="6bc81-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-137">说明</span><span class="sxs-lookup"><span data-stu-id="6bc81-137">description</span></span>|<span data-ttu-id="6bc81-138">字符串</span><span class="sxs-lookup"><span data-stu-id="6bc81-138">String</span></span>|<span data-ttu-id="6bc81-139">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="6bc81-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="6bc81-140">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc81-141">createdDateTime</span></span>|<span data-ttu-id="6bc81-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc81-142">DateTimeOffset</span></span>|<span data-ttu-id="6bc81-143">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="6bc81-143">The time the management condition was created.</span></span> <span data-ttu-id="6bc81-144">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="6bc81-144">Generated service side.</span></span> <span data-ttu-id="6bc81-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc81-146">modifiedDateTime</span></span>|<span data-ttu-id="6bc81-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc81-147">DateTimeOffset</span></span>|<span data-ttu-id="6bc81-148">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="6bc81-148">The time the management condition was last modified.</span></span> <span data-ttu-id="6bc81-149">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="6bc81-149">Updated service side.</span></span> <span data-ttu-id="6bc81-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-151">eTag</span><span class="sxs-lookup"><span data-stu-id="6bc81-151">eTag</span></span>|<span data-ttu-id="6bc81-152">String</span><span class="sxs-lookup"><span data-stu-id="6bc81-152">String</span></span>|<span data-ttu-id="6bc81-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="6bc81-153">ETag of the management condition.</span></span> <span data-ttu-id="6bc81-154">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="6bc81-154">Updated service side.</span></span> <span data-ttu-id="6bc81-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6bc81-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="6bc81-156">applicablePlatforms</span></span>|<span data-ttu-id="6bc81-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bc81-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="6bc81-158">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="6bc81-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="6bc81-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bc81-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="6bc81-160">Relationships</span></span>
|<span data-ttu-id="6bc81-161">关系</span><span class="sxs-lookup"><span data-stu-id="6bc81-161">Relationship</span></span>|<span data-ttu-id="6bc81-162">类型</span><span class="sxs-lookup"><span data-stu-id="6bc81-162">Type</span></span>|<span data-ttu-id="6bc81-163">Description</span><span class="sxs-lookup"><span data-stu-id="6bc81-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc81-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="6bc81-164">managementConditionStatements</span></span>|<span data-ttu-id="6bc81-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bc81-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="6bc81-166">为管理 condition 相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="6bc81-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="6bc81-167">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6bc81-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bc81-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bc81-168">JSON Representation</span></span>
<span data-ttu-id="6bc81-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bc81-169">Here is a JSON representation of the resource.</span></span>
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





