---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6554f62805bcd1d45f6db165367624434e794117
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783722"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="ea6c7-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea6c7-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="ea6c7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea6c7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea6c7-106">使用一元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="ea6c7-107">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="ea6c7-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea6c7-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea6c7-108">Properties</span></span>
|<span data-ttu-id="ea6c7-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea6c7-109">Property</span></span>|<span data-ttu-id="ea6c7-110">类型</span><span class="sxs-lookup"><span data-stu-id="ea6c7-110">Type</span></span>|<span data-ttu-id="ea6c7-111">说明</span><span class="sxs-lookup"><span data-stu-id="ea6c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea6c7-112">operator</span><span class="sxs-lookup"><span data-stu-id="ea6c7-112">operator</span></span>|[<span data-ttu-id="ea6c7-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="ea6c7-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="ea6c7-114">在一元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="ea6c7-115">可能的值是`not`:。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="ea6c7-116">运算符</span><span class="sxs-lookup"><span data-stu-id="ea6c7-116">operand</span></span>|[<span data-ttu-id="ea6c7-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="ea6c7-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ea6c7-118">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea6c7-119">关系</span><span class="sxs-lookup"><span data-stu-id="ea6c7-119">Relationships</span></span>
<span data-ttu-id="ea6c7-120">无</span><span class="sxs-lookup"><span data-stu-id="ea6c7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea6c7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea6c7-121">JSON Representation</span></span>
<span data-ttu-id="ea6c7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea6c7-122">Here is a JSON representation of the resource.</span></span>
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





