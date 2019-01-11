---
title: unaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用一元操作。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 619d931e53fbd65419e07ab1b2f27341ccb5dd41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829769"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="c1d5a-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1d5a-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="c1d5a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1d5a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1d5a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1d5a-107">管理条件表达式进行求值使用一元操作。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="c1d5a-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="c1d5a-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1d5a-109">属性</span><span class="sxs-lookup"><span data-stu-id="c1d5a-109">Properties</span></span>
|<span data-ttu-id="c1d5a-110">属性</span><span class="sxs-lookup"><span data-stu-id="c1d5a-110">Property</span></span>|<span data-ttu-id="c1d5a-111">类型</span><span class="sxs-lookup"><span data-stu-id="c1d5a-111">Type</span></span>|<span data-ttu-id="c1d5a-112">Description</span><span class="sxs-lookup"><span data-stu-id="c1d5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d5a-113">operator</span><span class="sxs-lookup"><span data-stu-id="c1d5a-113">operator</span></span>|[<span data-ttu-id="c1d5a-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="c1d5a-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="c1d5a-115">在评估一元运算的运算符。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="c1d5a-116">可能的值为： `not`。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="c1d5a-117">操作数</span><span class="sxs-lookup"><span data-stu-id="c1d5a-117">operand</span></span>|[<span data-ttu-id="c1d5a-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="c1d5a-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="c1d5a-119">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1d5a-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="c1d5a-120">Relationships</span></span>
<span data-ttu-id="c1d5a-121">无</span><span class="sxs-lookup"><span data-stu-id="c1d5a-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1d5a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1d5a-122">JSON Representation</span></span>
<span data-ttu-id="c1d5a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1d5a-123">Here is a JSON representation of the resource.</span></span>
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





