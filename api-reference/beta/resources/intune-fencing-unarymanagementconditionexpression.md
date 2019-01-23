---
title: unaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用一元操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1224a869ec2ec9cae2f38273f7a68b64d3d7333
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406778"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="472d5-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="472d5-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="472d5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="472d5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="472d5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="472d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="472d5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="472d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="472d5-107">管理条件表达式进行求值使用一元操作。</span><span class="sxs-lookup"><span data-stu-id="472d5-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="472d5-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="472d5-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="472d5-109">属性</span><span class="sxs-lookup"><span data-stu-id="472d5-109">Properties</span></span>
|<span data-ttu-id="472d5-110">属性</span><span class="sxs-lookup"><span data-stu-id="472d5-110">Property</span></span>|<span data-ttu-id="472d5-111">类型</span><span class="sxs-lookup"><span data-stu-id="472d5-111">Type</span></span>|<span data-ttu-id="472d5-112">说明</span><span class="sxs-lookup"><span data-stu-id="472d5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472d5-113">operator</span><span class="sxs-lookup"><span data-stu-id="472d5-113">operator</span></span>|[<span data-ttu-id="472d5-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="472d5-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="472d5-115">在评估一元运算的运算符。</span><span class="sxs-lookup"><span data-stu-id="472d5-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="472d5-116">可能的值为： `not`。</span><span class="sxs-lookup"><span data-stu-id="472d5-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="472d5-117">操作数</span><span class="sxs-lookup"><span data-stu-id="472d5-117">operand</span></span>|[<span data-ttu-id="472d5-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="472d5-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="472d5-119">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="472d5-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="472d5-120">关系</span><span class="sxs-lookup"><span data-stu-id="472d5-120">Relationships</span></span>
<span data-ttu-id="472d5-121">无</span><span class="sxs-lookup"><span data-stu-id="472d5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="472d5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="472d5-122">JSON Representation</span></span>
<span data-ttu-id="472d5-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="472d5-123">Here is a JSON representation of the resource.</span></span>
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




