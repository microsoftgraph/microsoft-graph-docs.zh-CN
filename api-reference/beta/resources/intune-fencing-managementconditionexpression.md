---
title: managementConditionExpression 资源类型
description: 管理条件表达式是一个表达式，它在计算时生成一个布尔值，即 true 或 false，表示管理条件语句已激活/已停用。 管理条件表达式可以由表达式变量和布尔值表达式运算符的组合组成。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5fd8b822d50906cab8ea572d933319aa4c50ff52
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722863"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="3e628-104">managementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e628-104">managementConditionExpression resource type</span></span>

<span data-ttu-id="3e628-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e628-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e628-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e628-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e628-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e628-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e628-108">管理条件表达式是一个表达式，它在计算时生成一个布尔值，即 true 或 false，表示管理条件语句已激活/已停用。</span><span class="sxs-lookup"><span data-stu-id="3e628-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="3e628-109">管理条件表达式可以由表达式变量和布尔值表达式运算符的组合组成。</span><span class="sxs-lookup"><span data-stu-id="3e628-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>

## <a name="properties"></a><span data-ttu-id="3e628-110">属性</span><span class="sxs-lookup"><span data-stu-id="3e628-110">Properties</span></span>
|<span data-ttu-id="3e628-111">属性</span><span class="sxs-lookup"><span data-stu-id="3e628-111">Property</span></span>|<span data-ttu-id="3e628-112">类型</span><span class="sxs-lookup"><span data-stu-id="3e628-112">Type</span></span>|<span data-ttu-id="3e628-113">说明</span><span class="sxs-lookup"><span data-stu-id="3e628-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="3e628-114">关系</span><span class="sxs-lookup"><span data-stu-id="3e628-114">Relationships</span></span>
<span data-ttu-id="3e628-115">无</span><span class="sxs-lookup"><span data-stu-id="3e628-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e628-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e628-116">JSON Representation</span></span>
<span data-ttu-id="3e628-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e628-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpression"
}
```





