---
title: managementConditionStatement 资源类型
description: 管理条件语句是一组的管理条件的启用/禁用设备/应用程序配置满足所有包含的管理条件时。
ms.openlocfilehash: 98b76ce96550d894f8b32f6f6174d5c565e322ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045842"
---
# <a name="managementconditionstatement-resource-type"></a><span data-ttu-id="a8e2b-103">managementConditionStatement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8e2b-103">managementConditionStatement resource type</span></span>

> <span data-ttu-id="a8e2b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8e2b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8e2b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e2b-107">管理条件语句是一组的管理条件的启用/禁用设备/应用程序配置满足所有包含的管理条件时。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-107">A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.</span></span>
## <a name="methods"></a><span data-ttu-id="a8e2b-108">方法</span><span class="sxs-lookup"><span data-stu-id="a8e2b-108">Methods</span></span>
|<span data-ttu-id="a8e2b-109">方法</span><span class="sxs-lookup"><span data-stu-id="a8e2b-109">Method</span></span>|<span data-ttu-id="a8e2b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8e2b-110">Return Type</span></span>|<span data-ttu-id="a8e2b-111">说明</span><span class="sxs-lookup"><span data-stu-id="a8e2b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8e2b-112">列表 managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="a8e2b-112">List managementConditionStatements</span></span>](../api/intune-fencing-managementconditionstatement-list.md)|<span data-ttu-id="a8e2b-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8e2b-113">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="a8e2b-114">列出属性和[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-114">List properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) objects.</span></span>|
|[<span data-ttu-id="a8e2b-115">获取 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-115">Get managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-get.md)|[<span data-ttu-id="a8e2b-116">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-116">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="a8e2b-117">读取属性和[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-117">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="a8e2b-118">创建 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-118">Create managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-create.md)|[<span data-ttu-id="a8e2b-119">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-119">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="a8e2b-120">创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-120">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="a8e2b-121">删除 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-121">Delete managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-delete.md)|<span data-ttu-id="a8e2b-122">无</span><span class="sxs-lookup"><span data-stu-id="a8e2b-122">None</span></span>|<span data-ttu-id="a8e2b-123">删除[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-123">Deletes a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>|
|[<span data-ttu-id="a8e2b-124">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-124">Update managementConditionStatement</span></span>](../api/intune-fencing-managementconditionstatement-update.md)|[<span data-ttu-id="a8e2b-125">managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a8e2b-125">managementConditionStatement</span></span>](../resources/intune-fencing-managementconditionstatement.md)|<span data-ttu-id="a8e2b-126">更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-126">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>|
|[<span data-ttu-id="a8e2b-127">getManagementConditionStatementExpressionString 函数</span><span class="sxs-lookup"><span data-stu-id="a8e2b-127">getManagementConditionStatementExpressionString function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[<span data-ttu-id="a8e2b-128">managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="a8e2b-128">managementConditionExpressionString</span></span>](../resources/intune-fencing-managementconditionexpressionstring.md)|<span data-ttu-id="a8e2b-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a8e2b-129">Not yet documented</span></span>|
|[<span data-ttu-id="a8e2b-130">getManagementConditionStatementsForPlatform 函数</span><span class="sxs-lookup"><span data-stu-id="a8e2b-130">getManagementConditionStatementsForPlatform function</span></span>](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|<span data-ttu-id="a8e2b-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8e2b-131">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="a8e2b-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a8e2b-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a8e2b-133">属性</span><span class="sxs-lookup"><span data-stu-id="a8e2b-133">Properties</span></span>
|<span data-ttu-id="a8e2b-134">属性</span><span class="sxs-lookup"><span data-stu-id="a8e2b-134">Property</span></span>|<span data-ttu-id="a8e2b-135">类型</span><span class="sxs-lookup"><span data-stu-id="a8e2b-135">Type</span></span>|<span data-ttu-id="a8e2b-136">说明</span><span class="sxs-lookup"><span data-stu-id="a8e2b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e2b-137">id</span><span class="sxs-lookup"><span data-stu-id="a8e2b-137">id</span></span>|<span data-ttu-id="a8e2b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a8e2b-138">String</span></span>|<span data-ttu-id="a8e2b-139">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-139">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="a8e2b-140">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-140">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a8e2b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a8e2b-141">displayName</span></span>|<span data-ttu-id="a8e2b-142">字符串</span><span class="sxs-lookup"><span data-stu-id="a8e2b-142">String</span></span>|<span data-ttu-id="a8e2b-143">管理员定义管理条件语句的名称。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-143">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="a8e2b-144">说明</span><span class="sxs-lookup"><span data-stu-id="a8e2b-144">description</span></span>|<span data-ttu-id="a8e2b-145">字符串</span><span class="sxs-lookup"><span data-stu-id="a8e2b-145">String</span></span>|<span data-ttu-id="a8e2b-146">管理员定义管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-146">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="a8e2b-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e2b-147">createdDateTime</span></span>|<span data-ttu-id="a8e2b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e2b-148">DateTimeOffset</span></span>|<span data-ttu-id="a8e2b-149">创建管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-149">The time the management condition statement was created.</span></span> <span data-ttu-id="a8e2b-150">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-150">Generated service side.</span></span>|
|<span data-ttu-id="a8e2b-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e2b-151">modifiedDateTime</span></span>|<span data-ttu-id="a8e2b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e2b-152">DateTimeOffset</span></span>|<span data-ttu-id="a8e2b-153">管理条件语句上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-153">The time the management condition statement was last modified.</span></span> <span data-ttu-id="a8e2b-154">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-154">Updated service side.</span></span>|
|<span data-ttu-id="a8e2b-155">表达式</span><span class="sxs-lookup"><span data-stu-id="a8e2b-155">expression</span></span>|[<span data-ttu-id="a8e2b-156">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="a8e2b-156">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="a8e2b-157">用来评估如果管理条件语句的管理条件语句表达式已激活/停用。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-157">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="a8e2b-158">eTag</span><span class="sxs-lookup"><span data-stu-id="a8e2b-158">eTag</span></span>|<span data-ttu-id="a8e2b-159">String</span><span class="sxs-lookup"><span data-stu-id="a8e2b-159">String</span></span>|<span data-ttu-id="a8e2b-160">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-160">ETag of the management condition statement.</span></span> <span data-ttu-id="a8e2b-161">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-161">Updated service side.</span></span>|
|<span data-ttu-id="a8e2b-162">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a8e2b-162">applicablePlatforms</span></span>|<span data-ttu-id="a8e2b-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8e2b-163">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a8e2b-164">此管理条件语句适用的平台。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-164">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="a8e2b-165">这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-165">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e2b-166">Relationships</span><span class="sxs-lookup"><span data-stu-id="a8e2b-166">Relationships</span></span>
|<span data-ttu-id="a8e2b-167">关系</span><span class="sxs-lookup"><span data-stu-id="a8e2b-167">Relationship</span></span>|<span data-ttu-id="a8e2b-168">类型</span><span class="sxs-lookup"><span data-stu-id="a8e2b-168">Type</span></span>|<span data-ttu-id="a8e2b-169">说明</span><span class="sxs-lookup"><span data-stu-id="a8e2b-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e2b-170">managementConditions</span><span class="sxs-lookup"><span data-stu-id="a8e2b-170">managementConditions</span></span>|<span data-ttu-id="a8e2b-171">[managementCondition](../resources/intune-fencing-managementcondition.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8e2b-171">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="a8e2b-172">管理条件语句对相关的管理条件。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-172">The management conditions associated to the management condition statement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8e2b-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8e2b-173">JSON Representation</span></span>
<span data-ttu-id="a8e2b-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8e2b-174">Here is a JSON representation of the resource.</span></span>
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





