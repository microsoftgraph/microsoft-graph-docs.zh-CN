---
title: managementConditionStatement 资源类型
description: 管理条件语句是一组管理条件，在满足所有包含的管理条件时启用/禁用设备/应用程序配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd52a4c78873a55c6b7635538cac11c2c5168542
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439708"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="89096-103">managementConditionStatement 资源类型</span><span class="sxs-lookup"><span data-stu-id="89096-103">managementConditionStatement resource type</span></span>

<span data-ttu-id="89096-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89096-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89096-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89096-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89096-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89096-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89096-107">管理条件语句是一组管理条件，在满足所有包含的管理条件时启用/禁用设备/应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="89096-107">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="89096-108">方法</span><span class="sxs-lookup"><span data-stu-id="89096-108">Methods</span></span>
|<span data-ttu-id="89096-109">方法</span><span class="sxs-lookup"><span data-stu-id="89096-109">Method</span></span>|<span data-ttu-id="89096-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="89096-110">Return Type</span></span>|<span data-ttu-id="89096-111">说明</span><span class="sxs-lookup"><span data-stu-id="89096-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89096-112">列出 managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="89096-112">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="89096-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="89096-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="89096-114">列出[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89096-114">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="89096-115">获取 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-115">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="89096-116">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-116">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="89096-117">读取[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89096-117">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="89096-118">创建 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-118">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="89096-119">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-119">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="89096-120">创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="89096-120">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="89096-121">删除 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-121">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="89096-122">无</span><span class="sxs-lookup"><span data-stu-id="89096-122">None</span></span>|<span data-ttu-id="89096-123">删除[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)。</span><span class="sxs-lookup"><span data-stu-id="89096-123">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="89096-124">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-124">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="89096-125">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="89096-125">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="89096-126">更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89096-126">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="89096-127">getManagementConditionStatementExpressionString 函数</span><span class="sxs-lookup"><span data-stu-id="89096-127">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="89096-128">managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="89096-128">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="89096-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89096-129">Not yet documented</span></span>|
|[<span data-ttu-id="89096-130">getManagementConditionStatementsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="89096-130">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="89096-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="89096-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="89096-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89096-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="89096-133">属性</span><span class="sxs-lookup"><span data-stu-id="89096-133">Properties</span></span>
|<span data-ttu-id="89096-134">属性</span><span class="sxs-lookup"><span data-stu-id="89096-134">Property</span></span>|<span data-ttu-id="89096-135">类型</span><span class="sxs-lookup"><span data-stu-id="89096-135">Type</span></span>|<span data-ttu-id="89096-136">说明</span><span class="sxs-lookup"><span data-stu-id="89096-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89096-137">id</span><span class="sxs-lookup"><span data-stu-id="89096-137">id</span></span>|<span data-ttu-id="89096-138">字符串</span><span class="sxs-lookup"><span data-stu-id="89096-138">String</span></span>|<span data-ttu-id="89096-139">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="89096-139">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="89096-140">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="89096-140">System generated value assigned when created.</span></span>|
|<span data-ttu-id="89096-141">displayName</span><span class="sxs-lookup"><span data-stu-id="89096-141">displayName</span></span>|<span data-ttu-id="89096-142">String</span><span class="sxs-lookup"><span data-stu-id="89096-142">String</span></span>|<span data-ttu-id="89096-143">管理条件语句的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="89096-143">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="89096-144">description</span><span class="sxs-lookup"><span data-stu-id="89096-144">description</span></span>|<span data-ttu-id="89096-145">字符串</span><span class="sxs-lookup"><span data-stu-id="89096-145">String</span></span>|<span data-ttu-id="89096-146">管理员定义的管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="89096-146">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="89096-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89096-147">createdDateTime</span></span>|<span data-ttu-id="89096-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89096-148">DateTimeOffset</span></span>|<span data-ttu-id="89096-149">管理条件语句的创建时间。</span><span class="sxs-lookup"><span data-stu-id="89096-149">The time the management condition statement was created.</span></span> <span data-ttu-id="89096-150">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="89096-150">Generated service side.</span></span>|
|<span data-ttu-id="89096-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89096-151">modifiedDateTime</span></span>|<span data-ttu-id="89096-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89096-152">DateTimeOffset</span></span>|<span data-ttu-id="89096-153">上次修改管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="89096-153">The time the management condition statement was last modified.</span></span> <span data-ttu-id="89096-154">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="89096-154">Updated service side.</span></span>|
|<span data-ttu-id="89096-155">表达式</span><span class="sxs-lookup"><span data-stu-id="89096-155">expression</span></span>|[<span data-ttu-id="89096-156">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="89096-156">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="89096-157">用于评估管理条件语句是否已激活/停用的管理条件语句表达式。</span><span class="sxs-lookup"><span data-stu-id="89096-157">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="89096-158">eTag</span><span class="sxs-lookup"><span data-stu-id="89096-158">eTag</span></span>|<span data-ttu-id="89096-159">String</span><span class="sxs-lookup"><span data-stu-id="89096-159">String</span></span>|<span data-ttu-id="89096-160">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="89096-160">ETag of the management condition statement.</span></span> <span data-ttu-id="89096-161">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="89096-161">Updated service side.</span></span>|
|<span data-ttu-id="89096-162">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="89096-162">applicablePlatforms</span></span>|<span data-ttu-id="89096-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="89096-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="89096-164">适用于此管理条件语句的平台。</span><span class="sxs-lookup"><span data-stu-id="89096-164">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="89096-165">这是通过查看与管理条件语句相关的管理条件和查找适用平台的交集计算得出的。</span><span class="sxs-lookup"><span data-stu-id="89096-165">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89096-166">关系</span><span class="sxs-lookup"><span data-stu-id="89096-166">Relationships</span></span>
|<span data-ttu-id="89096-167">关系</span><span class="sxs-lookup"><span data-stu-id="89096-167">Relationship</span></span>|<span data-ttu-id="89096-168">类型</span><span class="sxs-lookup"><span data-stu-id="89096-168">Type</span></span>|<span data-ttu-id="89096-169">说明</span><span class="sxs-lookup"><span data-stu-id="89096-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89096-170">managementConditions</span><span class="sxs-lookup"><span data-stu-id="89096-170">managementConditions</span></span>|<span data-ttu-id="89096-171">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="89096-171">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="89096-172">与管理条件语句关联的管理条件。</span><span class="sxs-lookup"><span data-stu-id="89096-172">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89096-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89096-173">JSON Representation</span></span>
<span data-ttu-id="89096-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89096-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



