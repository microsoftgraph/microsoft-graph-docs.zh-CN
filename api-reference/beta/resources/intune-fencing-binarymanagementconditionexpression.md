---
title: binaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用二进制操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b15938d0bb29fdfdad8abb1b37b02ad1e6468cf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978534"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="ebaee-103">binaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebaee-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="ebaee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ebaee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebaee-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ebaee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebaee-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ebaee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebaee-107">管理条件表达式进行求值使用二进制操作。</span><span class="sxs-lookup"><span data-stu-id="ebaee-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="ebaee-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="ebaee-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebaee-109">属性</span><span class="sxs-lookup"><span data-stu-id="ebaee-109">Properties</span></span>
|<span data-ttu-id="ebaee-110">属性</span><span class="sxs-lookup"><span data-stu-id="ebaee-110">Property</span></span>|<span data-ttu-id="ebaee-111">类型</span><span class="sxs-lookup"><span data-stu-id="ebaee-111">Type</span></span>|<span data-ttu-id="ebaee-112">说明</span><span class="sxs-lookup"><span data-stu-id="ebaee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebaee-113">operator</span><span class="sxs-lookup"><span data-stu-id="ebaee-113">operator</span></span>|[<span data-ttu-id="ebaee-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="ebaee-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="ebaee-115">使用二进制操作的评估版的运算符。</span><span class="sxs-lookup"><span data-stu-id="ebaee-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="ebaee-116">可取值为：`or`、`and`。</span><span class="sxs-lookup"><span data-stu-id="ebaee-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="ebaee-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="ebaee-117">firstOperand</span></span>|[<span data-ttu-id="ebaee-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="ebaee-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ebaee-119">二进制操作的第一个操作数。</span><span class="sxs-lookup"><span data-stu-id="ebaee-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="ebaee-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="ebaee-120">secondOperand</span></span>|[<span data-ttu-id="ebaee-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="ebaee-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ebaee-122">二进制操作第二个操作数。</span><span class="sxs-lookup"><span data-stu-id="ebaee-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebaee-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="ebaee-123">Relationships</span></span>
<span data-ttu-id="ebaee-124">无</span><span class="sxs-lookup"><span data-stu-id="ebaee-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebaee-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebaee-125">JSON Representation</span></span>
<span data-ttu-id="ebaee-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebaee-126">Here is a JSON representation of the resource.</span></span>
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





