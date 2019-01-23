---
title: binaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用二进制操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 722387492e6167c3bd74d306fa03e4835bc12dbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402725"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="7f85e-103">binaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f85e-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="7f85e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7f85e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f85e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7f85e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f85e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f85e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f85e-107">管理条件表达式进行求值使用二进制操作。</span><span class="sxs-lookup"><span data-stu-id="7f85e-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="7f85e-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="7f85e-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f85e-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f85e-109">Properties</span></span>
|<span data-ttu-id="7f85e-110">属性</span><span class="sxs-lookup"><span data-stu-id="7f85e-110">Property</span></span>|<span data-ttu-id="7f85e-111">类型</span><span class="sxs-lookup"><span data-stu-id="7f85e-111">Type</span></span>|<span data-ttu-id="7f85e-112">说明</span><span class="sxs-lookup"><span data-stu-id="7f85e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f85e-113">operator</span><span class="sxs-lookup"><span data-stu-id="7f85e-113">operator</span></span>|[<span data-ttu-id="7f85e-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="7f85e-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="7f85e-115">使用二进制操作的评估版的运算符。</span><span class="sxs-lookup"><span data-stu-id="7f85e-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="7f85e-116">可取值为：`or`、`and`。</span><span class="sxs-lookup"><span data-stu-id="7f85e-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="7f85e-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="7f85e-117">firstOperand</span></span>|[<span data-ttu-id="7f85e-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="7f85e-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7f85e-119">二进制操作的第一个操作数。</span><span class="sxs-lookup"><span data-stu-id="7f85e-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="7f85e-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="7f85e-120">secondOperand</span></span>|[<span data-ttu-id="7f85e-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="7f85e-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7f85e-122">二进制操作第二个操作数。</span><span class="sxs-lookup"><span data-stu-id="7f85e-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f85e-123">关系</span><span class="sxs-lookup"><span data-stu-id="7f85e-123">Relationships</span></span>
<span data-ttu-id="7f85e-124">无</span><span class="sxs-lookup"><span data-stu-id="7f85e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f85e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f85e-125">JSON Representation</span></span>
<span data-ttu-id="7f85e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f85e-126">Here is a JSON representation of the resource.</span></span>
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




