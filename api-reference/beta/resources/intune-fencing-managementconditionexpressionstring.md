---
title: managementConditionExpressionString 资源类型
description: 管理条件表达式字符串是管理条件表达式的字符串表示形式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3dac405c71e4e85cc29bb36d335a57bb51fbe0f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783736"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="0ea4c-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ea4c-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="0ea4c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ea4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ea4c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ea4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ea4c-106">管理条件表达式字符串是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ea4c-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="0ea4c-107">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="0ea4c-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ea4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ea4c-108">Properties</span></span>
|<span data-ttu-id="0ea4c-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ea4c-109">Property</span></span>|<span data-ttu-id="0ea4c-110">类型</span><span class="sxs-lookup"><span data-stu-id="0ea4c-110">Type</span></span>|<span data-ttu-id="0ea4c-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ea4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ea4c-112">value</span><span class="sxs-lookup"><span data-stu-id="0ea4c-112">value</span></span>|<span data-ttu-id="0ea4c-113">String</span><span class="sxs-lookup"><span data-stu-id="0ea4c-113">String</span></span>|<span data-ttu-id="0ea4c-114">管理条件语句表达式字符串值。</span><span class="sxs-lookup"><span data-stu-id="0ea4c-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ea4c-115">关系</span><span class="sxs-lookup"><span data-stu-id="0ea4c-115">Relationships</span></span>
<span data-ttu-id="0ea4c-116">无</span><span class="sxs-lookup"><span data-stu-id="0ea4c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ea4c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ea4c-117">JSON Representation</span></span>
<span data-ttu-id="0ea4c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ea4c-118">Here is a JSON representation of the resource.</span></span>
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





