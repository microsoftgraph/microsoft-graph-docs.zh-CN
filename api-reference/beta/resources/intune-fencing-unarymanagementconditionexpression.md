---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 403867dcbdcc0767043fbe873c6de6b415eb32f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524502"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="d7564-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7564-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="d7564-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7564-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7564-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7564-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7564-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7564-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7564-107">使用一元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="d7564-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="d7564-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="d7564-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7564-109">属性</span><span class="sxs-lookup"><span data-stu-id="d7564-109">Properties</span></span>
|<span data-ttu-id="d7564-110">属性</span><span class="sxs-lookup"><span data-stu-id="d7564-110">Property</span></span>|<span data-ttu-id="d7564-111">类型</span><span class="sxs-lookup"><span data-stu-id="d7564-111">Type</span></span>|<span data-ttu-id="d7564-112">说明</span><span class="sxs-lookup"><span data-stu-id="d7564-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7564-113">operator</span><span class="sxs-lookup"><span data-stu-id="d7564-113">operator</span></span>|[<span data-ttu-id="d7564-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="d7564-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="d7564-115">在一元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="d7564-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="d7564-116">可能的值是`not`：。</span><span class="sxs-lookup"><span data-stu-id="d7564-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="d7564-117">运算符</span><span class="sxs-lookup"><span data-stu-id="d7564-117">operand</span></span>|[<span data-ttu-id="d7564-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="d7564-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="d7564-119">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="d7564-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7564-120">关系</span><span class="sxs-lookup"><span data-stu-id="d7564-120">Relationships</span></span>
<span data-ttu-id="d7564-121">无</span><span class="sxs-lookup"><span data-stu-id="d7564-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7564-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7564-122">JSON Representation</span></span>
<span data-ttu-id="d7564-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7564-123">Here is a JSON representation of the resource.</span></span>
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



