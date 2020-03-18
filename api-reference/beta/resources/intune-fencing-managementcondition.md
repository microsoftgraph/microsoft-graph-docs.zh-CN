---
title: managementCondition 资源类型
description: 管理条件是可以动态触发的事件，如地域时限、时限和网络时限。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d1adf4538cdfc4bfd819c1e9871c3d3a5a5a800
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783247"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="1d766-103">managementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d766-103">managementCondition resource type</span></span>

> <span data-ttu-id="1d766-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d766-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d766-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d766-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d766-106">管理条件是可以动态触发的事件，如地域时限、时限和网络时限。</span><span class="sxs-lookup"><span data-stu-id="1d766-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="1d766-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d766-107">Methods</span></span>
|<span data-ttu-id="1d766-108">方法</span><span class="sxs-lookup"><span data-stu-id="1d766-108">Method</span></span>|<span data-ttu-id="1d766-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d766-109">Return Type</span></span>|<span data-ttu-id="1d766-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d766-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d766-111">列出 managementConditions</span><span class="sxs-lookup"><span data-stu-id="1d766-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="1d766-112">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d766-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1d766-113">列出[managementCondition](../resources/intune-fencing-managementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d766-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="1d766-114">获取 managementCondition</span><span class="sxs-lookup"><span data-stu-id="1d766-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="1d766-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="1d766-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="1d766-116">读取[managementCondition](../resources/intune-fencing-managementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d766-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="1d766-117">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="1d766-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="1d766-118">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d766-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1d766-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1d766-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1d766-120">属性</span><span class="sxs-lookup"><span data-stu-id="1d766-120">Properties</span></span>
|<span data-ttu-id="1d766-121">属性</span><span class="sxs-lookup"><span data-stu-id="1d766-121">Property</span></span>|<span data-ttu-id="1d766-122">类型</span><span class="sxs-lookup"><span data-stu-id="1d766-122">Type</span></span>|<span data-ttu-id="1d766-123">说明</span><span class="sxs-lookup"><span data-stu-id="1d766-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d766-124">id</span><span class="sxs-lookup"><span data-stu-id="1d766-124">id</span></span>|<span data-ttu-id="1d766-125">字符串</span><span class="sxs-lookup"><span data-stu-id="1d766-125">String</span></span>|<span data-ttu-id="1d766-126">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1d766-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="1d766-127">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="1d766-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1d766-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="1d766-128">uniqueName</span></span>|<span data-ttu-id="1d766-129">String</span><span class="sxs-lookup"><span data-stu-id="1d766-129">String</span></span>|<span data-ttu-id="1d766-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="1d766-130">Unique name for the management condition.</span></span> <span data-ttu-id="1d766-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="1d766-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="1d766-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1d766-132">displayName</span></span>|<span data-ttu-id="1d766-133">String</span><span class="sxs-lookup"><span data-stu-id="1d766-133">String</span></span>|<span data-ttu-id="1d766-134">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="1d766-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="1d766-135">说明</span><span class="sxs-lookup"><span data-stu-id="1d766-135">description</span></span>|<span data-ttu-id="1d766-136">字符串</span><span class="sxs-lookup"><span data-stu-id="1d766-136">String</span></span>|<span data-ttu-id="1d766-137">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="1d766-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="1d766-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d766-138">createdDateTime</span></span>|<span data-ttu-id="1d766-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d766-139">DateTimeOffset</span></span>|<span data-ttu-id="1d766-140">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="1d766-140">The time the management condition was created.</span></span> <span data-ttu-id="1d766-141">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="1d766-141">Generated service side.</span></span>|
|<span data-ttu-id="1d766-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d766-142">modifiedDateTime</span></span>|<span data-ttu-id="1d766-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d766-143">DateTimeOffset</span></span>|<span data-ttu-id="1d766-144">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="1d766-144">The time the management condition was last modified.</span></span> <span data-ttu-id="1d766-145">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="1d766-145">Updated service side.</span></span>|
|<span data-ttu-id="1d766-146">eTag</span><span class="sxs-lookup"><span data-stu-id="1d766-146">eTag</span></span>|<span data-ttu-id="1d766-147">String</span><span class="sxs-lookup"><span data-stu-id="1d766-147">String</span></span>|<span data-ttu-id="1d766-148">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="1d766-148">ETag of the management condition.</span></span> <span data-ttu-id="1d766-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="1d766-149">Updated service side.</span></span>|
|<span data-ttu-id="1d766-150">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1d766-150">applicablePlatforms</span></span>|<span data-ttu-id="1d766-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d766-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1d766-152">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="1d766-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d766-153">关系</span><span class="sxs-lookup"><span data-stu-id="1d766-153">Relationships</span></span>
|<span data-ttu-id="1d766-154">关系</span><span class="sxs-lookup"><span data-stu-id="1d766-154">Relationship</span></span>|<span data-ttu-id="1d766-155">类型</span><span class="sxs-lookup"><span data-stu-id="1d766-155">Type</span></span>|<span data-ttu-id="1d766-156">说明</span><span class="sxs-lookup"><span data-stu-id="1d766-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d766-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="1d766-157">managementConditionStatements</span></span>|<span data-ttu-id="1d766-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d766-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1d766-159">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="1d766-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d766-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d766-160">JSON Representation</span></span>
<span data-ttu-id="1d766-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d766-161">Here is a JSON representation of the resource.</span></span>
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



