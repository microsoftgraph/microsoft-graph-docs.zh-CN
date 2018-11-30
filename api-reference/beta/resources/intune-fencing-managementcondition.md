---
title: managementCondition 资源类型
description: 管理条件都可以地理范围，如动态触发的事件时限和网络范围。
ms.openlocfilehash: 3c2bc1d7594e61642b96398bfb55d6aa38f3283d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043507"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="08fed-103">managementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="08fed-103">managementCondition resource type</span></span>

> <span data-ttu-id="08fed-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08fed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08fed-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08fed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08fed-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="08fed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08fed-107">管理条件都可以地理范围，如动态触发的事件时限和网络范围。</span><span class="sxs-lookup"><span data-stu-id="08fed-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="08fed-108">方法</span><span class="sxs-lookup"><span data-stu-id="08fed-108">Methods</span></span>
|<span data-ttu-id="08fed-109">方法</span><span class="sxs-lookup"><span data-stu-id="08fed-109">Method</span></span>|<span data-ttu-id="08fed-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="08fed-110">Return Type</span></span>|<span data-ttu-id="08fed-111">说明</span><span class="sxs-lookup"><span data-stu-id="08fed-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08fed-112">列表 managementConditions</span><span class="sxs-lookup"><span data-stu-id="08fed-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="08fed-113">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="08fed-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="08fed-114">列出属性和[managementCondition](../resources/intune-fencing-managementcondition.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="08fed-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="08fed-115">获取 managementCondition</span><span class="sxs-lookup"><span data-stu-id="08fed-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="08fed-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="08fed-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="08fed-117">读取属性和[managementCondition](../resources/intune-fencing-managementcondition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="08fed-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="08fed-118">getManagementConditionsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="08fed-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="08fed-119">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="08fed-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="08fed-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="08fed-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="08fed-121">属性</span><span class="sxs-lookup"><span data-stu-id="08fed-121">Properties</span></span>
|<span data-ttu-id="08fed-122">属性</span><span class="sxs-lookup"><span data-stu-id="08fed-122">Property</span></span>|<span data-ttu-id="08fed-123">类型</span><span class="sxs-lookup"><span data-stu-id="08fed-123">Type</span></span>|<span data-ttu-id="08fed-124">说明</span><span class="sxs-lookup"><span data-stu-id="08fed-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08fed-125">id</span><span class="sxs-lookup"><span data-stu-id="08fed-125">id</span></span>|<span data-ttu-id="08fed-126">字符串</span><span class="sxs-lookup"><span data-stu-id="08fed-126">String</span></span>|<span data-ttu-id="08fed-127">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08fed-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="08fed-128">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="08fed-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="08fed-129">唯一名称</span><span class="sxs-lookup"><span data-stu-id="08fed-129">uniqueName</span></span>|<span data-ttu-id="08fed-130">字符串</span><span class="sxs-lookup"><span data-stu-id="08fed-130">String</span></span>|<span data-ttu-id="08fed-131">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="08fed-131">Unique name for the management condition.</span></span> <span data-ttu-id="08fed-132">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="08fed-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="08fed-133">displayName</span><span class="sxs-lookup"><span data-stu-id="08fed-133">displayName</span></span>|<span data-ttu-id="08fed-134">字符串</span><span class="sxs-lookup"><span data-stu-id="08fed-134">String</span></span>|<span data-ttu-id="08fed-135">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="08fed-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="08fed-136">说明</span><span class="sxs-lookup"><span data-stu-id="08fed-136">description</span></span>|<span data-ttu-id="08fed-137">字符串</span><span class="sxs-lookup"><span data-stu-id="08fed-137">String</span></span>|<span data-ttu-id="08fed-138">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="08fed-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="08fed-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08fed-139">createdDateTime</span></span>|<span data-ttu-id="08fed-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fed-140">DateTimeOffset</span></span>|<span data-ttu-id="08fed-141">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="08fed-141">The time the management condition was created.</span></span> <span data-ttu-id="08fed-142">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="08fed-142">Generated service side.</span></span>|
|<span data-ttu-id="08fed-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08fed-143">modifiedDateTime</span></span>|<span data-ttu-id="08fed-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fed-144">DateTimeOffset</span></span>|<span data-ttu-id="08fed-145">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="08fed-145">The time the management condition was last modified.</span></span> <span data-ttu-id="08fed-146">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="08fed-146">Updated service side.</span></span>|
|<span data-ttu-id="08fed-147">eTag</span><span class="sxs-lookup"><span data-stu-id="08fed-147">eTag</span></span>|<span data-ttu-id="08fed-148">String</span><span class="sxs-lookup"><span data-stu-id="08fed-148">String</span></span>|<span data-ttu-id="08fed-149">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="08fed-149">ETag of the management condition.</span></span> <span data-ttu-id="08fed-150">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="08fed-150">Updated service side.</span></span>|
|<span data-ttu-id="08fed-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="08fed-151">applicablePlatforms</span></span>|<span data-ttu-id="08fed-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="08fed-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="08fed-153">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="08fed-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08fed-154">Relationships</span><span class="sxs-lookup"><span data-stu-id="08fed-154">Relationships</span></span>
|<span data-ttu-id="08fed-155">关系</span><span class="sxs-lookup"><span data-stu-id="08fed-155">Relationship</span></span>|<span data-ttu-id="08fed-156">类型</span><span class="sxs-lookup"><span data-stu-id="08fed-156">Type</span></span>|<span data-ttu-id="08fed-157">说明</span><span class="sxs-lookup"><span data-stu-id="08fed-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08fed-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="08fed-158">managementConditionStatements</span></span>|<span data-ttu-id="08fed-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="08fed-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="08fed-160">为管理 condition 相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="08fed-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08fed-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08fed-161">JSON Representation</span></span>
<span data-ttu-id="08fed-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08fed-162">Here is a JSON representation of the resource.</span></span>
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





