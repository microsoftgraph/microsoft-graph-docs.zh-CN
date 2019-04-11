---
title: managementCondition 资源类型
description: 管理条件是可以动态触发的事件, 如地域时限、时限和网络时限。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b10442832d08507c3d33b71dd38928bc1be895d9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775245"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="751ce-103">managementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="751ce-103">managementCondition resource type</span></span>

> <span data-ttu-id="751ce-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="751ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="751ce-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="751ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="751ce-106">管理条件是可以动态触发的事件, 如地域时限、时限和网络时限。</span><span class="sxs-lookup"><span data-stu-id="751ce-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="751ce-107">方法</span><span class="sxs-lookup"><span data-stu-id="751ce-107">Methods</span></span>
|<span data-ttu-id="751ce-108">方法</span><span class="sxs-lookup"><span data-stu-id="751ce-108">Method</span></span>|<span data-ttu-id="751ce-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="751ce-109">Return Type</span></span>|<span data-ttu-id="751ce-110">说明</span><span class="sxs-lookup"><span data-stu-id="751ce-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="751ce-111">列出 managementConditions</span><span class="sxs-lookup"><span data-stu-id="751ce-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="751ce-112">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="751ce-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="751ce-113">列出[managementCondition](../resources/intune-fencing-managementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="751ce-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="751ce-114">获取 managementCondition</span><span class="sxs-lookup"><span data-stu-id="751ce-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="751ce-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="751ce-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="751ce-116">读取[managementCondition](../resources/intune-fencing-managementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="751ce-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="751ce-117">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="751ce-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="751ce-118">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="751ce-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="751ce-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="751ce-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="751ce-120">属性</span><span class="sxs-lookup"><span data-stu-id="751ce-120">Properties</span></span>
|<span data-ttu-id="751ce-121">属性</span><span class="sxs-lookup"><span data-stu-id="751ce-121">Property</span></span>|<span data-ttu-id="751ce-122">类型</span><span class="sxs-lookup"><span data-stu-id="751ce-122">Type</span></span>|<span data-ttu-id="751ce-123">说明</span><span class="sxs-lookup"><span data-stu-id="751ce-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751ce-124">id</span><span class="sxs-lookup"><span data-stu-id="751ce-124">id</span></span>|<span data-ttu-id="751ce-125">String</span><span class="sxs-lookup"><span data-stu-id="751ce-125">String</span></span>|<span data-ttu-id="751ce-126">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="751ce-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="751ce-127">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="751ce-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="751ce-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="751ce-128">uniqueName</span></span>|<span data-ttu-id="751ce-129">String</span><span class="sxs-lookup"><span data-stu-id="751ce-129">String</span></span>|<span data-ttu-id="751ce-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="751ce-130">Unique name for the management condition.</span></span> <span data-ttu-id="751ce-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="751ce-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="751ce-132">displayName</span><span class="sxs-lookup"><span data-stu-id="751ce-132">displayName</span></span>|<span data-ttu-id="751ce-133">String</span><span class="sxs-lookup"><span data-stu-id="751ce-133">String</span></span>|<span data-ttu-id="751ce-134">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="751ce-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="751ce-135">description</span><span class="sxs-lookup"><span data-stu-id="751ce-135">description</span></span>|<span data-ttu-id="751ce-136">字符串</span><span class="sxs-lookup"><span data-stu-id="751ce-136">String</span></span>|<span data-ttu-id="751ce-137">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="751ce-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="751ce-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="751ce-138">createdDateTime</span></span>|<span data-ttu-id="751ce-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751ce-139">DateTimeOffset</span></span>|<span data-ttu-id="751ce-140">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="751ce-140">The time the management condition was created.</span></span> <span data-ttu-id="751ce-141">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="751ce-141">Generated service side.</span></span>|
|<span data-ttu-id="751ce-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="751ce-142">modifiedDateTime</span></span>|<span data-ttu-id="751ce-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751ce-143">DateTimeOffset</span></span>|<span data-ttu-id="751ce-144">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="751ce-144">The time the management condition was last modified.</span></span> <span data-ttu-id="751ce-145">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="751ce-145">Updated service side.</span></span>|
|<span data-ttu-id="751ce-146">eTag</span><span class="sxs-lookup"><span data-stu-id="751ce-146">eTag</span></span>|<span data-ttu-id="751ce-147">String</span><span class="sxs-lookup"><span data-stu-id="751ce-147">String</span></span>|<span data-ttu-id="751ce-148">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="751ce-148">ETag of the management condition.</span></span> <span data-ttu-id="751ce-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="751ce-149">Updated service side.</span></span>|
|<span data-ttu-id="751ce-150">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="751ce-150">applicablePlatforms</span></span>|<span data-ttu-id="751ce-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="751ce-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="751ce-152">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="751ce-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="751ce-153">关系</span><span class="sxs-lookup"><span data-stu-id="751ce-153">Relationships</span></span>
|<span data-ttu-id="751ce-154">关系</span><span class="sxs-lookup"><span data-stu-id="751ce-154">Relationship</span></span>|<span data-ttu-id="751ce-155">类型</span><span class="sxs-lookup"><span data-stu-id="751ce-155">Type</span></span>|<span data-ttu-id="751ce-156">说明</span><span class="sxs-lookup"><span data-stu-id="751ce-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751ce-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="751ce-157">managementConditionStatements</span></span>|<span data-ttu-id="751ce-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="751ce-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="751ce-159">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="751ce-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="751ce-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="751ce-160">JSON Representation</span></span>
<span data-ttu-id="751ce-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="751ce-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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





