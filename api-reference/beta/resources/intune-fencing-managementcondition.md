---
title: managementCondition 资源类型
description: 管理条件是可以动态触发的事件，如地域时限、时限和网络时限。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb7f6ecb00072fb5280cb4033a39fb2041524b7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031380"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="1a68b-103">managementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a68b-103">managementCondition resource type</span></span>

<span data-ttu-id="1a68b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a68b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a68b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a68b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a68b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a68b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a68b-107">管理条件是可以动态触发的事件，如地域时限、时限和网络时限。</span><span class="sxs-lookup"><span data-stu-id="1a68b-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="1a68b-108">方法</span><span class="sxs-lookup"><span data-stu-id="1a68b-108">Methods</span></span>
|<span data-ttu-id="1a68b-109">方法</span><span class="sxs-lookup"><span data-stu-id="1a68b-109">Method</span></span>|<span data-ttu-id="1a68b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a68b-110">Return Type</span></span>|<span data-ttu-id="1a68b-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a68b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a68b-112">列出 managementConditions</span><span class="sxs-lookup"><span data-stu-id="1a68b-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="1a68b-113">[managementCondition](../resources/intune-fencing-managementcondition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a68b-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1a68b-114">列出 [managementCondition](../resources/intune-fencing-managementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a68b-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="1a68b-115">获取 managementCondition</span><span class="sxs-lookup"><span data-stu-id="1a68b-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="1a68b-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="1a68b-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="1a68b-117">读取 [managementCondition](../resources/intune-fencing-managementcondition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a68b-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="1a68b-118">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="1a68b-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="1a68b-119">[managementCondition](../resources/intune-fencing-managementcondition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a68b-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="1a68b-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1a68b-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1a68b-121">属性</span><span class="sxs-lookup"><span data-stu-id="1a68b-121">Properties</span></span>
|<span data-ttu-id="1a68b-122">属性</span><span class="sxs-lookup"><span data-stu-id="1a68b-122">Property</span></span>|<span data-ttu-id="1a68b-123">类型</span><span class="sxs-lookup"><span data-stu-id="1a68b-123">Type</span></span>|<span data-ttu-id="1a68b-124">说明</span><span class="sxs-lookup"><span data-stu-id="1a68b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a68b-125">id</span><span class="sxs-lookup"><span data-stu-id="1a68b-125">id</span></span>|<span data-ttu-id="1a68b-126">String</span><span class="sxs-lookup"><span data-stu-id="1a68b-126">String</span></span>|<span data-ttu-id="1a68b-127">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1a68b-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="1a68b-128">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="1a68b-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1a68b-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="1a68b-129">uniqueName</span></span>|<span data-ttu-id="1a68b-130">String</span><span class="sxs-lookup"><span data-stu-id="1a68b-130">String</span></span>|<span data-ttu-id="1a68b-131">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="1a68b-131">Unique name for the management condition.</span></span> <span data-ttu-id="1a68b-132">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="1a68b-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="1a68b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1a68b-133">displayName</span></span>|<span data-ttu-id="1a68b-134">String</span><span class="sxs-lookup"><span data-stu-id="1a68b-134">String</span></span>|<span data-ttu-id="1a68b-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="1a68b-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="1a68b-136">description</span><span class="sxs-lookup"><span data-stu-id="1a68b-136">description</span></span>|<span data-ttu-id="1a68b-137">String</span><span class="sxs-lookup"><span data-stu-id="1a68b-137">String</span></span>|<span data-ttu-id="1a68b-138">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="1a68b-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="1a68b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a68b-139">createdDateTime</span></span>|<span data-ttu-id="1a68b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a68b-140">DateTimeOffset</span></span>|<span data-ttu-id="1a68b-141">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="1a68b-141">The time the management condition was created.</span></span> <span data-ttu-id="1a68b-142">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="1a68b-142">Generated service side.</span></span>|
|<span data-ttu-id="1a68b-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a68b-143">modifiedDateTime</span></span>|<span data-ttu-id="1a68b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a68b-144">DateTimeOffset</span></span>|<span data-ttu-id="1a68b-145">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="1a68b-145">The time the management condition was last modified.</span></span> <span data-ttu-id="1a68b-146">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="1a68b-146">Updated service side.</span></span>|
|<span data-ttu-id="1a68b-147">eTag</span><span class="sxs-lookup"><span data-stu-id="1a68b-147">eTag</span></span>|<span data-ttu-id="1a68b-148">String</span><span class="sxs-lookup"><span data-stu-id="1a68b-148">String</span></span>|<span data-ttu-id="1a68b-149">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="1a68b-149">ETag of the management condition.</span></span> <span data-ttu-id="1a68b-150">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="1a68b-150">Updated service side.</span></span>|
|<span data-ttu-id="1a68b-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1a68b-151">applicablePlatforms</span></span>|<span data-ttu-id="1a68b-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a68b-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1a68b-153">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="1a68b-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a68b-154">关系</span><span class="sxs-lookup"><span data-stu-id="1a68b-154">Relationships</span></span>
|<span data-ttu-id="1a68b-155">关系</span><span class="sxs-lookup"><span data-stu-id="1a68b-155">Relationship</span></span>|<span data-ttu-id="1a68b-156">类型</span><span class="sxs-lookup"><span data-stu-id="1a68b-156">Type</span></span>|<span data-ttu-id="1a68b-157">说明</span><span class="sxs-lookup"><span data-stu-id="1a68b-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a68b-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="1a68b-158">managementConditionStatements</span></span>|<span data-ttu-id="1a68b-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a68b-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1a68b-160">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="1a68b-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a68b-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a68b-161">JSON Representation</span></span>
<span data-ttu-id="1a68b-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a68b-162">Here is a JSON representation of the resource.</span></span>
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






