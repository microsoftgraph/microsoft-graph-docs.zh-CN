---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 155386e63a5d1f28a3cbe0ed35b9c5f659389bc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011062"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="71908-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="71908-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="71908-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71908-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71908-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71908-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71908-106">使用一元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="71908-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="71908-107">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="71908-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71908-108">属性</span><span class="sxs-lookup"><span data-stu-id="71908-108">Properties</span></span>
|<span data-ttu-id="71908-109">属性</span><span class="sxs-lookup"><span data-stu-id="71908-109">Property</span></span>|<span data-ttu-id="71908-110">类型</span><span class="sxs-lookup"><span data-stu-id="71908-110">Type</span></span>|<span data-ttu-id="71908-111">说明</span><span class="sxs-lookup"><span data-stu-id="71908-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71908-112">operator</span><span class="sxs-lookup"><span data-stu-id="71908-112">operator</span></span>|[<span data-ttu-id="71908-113">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="71908-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="71908-114">在一元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="71908-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="71908-115">可能的值是`not`:。</span><span class="sxs-lookup"><span data-stu-id="71908-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="71908-116">运算符</span><span class="sxs-lookup"><span data-stu-id="71908-116">operand</span></span>|[<span data-ttu-id="71908-117">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="71908-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="71908-118">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="71908-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71908-119">关系</span><span class="sxs-lookup"><span data-stu-id="71908-119">Relationships</span></span>
<span data-ttu-id="71908-120">无</span><span class="sxs-lookup"><span data-stu-id="71908-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71908-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71908-121">JSON Representation</span></span>
<span data-ttu-id="71908-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71908-122">Here is a JSON representation of the resource.</span></span>
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





