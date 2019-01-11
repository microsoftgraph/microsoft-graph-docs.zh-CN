---
title: managementConditionExpressionString 资源类型
description: 管理条件字符串表达式是管理条件表达式的字符串表示形式。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 815d799bc37328062a717097fd27bc0870a315f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811576"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="23a3f-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="23a3f-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="23a3f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="23a3f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23a3f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23a3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23a3f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="23a3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23a3f-107">管理条件字符串表达式是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="23a3f-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="23a3f-108">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="23a3f-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23a3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="23a3f-109">Properties</span></span>
|<span data-ttu-id="23a3f-110">属性</span><span class="sxs-lookup"><span data-stu-id="23a3f-110">Property</span></span>|<span data-ttu-id="23a3f-111">类型</span><span class="sxs-lookup"><span data-stu-id="23a3f-111">Type</span></span>|<span data-ttu-id="23a3f-112">说明</span><span class="sxs-lookup"><span data-stu-id="23a3f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a3f-113">value</span><span class="sxs-lookup"><span data-stu-id="23a3f-113">value</span></span>|<span data-ttu-id="23a3f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="23a3f-114">String</span></span>|<span data-ttu-id="23a3f-115">管理条件语句表达式的字符串值。</span><span class="sxs-lookup"><span data-stu-id="23a3f-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23a3f-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="23a3f-116">Relationships</span></span>
<span data-ttu-id="23a3f-117">无</span><span class="sxs-lookup"><span data-stu-id="23a3f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23a3f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23a3f-118">JSON Representation</span></span>
<span data-ttu-id="23a3f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23a3f-119">Here is a JSON representation of the resource.</span></span>
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





