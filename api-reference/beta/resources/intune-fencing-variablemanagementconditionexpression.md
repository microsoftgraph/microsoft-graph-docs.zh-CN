---
title: variableManagementConditionExpression 资源类型
description: 求值为布尔表达式管理条件状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5e7efd0c8213f40d1dfb5f86d2f86c999069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399624"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="63424-103">variableManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="63424-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="63424-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="63424-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63424-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63424-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63424-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63424-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63424-107">求值为布尔表达式管理条件状态。</span><span class="sxs-lookup"><span data-stu-id="63424-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="63424-108">继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="63424-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63424-109">属性</span><span class="sxs-lookup"><span data-stu-id="63424-109">Properties</span></span>
|<span data-ttu-id="63424-110">属性</span><span class="sxs-lookup"><span data-stu-id="63424-110">Property</span></span>|<span data-ttu-id="63424-111">类型</span><span class="sxs-lookup"><span data-stu-id="63424-111">Type</span></span>|<span data-ttu-id="63424-112">说明</span><span class="sxs-lookup"><span data-stu-id="63424-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63424-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="63424-113">managementConditionId</span></span>|<span data-ttu-id="63424-114">String</span><span class="sxs-lookup"><span data-stu-id="63424-114">String</span></span>|<span data-ttu-id="63424-115">用来计算 expression 管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="63424-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63424-116">关系</span><span class="sxs-lookup"><span data-stu-id="63424-116">Relationships</span></span>
<span data-ttu-id="63424-117">无</span><span class="sxs-lookup"><span data-stu-id="63424-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63424-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63424-118">JSON Representation</span></span>
<span data-ttu-id="63424-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63424-119">Here is a JSON representation of the resource.</span></span>
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




