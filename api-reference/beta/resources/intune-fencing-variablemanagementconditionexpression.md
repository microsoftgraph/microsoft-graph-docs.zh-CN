---
title: variableManagementConditionExpression 资源类型
description: 求值为布尔表达式管理条件状态。
author: tfitzmac
ms.openlocfilehash: 8a6ee46bd42139d519e845c7fe53ab3ae964833f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305920"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="eb4cf-103">variableManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb4cf-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="eb4cf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb4cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb4cf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb4cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb4cf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb4cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb4cf-107">求值为布尔表达式管理条件状态。</span><span class="sxs-lookup"><span data-stu-id="eb4cf-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="eb4cf-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="eb4cf-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb4cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb4cf-109">Properties</span></span>
|<span data-ttu-id="eb4cf-110">属性</span><span class="sxs-lookup"><span data-stu-id="eb4cf-110">Property</span></span>|<span data-ttu-id="eb4cf-111">类型</span><span class="sxs-lookup"><span data-stu-id="eb4cf-111">Type</span></span>|<span data-ttu-id="eb4cf-112">说明</span><span class="sxs-lookup"><span data-stu-id="eb4cf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb4cf-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="eb4cf-113">managementConditionId</span></span>|<span data-ttu-id="eb4cf-114">字符串</span><span class="sxs-lookup"><span data-stu-id="eb4cf-114">String</span></span>|<span data-ttu-id="eb4cf-115">用来计算 expression 管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="eb4cf-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb4cf-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="eb4cf-116">Relationships</span></span>
<span data-ttu-id="eb4cf-117">无</span><span class="sxs-lookup"><span data-stu-id="eb4cf-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb4cf-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb4cf-118">JSON Representation</span></span>
<span data-ttu-id="eb4cf-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb4cf-119">Here is a JSON representation of the resource.</span></span>
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





