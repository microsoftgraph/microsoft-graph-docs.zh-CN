---
title: managementConditionStatement 资源类型
description: 管理条件语句是一组管理条件, 在满足所有包含的管理条件时启用/禁用设备/应用程序配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37718b5efaa34680f3b990fe61421d0faf24dac5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979170"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="26d55-103">managementConditionStatement 资源类型</span><span class="sxs-lookup"><span data-stu-id="26d55-103">managementConditionStatement resource type</span></span>

> <span data-ttu-id="26d55-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26d55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26d55-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26d55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26d55-106">管理条件语句是一组管理条件, 在满足所有包含的管理条件时启用/禁用设备/应用程序配置。</span><span class="sxs-lookup"><span data-stu-id="26d55-106">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>

## <a name="methods"></a><span data-ttu-id="26d55-107">方法</span><span class="sxs-lookup"><span data-stu-id="26d55-107">Methods</span></span>
|<span data-ttu-id="26d55-108">方法</span><span class="sxs-lookup"><span data-stu-id="26d55-108">Method</span></span>|<span data-ttu-id="26d55-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26d55-109">Return Type</span></span>|<span data-ttu-id="26d55-110">说明</span><span class="sxs-lookup"><span data-stu-id="26d55-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26d55-111">列出 managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="26d55-111">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="26d55-112">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="26d55-112">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="26d55-113">列出[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26d55-113">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="26d55-114">获取 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-114">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="26d55-115">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-115">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="26d55-116">读取[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26d55-116">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="26d55-117">创建 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-117">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="26d55-118">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-118">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="26d55-119">创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26d55-119">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="26d55-120">删除 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-120">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="26d55-121">无</span><span class="sxs-lookup"><span data-stu-id="26d55-121">None</span></span>|<span data-ttu-id="26d55-122">删除[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)。</span><span class="sxs-lookup"><span data-stu-id="26d55-122">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="26d55-123">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-123">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="26d55-124">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="26d55-124">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="26d55-125">更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26d55-125">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="26d55-126">getManagementConditionStatementExpressionString 函数</span><span class="sxs-lookup"><span data-stu-id="26d55-126">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="26d55-127">managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="26d55-127">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="26d55-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26d55-128">Not yet documented</span></span>|
|[<span data-ttu-id="26d55-129">getManagementConditionStatementsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="26d55-129">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="26d55-130">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="26d55-130">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="26d55-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26d55-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="26d55-132">属性</span><span class="sxs-lookup"><span data-stu-id="26d55-132">Properties</span></span>
|<span data-ttu-id="26d55-133">属性</span><span class="sxs-lookup"><span data-stu-id="26d55-133">Property</span></span>|<span data-ttu-id="26d55-134">类型</span><span class="sxs-lookup"><span data-stu-id="26d55-134">Type</span></span>|<span data-ttu-id="26d55-135">说明</span><span class="sxs-lookup"><span data-stu-id="26d55-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d55-136">id</span><span class="sxs-lookup"><span data-stu-id="26d55-136">id</span></span>|<span data-ttu-id="26d55-137">字符串</span><span class="sxs-lookup"><span data-stu-id="26d55-137">String</span></span>|<span data-ttu-id="26d55-138">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="26d55-138">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="26d55-139">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="26d55-139">System generated value assigned when created.</span></span>|
|<span data-ttu-id="26d55-140">displayName</span><span class="sxs-lookup"><span data-stu-id="26d55-140">displayName</span></span>|<span data-ttu-id="26d55-141">String</span><span class="sxs-lookup"><span data-stu-id="26d55-141">String</span></span>|<span data-ttu-id="26d55-142">管理条件语句的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="26d55-142">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="26d55-143">说明</span><span class="sxs-lookup"><span data-stu-id="26d55-143">description</span></span>|<span data-ttu-id="26d55-144">字符串</span><span class="sxs-lookup"><span data-stu-id="26d55-144">String</span></span>|<span data-ttu-id="26d55-145">管理员定义的管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="26d55-145">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="26d55-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26d55-146">createdDateTime</span></span>|<span data-ttu-id="26d55-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26d55-147">DateTimeOffset</span></span>|<span data-ttu-id="26d55-148">管理条件语句的创建时间。</span><span class="sxs-lookup"><span data-stu-id="26d55-148">The time the management condition statement was created.</span></span> <span data-ttu-id="26d55-149">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="26d55-149">Generated service side.</span></span>|
|<span data-ttu-id="26d55-150">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26d55-150">modifiedDateTime</span></span>|<span data-ttu-id="26d55-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26d55-151">DateTimeOffset</span></span>|<span data-ttu-id="26d55-152">上次修改管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="26d55-152">The time the management condition statement was last modified.</span></span> <span data-ttu-id="26d55-153">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="26d55-153">Updated service side.</span></span>|
|<span data-ttu-id="26d55-154">表达式</span><span class="sxs-lookup"><span data-stu-id="26d55-154">expression</span></span>|[<span data-ttu-id="26d55-155">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="26d55-155">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="26d55-156">用于评估管理条件语句是否已激活/停用的管理条件语句表达式。</span><span class="sxs-lookup"><span data-stu-id="26d55-156">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="26d55-157">eTag</span><span class="sxs-lookup"><span data-stu-id="26d55-157">eTag</span></span>|<span data-ttu-id="26d55-158">String</span><span class="sxs-lookup"><span data-stu-id="26d55-158">String</span></span>|<span data-ttu-id="26d55-159">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="26d55-159">ETag of the management condition statement.</span></span> <span data-ttu-id="26d55-160">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="26d55-160">Updated service side.</span></span>|
|<span data-ttu-id="26d55-161">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="26d55-161">applicablePlatforms</span></span>|<span data-ttu-id="26d55-162">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="26d55-162">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="26d55-163">适用于此管理条件语句的平台。</span><span class="sxs-lookup"><span data-stu-id="26d55-163">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="26d55-164">这是通过查看与管理条件语句相关的管理条件和查找适用平台的交集计算得出的。</span><span class="sxs-lookup"><span data-stu-id="26d55-164">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26d55-165">关系</span><span class="sxs-lookup"><span data-stu-id="26d55-165">Relationships</span></span>
|<span data-ttu-id="26d55-166">关系</span><span class="sxs-lookup"><span data-stu-id="26d55-166">Relationship</span></span>|<span data-ttu-id="26d55-167">类型</span><span class="sxs-lookup"><span data-stu-id="26d55-167">Type</span></span>|<span data-ttu-id="26d55-168">说明</span><span class="sxs-lookup"><span data-stu-id="26d55-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d55-169">managementConditions</span><span class="sxs-lookup"><span data-stu-id="26d55-169">managementConditions</span></span>|<span data-ttu-id="26d55-170">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="26d55-170">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="26d55-171">与管理条件语句关联的管理条件。</span><span class="sxs-lookup"><span data-stu-id="26d55-171">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26d55-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26d55-172">JSON Representation</span></span>
<span data-ttu-id="26d55-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26d55-173">Here is a JSON representation of the resource.</span></span>
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





