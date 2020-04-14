---
title: binaryManagementConditionExpression 资源类型
description: 使用二元运算计算的管理条件表达式。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 575f5d14b3c7427976814405729f12ed48d8a3fa
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442743"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="26ae8-103">binaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="26ae8-103">binaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="26ae8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ae8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26ae8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26ae8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26ae8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26ae8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ae8-107">使用二元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="26ae8-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="26ae8-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="26ae8-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26ae8-109">属性</span><span class="sxs-lookup"><span data-stu-id="26ae8-109">Properties</span></span>
|<span data-ttu-id="26ae8-110">属性</span><span class="sxs-lookup"><span data-stu-id="26ae8-110">Property</span></span>|<span data-ttu-id="26ae8-111">类型</span><span class="sxs-lookup"><span data-stu-id="26ae8-111">Type</span></span>|<span data-ttu-id="26ae8-112">说明</span><span class="sxs-lookup"><span data-stu-id="26ae8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ae8-113">operator</span><span class="sxs-lookup"><span data-stu-id="26ae8-113">operator</span></span>|[<span data-ttu-id="26ae8-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="26ae8-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="26ae8-115">在二元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="26ae8-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="26ae8-116">可取值为：`or`、`and`。</span><span class="sxs-lookup"><span data-stu-id="26ae8-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="26ae8-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="26ae8-117">firstOperand</span></span>|[<span data-ttu-id="26ae8-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="26ae8-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="26ae8-119">二元运算的第一个操作数。</span><span class="sxs-lookup"><span data-stu-id="26ae8-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="26ae8-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="26ae8-120">secondOperand</span></span>|[<span data-ttu-id="26ae8-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="26ae8-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="26ae8-122">二元运算的第二个操作数。</span><span class="sxs-lookup"><span data-stu-id="26ae8-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26ae8-123">关系</span><span class="sxs-lookup"><span data-stu-id="26ae8-123">Relationships</span></span>
<span data-ttu-id="26ae8-124">无</span><span class="sxs-lookup"><span data-stu-id="26ae8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26ae8-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26ae8-125">JSON Representation</span></span>
<span data-ttu-id="26ae8-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26ae8-126">Here is a JSON representation of the resource.</span></span>
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



