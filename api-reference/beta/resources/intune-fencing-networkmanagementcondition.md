---
title: networkManagementCondition 资源类型
description: 包含用于定义网络管理条件的信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bced41a40200cd79d58fe71a36cf1af5b1a65cc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528148"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="ff8ed-103">networkManagementCondition 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff8ed-103">networkManagementCondition resource type</span></span>

<span data-ttu-id="ff8ed-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff8ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff8ed-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff8ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff8ed-107">包含用于定义网络管理条件的信息。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="ff8ed-108">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ff8ed-109">方法</span><span class="sxs-lookup"><span data-stu-id="ff8ed-109">Methods</span></span>
|<span data-ttu-id="ff8ed-110">方法</span><span class="sxs-lookup"><span data-stu-id="ff8ed-110">Method</span></span>|<span data-ttu-id="ff8ed-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff8ed-111">Return Type</span></span>|<span data-ttu-id="ff8ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="ff8ed-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff8ed-113">列出 networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="ff8ed-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="ff8ed-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff8ed-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="ff8ed-115">列出[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="ff8ed-116">获取 networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ff8ed-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="ff8ed-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ff8ed-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="ff8ed-118">读取[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff8ed-119">属性</span><span class="sxs-lookup"><span data-stu-id="ff8ed-119">Properties</span></span>
|<span data-ttu-id="ff8ed-120">属性</span><span class="sxs-lookup"><span data-stu-id="ff8ed-120">Property</span></span>|<span data-ttu-id="ff8ed-121">类型</span><span class="sxs-lookup"><span data-stu-id="ff8ed-121">Type</span></span>|<span data-ttu-id="ff8ed-122">说明</span><span class="sxs-lookup"><span data-stu-id="ff8ed-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff8ed-123">id</span><span class="sxs-lookup"><span data-stu-id="ff8ed-123">id</span></span>|<span data-ttu-id="ff8ed-124">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8ed-124">String</span></span>|<span data-ttu-id="ff8ed-125">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="ff8ed-126">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-126">System generated value assigned when created.</span></span> <span data-ttu-id="ff8ed-127">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="ff8ed-128">uniqueName</span></span>|<span data-ttu-id="ff8ed-129">String</span><span class="sxs-lookup"><span data-stu-id="ff8ed-129">String</span></span>|<span data-ttu-id="ff8ed-130">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-130">Unique name for the management condition.</span></span> <span data-ttu-id="ff8ed-131">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-131">Used in management condition expressions.</span></span> <span data-ttu-id="ff8ed-132">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ff8ed-133">displayName</span></span>|<span data-ttu-id="ff8ed-134">String</span><span class="sxs-lookup"><span data-stu-id="ff8ed-134">String</span></span>|<span data-ttu-id="ff8ed-135">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="ff8ed-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-137">说明</span><span class="sxs-lookup"><span data-stu-id="ff8ed-137">description</span></span>|<span data-ttu-id="ff8ed-138">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8ed-138">String</span></span>|<span data-ttu-id="ff8ed-139">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="ff8ed-140">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff8ed-141">createdDateTime</span></span>|<span data-ttu-id="ff8ed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff8ed-142">DateTimeOffset</span></span>|<span data-ttu-id="ff8ed-143">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-143">The time the management condition was created.</span></span> <span data-ttu-id="ff8ed-144">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-144">Generated service side.</span></span> <span data-ttu-id="ff8ed-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff8ed-146">modifiedDateTime</span></span>|<span data-ttu-id="ff8ed-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff8ed-147">DateTimeOffset</span></span>|<span data-ttu-id="ff8ed-148">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-148">The time the management condition was last modified.</span></span> <span data-ttu-id="ff8ed-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-149">Updated service side.</span></span> <span data-ttu-id="ff8ed-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-151">eTag</span><span class="sxs-lookup"><span data-stu-id="ff8ed-151">eTag</span></span>|<span data-ttu-id="ff8ed-152">String</span><span class="sxs-lookup"><span data-stu-id="ff8ed-152">String</span></span>|<span data-ttu-id="ff8ed-153">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-153">ETag of the management condition.</span></span> <span data-ttu-id="ff8ed-154">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-154">Updated service side.</span></span> <span data-ttu-id="ff8ed-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ff8ed-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="ff8ed-156">applicablePlatforms</span></span>|<span data-ttu-id="ff8ed-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff8ed-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ff8ed-158">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="ff8ed-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff8ed-160">关系</span><span class="sxs-lookup"><span data-stu-id="ff8ed-160">Relationships</span></span>
|<span data-ttu-id="ff8ed-161">关系</span><span class="sxs-lookup"><span data-stu-id="ff8ed-161">Relationship</span></span>|<span data-ttu-id="ff8ed-162">类型</span><span class="sxs-lookup"><span data-stu-id="ff8ed-162">Type</span></span>|<span data-ttu-id="ff8ed-163">说明</span><span class="sxs-lookup"><span data-stu-id="ff8ed-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff8ed-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="ff8ed-164">managementConditionStatements</span></span>|<span data-ttu-id="ff8ed-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff8ed-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="ff8ed-166">与管理条件相关联的管理条件语句。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="ff8ed-167">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8ed-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff8ed-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff8ed-168">JSON Representation</span></span>
<span data-ttu-id="ff8ed-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff8ed-169">Here is a JSON representation of the resource.</span></span>
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



