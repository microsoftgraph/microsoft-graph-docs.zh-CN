---
title: networkManagementCondition 资源类型
description: 包含定义网络管理条件的信息。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 00ccc045892290ff03e68a109ccc01c4d5dbf8a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927042"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="b9d8d-103">networkManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9d8d-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="b9d8d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9d8d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9d8d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9d8d-107">包含定义网络管理条件的信息。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="b9d8d-108">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b9d8d-109">方法</span><span class="sxs-lookup"><span data-stu-id="b9d8d-109">Methods</span></span>
|<span data-ttu-id="b9d8d-110">方法</span><span class="sxs-lookup"><span data-stu-id="b9d8d-110">Method</span></span>|<span data-ttu-id="b9d8d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9d8d-111">Return Type</span></span>|<span data-ttu-id="b9d8d-112">说明</span><span class="sxs-lookup"><span data-stu-id="b9d8d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9d8d-113">列表 networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="b9d8d-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="b9d8d-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9d8d-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="b9d8d-115">列出属性和[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="b9d8d-116">获取 networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b9d8d-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="b9d8d-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b9d8d-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="b9d8d-118">读取属性和[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9d8d-119">属性</span><span class="sxs-lookup"><span data-stu-id="b9d8d-119">Properties</span></span>
|<span data-ttu-id="b9d8d-120">属性</span><span class="sxs-lookup"><span data-stu-id="b9d8d-120">Property</span></span>|<span data-ttu-id="b9d8d-121">类型</span><span class="sxs-lookup"><span data-stu-id="b9d8d-121">Type</span></span>|<span data-ttu-id="b9d8d-122">说明</span><span class="sxs-lookup"><span data-stu-id="b9d8d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d8d-123">id</span><span class="sxs-lookup"><span data-stu-id="b9d8d-123">id</span></span>|<span data-ttu-id="b9d8d-124">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d8d-124">String</span></span>|<span data-ttu-id="b9d8d-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="b9d8d-126">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-126">System generated value assigned when created.</span></span> <span data-ttu-id="b9d8d-127">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-128">唯一名称</span><span class="sxs-lookup"><span data-stu-id="b9d8d-128">uniqueName</span></span>|<span data-ttu-id="b9d8d-129">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d8d-129">String</span></span>|<span data-ttu-id="b9d8d-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-130">Unique name for the management condition.</span></span> <span data-ttu-id="b9d8d-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-131">Used in management condition expressions.</span></span> <span data-ttu-id="b9d8d-132">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b9d8d-133">displayName</span></span>|<span data-ttu-id="b9d8d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d8d-134">String</span></span>|<span data-ttu-id="b9d8d-135">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="b9d8d-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-137">说明</span><span class="sxs-lookup"><span data-stu-id="b9d8d-137">description</span></span>|<span data-ttu-id="b9d8d-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d8d-138">String</span></span>|<span data-ttu-id="b9d8d-139">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="b9d8d-140">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9d8d-141">createdDateTime</span></span>|<span data-ttu-id="b9d8d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d8d-142">DateTimeOffset</span></span>|<span data-ttu-id="b9d8d-143">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-143">The time the management condition was created.</span></span> <span data-ttu-id="b9d8d-144">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-144">Generated service side.</span></span> <span data-ttu-id="b9d8d-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9d8d-146">modifiedDateTime</span></span>|<span data-ttu-id="b9d8d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d8d-147">DateTimeOffset</span></span>|<span data-ttu-id="b9d8d-148">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-148">The time the management condition was last modified.</span></span> <span data-ttu-id="b9d8d-149">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-149">Updated service side.</span></span> <span data-ttu-id="b9d8d-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-151">eTag</span><span class="sxs-lookup"><span data-stu-id="b9d8d-151">eTag</span></span>|<span data-ttu-id="b9d8d-152">String</span><span class="sxs-lookup"><span data-stu-id="b9d8d-152">String</span></span>|<span data-ttu-id="b9d8d-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-153">ETag of the management condition.</span></span> <span data-ttu-id="b9d8d-154">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-154">Updated service side.</span></span> <span data-ttu-id="b9d8d-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b9d8d-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b9d8d-156">applicablePlatforms</span></span>|<span data-ttu-id="b9d8d-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9d8d-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b9d8d-158">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b9d8d-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9d8d-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="b9d8d-160">Relationships</span></span>
|<span data-ttu-id="b9d8d-161">关系</span><span class="sxs-lookup"><span data-stu-id="b9d8d-161">Relationship</span></span>|<span data-ttu-id="b9d8d-162">类型</span><span class="sxs-lookup"><span data-stu-id="b9d8d-162">Type</span></span>|<span data-ttu-id="b9d8d-163">Description</span><span class="sxs-lookup"><span data-stu-id="b9d8d-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d8d-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="b9d8d-164">managementConditionStatements</span></span>|<span data-ttu-id="b9d8d-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9d8d-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="b9d8d-166">为管理 condition 相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="b9d8d-167">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b9d8d-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9d8d-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9d8d-168">JSON Representation</span></span>
<span data-ttu-id="b9d8d-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9d8d-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
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





