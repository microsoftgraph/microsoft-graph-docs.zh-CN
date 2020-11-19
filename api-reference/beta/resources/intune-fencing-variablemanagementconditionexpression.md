---
title: variableManagementConditionExpression 资源类型
description: 将管理条件状态评估为布尔表达式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8be06947bfce0e032965d3704ab9eec3a401845f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298755"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="0fefc-103">variableManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fefc-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="0fefc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fefc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fefc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fefc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fefc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fefc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fefc-107">将管理条件状态评估为布尔表达式。</span><span class="sxs-lookup"><span data-stu-id="0fefc-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="0fefc-108">继承自 [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="0fefc-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0fefc-109">属性</span><span class="sxs-lookup"><span data-stu-id="0fefc-109">Properties</span></span>
|<span data-ttu-id="0fefc-110">属性</span><span class="sxs-lookup"><span data-stu-id="0fefc-110">Property</span></span>|<span data-ttu-id="0fefc-111">类型</span><span class="sxs-lookup"><span data-stu-id="0fefc-111">Type</span></span>|<span data-ttu-id="0fefc-112">Description</span><span class="sxs-lookup"><span data-stu-id="0fefc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fefc-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="0fefc-113">managementConditionId</span></span>|<span data-ttu-id="0fefc-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0fefc-114">String</span></span>|<span data-ttu-id="0fefc-115">用于计算表达式的管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="0fefc-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fefc-116">关系</span><span class="sxs-lookup"><span data-stu-id="0fefc-116">Relationships</span></span>
<span data-ttu-id="0fefc-117">无</span><span class="sxs-lookup"><span data-stu-id="0fefc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fefc-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fefc-118">JSON Representation</span></span>
<span data-ttu-id="0fefc-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fefc-119">Here is a JSON representation of the resource.</span></span>
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




