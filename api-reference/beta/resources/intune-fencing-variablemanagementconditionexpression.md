---
title: variableManagementConditionExpression 资源类型
description: 求值为布尔表达式管理条件状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8fc3e49e7ba55cf10a1dac36690d0b1e419890a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939761"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="6e436-103">variableManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e436-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="6e436-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6e436-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e436-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e436-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e436-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6e436-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e436-107">求值为布尔表达式管理条件状态。</span><span class="sxs-lookup"><span data-stu-id="6e436-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="6e436-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="6e436-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e436-109">属性</span><span class="sxs-lookup"><span data-stu-id="6e436-109">Properties</span></span>
|<span data-ttu-id="6e436-110">属性</span><span class="sxs-lookup"><span data-stu-id="6e436-110">Property</span></span>|<span data-ttu-id="6e436-111">类型</span><span class="sxs-lookup"><span data-stu-id="6e436-111">Type</span></span>|<span data-ttu-id="6e436-112">说明</span><span class="sxs-lookup"><span data-stu-id="6e436-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e436-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="6e436-113">managementConditionId</span></span>|<span data-ttu-id="6e436-114">字符串</span><span class="sxs-lookup"><span data-stu-id="6e436-114">String</span></span>|<span data-ttu-id="6e436-115">用来计算 expression 管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="6e436-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e436-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="6e436-116">Relationships</span></span>
<span data-ttu-id="6e436-117">无</span><span class="sxs-lookup"><span data-stu-id="6e436-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6e436-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e436-118">JSON Representation</span></span>
<span data-ttu-id="6e436-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e436-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```





