---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4616a7b7bdb54d1bb205d545db4ff7eecbeedbb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783191"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="47f63-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="47f63-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="47f63-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47f63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47f63-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47f63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47f63-106">使用一元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="47f63-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="47f63-107">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="47f63-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47f63-108">属性</span><span class="sxs-lookup"><span data-stu-id="47f63-108">Properties</span></span>
|<span data-ttu-id="47f63-109">属性</span><span class="sxs-lookup"><span data-stu-id="47f63-109">Property</span></span>|<span data-ttu-id="47f63-110">类型</span><span class="sxs-lookup"><span data-stu-id="47f63-110">Type</span></span>|<span data-ttu-id="47f63-111">说明</span><span class="sxs-lookup"><span data-stu-id="47f63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47f63-112">operator</span><span class="sxs-lookup"><span data-stu-id="47f63-112">operator</span></span>|[<span data-ttu-id="47f63-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="47f63-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="47f63-114">在一元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="47f63-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="47f63-115">可能的值是`not`：。</span><span class="sxs-lookup"><span data-stu-id="47f63-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="47f63-116">运算符</span><span class="sxs-lookup"><span data-stu-id="47f63-116">operand</span></span>|[<span data-ttu-id="47f63-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="47f63-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="47f63-118">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="47f63-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47f63-119">关系</span><span class="sxs-lookup"><span data-stu-id="47f63-119">Relationships</span></span>
<span data-ttu-id="47f63-120">无</span><span class="sxs-lookup"><span data-stu-id="47f63-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47f63-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47f63-121">JSON Representation</span></span>
<span data-ttu-id="47f63-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47f63-122">Here is a JSON representation of the resource.</span></span>
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



