---
title: binaryManagementConditionExpression 资源类型
description: 使用二元运算计算的管理条件表达式。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff87c376bd88e49d8dc2c3d4657607e7bddcb503
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783275"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="7f17f-103">binaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f17f-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="7f17f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f17f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f17f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f17f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f17f-106">使用二元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="7f17f-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="7f17f-107">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="7f17f-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f17f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f17f-108">Properties</span></span>
|<span data-ttu-id="7f17f-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f17f-109">Property</span></span>|<span data-ttu-id="7f17f-110">类型</span><span class="sxs-lookup"><span data-stu-id="7f17f-110">Type</span></span>|<span data-ttu-id="7f17f-111">说明</span><span class="sxs-lookup"><span data-stu-id="7f17f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f17f-112">operator</span><span class="sxs-lookup"><span data-stu-id="7f17f-112">operator</span></span>|[<span data-ttu-id="7f17f-113">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="7f17f-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="7f17f-114">在二元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="7f17f-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="7f17f-115">可取值为：`or`、`and`。</span><span class="sxs-lookup"><span data-stu-id="7f17f-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="7f17f-116">firstOperand</span><span class="sxs-lookup"><span data-stu-id="7f17f-116">firstOperand</span></span>|[<span data-ttu-id="7f17f-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="7f17f-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7f17f-118">二元运算的第一个操作数。</span><span class="sxs-lookup"><span data-stu-id="7f17f-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="7f17f-119">secondOperand</span><span class="sxs-lookup"><span data-stu-id="7f17f-119">secondOperand</span></span>|[<span data-ttu-id="7f17f-120">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="7f17f-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7f17f-121">二元运算的第二个操作数。</span><span class="sxs-lookup"><span data-stu-id="7f17f-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f17f-122">关系</span><span class="sxs-lookup"><span data-stu-id="7f17f-122">Relationships</span></span>
<span data-ttu-id="7f17f-123">无</span><span class="sxs-lookup"><span data-stu-id="7f17f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f17f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f17f-124">JSON Representation</span></span>
<span data-ttu-id="7f17f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f17f-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```



