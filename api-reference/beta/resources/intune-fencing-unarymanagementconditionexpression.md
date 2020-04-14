---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f0bd5282307d1c8619f756d79209fb04a86bef2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453235"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="29ee4-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="29ee4-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="29ee4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29ee4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29ee4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29ee4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29ee4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29ee4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29ee4-107">使用一元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="29ee4-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="29ee4-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="29ee4-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29ee4-109">属性</span><span class="sxs-lookup"><span data-stu-id="29ee4-109">Properties</span></span>
|<span data-ttu-id="29ee4-110">属性</span><span class="sxs-lookup"><span data-stu-id="29ee4-110">Property</span></span>|<span data-ttu-id="29ee4-111">类型</span><span class="sxs-lookup"><span data-stu-id="29ee4-111">Type</span></span>|<span data-ttu-id="29ee4-112">说明</span><span class="sxs-lookup"><span data-stu-id="29ee4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ee4-113">operator</span><span class="sxs-lookup"><span data-stu-id="29ee4-113">operator</span></span>|[<span data-ttu-id="29ee4-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="29ee4-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="29ee4-115">在一元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="29ee4-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="29ee4-116">可能的值是`not`：。</span><span class="sxs-lookup"><span data-stu-id="29ee4-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="29ee4-117">运算符</span><span class="sxs-lookup"><span data-stu-id="29ee4-117">operand</span></span>|[<span data-ttu-id="29ee4-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="29ee4-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="29ee4-119">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="29ee4-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ee4-120">关系</span><span class="sxs-lookup"><span data-stu-id="29ee4-120">Relationships</span></span>
<span data-ttu-id="29ee4-121">无</span><span class="sxs-lookup"><span data-stu-id="29ee4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29ee4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29ee4-122">JSON Representation</span></span>
<span data-ttu-id="29ee4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29ee4-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```



