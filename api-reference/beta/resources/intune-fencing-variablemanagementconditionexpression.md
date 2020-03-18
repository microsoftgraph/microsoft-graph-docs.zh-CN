---
title: variableManagementConditionExpression 资源类型
description: 将管理条件状态评估为布尔表达式。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 363f19e2f8b6860ba0228cd6a29a07dd82bd8277
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783177"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="fc3ee-103">variableManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc3ee-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="fc3ee-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc3ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc3ee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc3ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc3ee-106">将管理条件状态评估为布尔表达式。</span><span class="sxs-lookup"><span data-stu-id="fc3ee-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="fc3ee-107">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="fc3ee-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc3ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc3ee-108">Properties</span></span>
|<span data-ttu-id="fc3ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="fc3ee-109">Property</span></span>|<span data-ttu-id="fc3ee-110">类型</span><span class="sxs-lookup"><span data-stu-id="fc3ee-110">Type</span></span>|<span data-ttu-id="fc3ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="fc3ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc3ee-112">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="fc3ee-112">managementConditionId</span></span>|<span data-ttu-id="fc3ee-113">String</span><span class="sxs-lookup"><span data-stu-id="fc3ee-113">String</span></span>|<span data-ttu-id="fc3ee-114">用于计算表达式的管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="fc3ee-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc3ee-115">关系</span><span class="sxs-lookup"><span data-stu-id="fc3ee-115">Relationships</span></span>
<span data-ttu-id="fc3ee-116">无</span><span class="sxs-lookup"><span data-stu-id="fc3ee-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc3ee-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc3ee-117">JSON Representation</span></span>
<span data-ttu-id="fc3ee-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc3ee-118">Here is a JSON representation of the resource.</span></span>
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



