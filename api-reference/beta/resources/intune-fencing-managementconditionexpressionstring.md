---
title: managementConditionExpressionString 资源类型
description: 管理条件字符串表达式是管理条件表达式的字符串表示形式。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b8abc3492690afe6709070decbfe050356fd614
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419189"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="130f3-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="130f3-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="130f3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="130f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="130f3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="130f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="130f3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="130f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="130f3-107">管理条件字符串表达式是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="130f3-107">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="130f3-108">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="130f3-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="130f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="130f3-109">Properties</span></span>
|<span data-ttu-id="130f3-110">属性</span><span class="sxs-lookup"><span data-stu-id="130f3-110">Property</span></span>|<span data-ttu-id="130f3-111">类型</span><span class="sxs-lookup"><span data-stu-id="130f3-111">Type</span></span>|<span data-ttu-id="130f3-112">说明</span><span class="sxs-lookup"><span data-stu-id="130f3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="130f3-113">value</span><span class="sxs-lookup"><span data-stu-id="130f3-113">value</span></span>|<span data-ttu-id="130f3-114">String</span><span class="sxs-lookup"><span data-stu-id="130f3-114">String</span></span>|<span data-ttu-id="130f3-115">管理条件语句表达式的字符串值。</span><span class="sxs-lookup"><span data-stu-id="130f3-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="130f3-116">关系</span><span class="sxs-lookup"><span data-stu-id="130f3-116">Relationships</span></span>
<span data-ttu-id="130f3-117">无</span><span class="sxs-lookup"><span data-stu-id="130f3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="130f3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="130f3-118">JSON Representation</span></span>
<span data-ttu-id="130f3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="130f3-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```




