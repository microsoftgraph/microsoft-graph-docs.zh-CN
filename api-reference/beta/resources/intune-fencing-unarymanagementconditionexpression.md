---
title: unaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用一元操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 06a379a53d6d85956a54bede444714e082196ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949421"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="032b9-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="032b9-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="032b9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="032b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="032b9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="032b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="032b9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="032b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="032b9-107">管理条件表达式进行求值使用一元操作。</span><span class="sxs-lookup"><span data-stu-id="032b9-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="032b9-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="032b9-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="032b9-109">属性</span><span class="sxs-lookup"><span data-stu-id="032b9-109">Properties</span></span>
|<span data-ttu-id="032b9-110">属性</span><span class="sxs-lookup"><span data-stu-id="032b9-110">Property</span></span>|<span data-ttu-id="032b9-111">类型</span><span class="sxs-lookup"><span data-stu-id="032b9-111">Type</span></span>|<span data-ttu-id="032b9-112">说明</span><span class="sxs-lookup"><span data-stu-id="032b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="032b9-113">operator</span><span class="sxs-lookup"><span data-stu-id="032b9-113">operator</span></span>|[<span data-ttu-id="032b9-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="032b9-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="032b9-115">在评估一元运算的运算符。</span><span class="sxs-lookup"><span data-stu-id="032b9-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="032b9-116">可能的值为： `not`。</span><span class="sxs-lookup"><span data-stu-id="032b9-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="032b9-117">操作数</span><span class="sxs-lookup"><span data-stu-id="032b9-117">operand</span></span>|[<span data-ttu-id="032b9-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="032b9-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="032b9-119">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="032b9-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="032b9-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="032b9-120">Relationships</span></span>
<span data-ttu-id="032b9-121">无</span><span class="sxs-lookup"><span data-stu-id="032b9-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="032b9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="032b9-122">JSON Representation</span></span>
<span data-ttu-id="032b9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="032b9-123">Here is a JSON representation of the resource.</span></span>
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





