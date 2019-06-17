---
title: networkManagementCondition 资源类型
description: 包含用于定义网络管理条件的信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46e32312dc501219d887fcebb5da435ad2690031
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987738"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="aae02-103">networkManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="aae02-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="aae02-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aae02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aae02-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aae02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aae02-106">包含用于定义网络管理条件的信息。</span><span class="sxs-lookup"><span data-stu-id="aae02-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="aae02-107">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="aae02-108">方法</span><span class="sxs-lookup"><span data-stu-id="aae02-108">Methods</span></span>
|<span data-ttu-id="aae02-109">方法</span><span class="sxs-lookup"><span data-stu-id="aae02-109">Method</span></span>|<span data-ttu-id="aae02-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="aae02-110">Return Type</span></span>|<span data-ttu-id="aae02-111">说明</span><span class="sxs-lookup"><span data-stu-id="aae02-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aae02-112">列出 networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="aae02-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="aae02-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="aae02-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="aae02-114">列出[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aae02-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="aae02-115">获取 networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="aae02-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="aae02-116">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="aae02-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="aae02-117">读取[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aae02-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aae02-118">属性</span><span class="sxs-lookup"><span data-stu-id="aae02-118">Properties</span></span>
|<span data-ttu-id="aae02-119">属性</span><span class="sxs-lookup"><span data-stu-id="aae02-119">Property</span></span>|<span data-ttu-id="aae02-120">类型</span><span class="sxs-lookup"><span data-stu-id="aae02-120">Type</span></span>|<span data-ttu-id="aae02-121">说明</span><span class="sxs-lookup"><span data-stu-id="aae02-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae02-122">id</span><span class="sxs-lookup"><span data-stu-id="aae02-122">id</span></span>|<span data-ttu-id="aae02-123">字符串</span><span class="sxs-lookup"><span data-stu-id="aae02-123">String</span></span>|<span data-ttu-id="aae02-124">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aae02-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="aae02-125">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="aae02-125">System generated value assigned when created.</span></span> <span data-ttu-id="aae02-126">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="aae02-127">uniqueName</span></span>|<span data-ttu-id="aae02-128">String</span><span class="sxs-lookup"><span data-stu-id="aae02-128">String</span></span>|<span data-ttu-id="aae02-129">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="aae02-129">Unique name for the management condition.</span></span> <span data-ttu-id="aae02-130">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="aae02-130">Used in management condition expressions.</span></span> <span data-ttu-id="aae02-131">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-132">displayName</span><span class="sxs-lookup"><span data-stu-id="aae02-132">displayName</span></span>|<span data-ttu-id="aae02-133">String</span><span class="sxs-lookup"><span data-stu-id="aae02-133">String</span></span>|<span data-ttu-id="aae02-134">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="aae02-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="aae02-135">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-136">说明</span><span class="sxs-lookup"><span data-stu-id="aae02-136">description</span></span>|<span data-ttu-id="aae02-137">字符串</span><span class="sxs-lookup"><span data-stu-id="aae02-137">String</span></span>|<span data-ttu-id="aae02-138">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="aae02-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="aae02-139">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aae02-140">createdDateTime</span></span>|<span data-ttu-id="aae02-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae02-141">DateTimeOffset</span></span>|<span data-ttu-id="aae02-142">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="aae02-142">The time the management condition was created.</span></span> <span data-ttu-id="aae02-143">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="aae02-143">Generated service side.</span></span> <span data-ttu-id="aae02-144">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aae02-145">modifiedDateTime</span></span>|<span data-ttu-id="aae02-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae02-146">DateTimeOffset</span></span>|<span data-ttu-id="aae02-147">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="aae02-147">The time the management condition was last modified.</span></span> <span data-ttu-id="aae02-148">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="aae02-148">Updated service side.</span></span> <span data-ttu-id="aae02-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-150">eTag</span><span class="sxs-lookup"><span data-stu-id="aae02-150">eTag</span></span>|<span data-ttu-id="aae02-151">String</span><span class="sxs-lookup"><span data-stu-id="aae02-151">String</span></span>|<span data-ttu-id="aae02-152">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="aae02-152">ETag of the management condition.</span></span> <span data-ttu-id="aae02-153">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="aae02-153">Updated service side.</span></span> <span data-ttu-id="aae02-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aae02-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="aae02-155">applicablePlatforms</span></span>|<span data-ttu-id="aae02-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="aae02-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="aae02-157">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="aae02-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="aae02-158">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="aae02-159">关系</span><span class="sxs-lookup"><span data-stu-id="aae02-159">Relationships</span></span>
|<span data-ttu-id="aae02-160">关系</span><span class="sxs-lookup"><span data-stu-id="aae02-160">Relationship</span></span>|<span data-ttu-id="aae02-161">类型</span><span class="sxs-lookup"><span data-stu-id="aae02-161">Type</span></span>|<span data-ttu-id="aae02-162">说明</span><span class="sxs-lookup"><span data-stu-id="aae02-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae02-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="aae02-163">managementConditionStatements</span></span>|<span data-ttu-id="aae02-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="aae02-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="aae02-165">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="aae02-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="aae02-166">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aae02-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aae02-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aae02-167">JSON Representation</span></span>
<span data-ttu-id="aae02-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aae02-168">Here is a JSON representation of the resource.</span></span>
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





