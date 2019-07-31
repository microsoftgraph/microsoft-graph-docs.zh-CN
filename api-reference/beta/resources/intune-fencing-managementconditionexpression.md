---
title: managementConditionExpression 资源类型
description: 管理条件表达式是一个表达式, 它在计算时生成一个布尔值, 即 true 或 false, 表示管理条件语句已激活/已停用。 管理条件表达式可以由表达式变量和布尔值表达式运算符的组合组成。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2758d4223eedafa082901d890ef45103c0e8082a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011104"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="099f7-104">managementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="099f7-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="099f7-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="099f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="099f7-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="099f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="099f7-107">管理条件表达式是一个表达式, 它在计算时生成一个布尔值, 即 true 或 false, 表示管理条件语句已激活/已停用。</span><span class="sxs-lookup"><span data-stu-id="099f7-107">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="099f7-108">管理条件表达式可以由表达式变量和布尔值表达式运算符的组合组成。</span><span class="sxs-lookup"><span data-stu-id="099f7-108">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>

## <a name="properties"></a><span data-ttu-id="099f7-109">属性</span><span class="sxs-lookup"><span data-stu-id="099f7-109">Properties</span></span>
|<span data-ttu-id="099f7-110">属性</span><span class="sxs-lookup"><span data-stu-id="099f7-110">Property</span></span>|<span data-ttu-id="099f7-111">类型</span><span class="sxs-lookup"><span data-stu-id="099f7-111">Type</span></span>|<span data-ttu-id="099f7-112">说明</span><span class="sxs-lookup"><span data-stu-id="099f7-112">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="099f7-113">关系</span><span class="sxs-lookup"><span data-stu-id="099f7-113">Relationships</span></span>
<span data-ttu-id="099f7-114">无</span><span class="sxs-lookup"><span data-stu-id="099f7-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="099f7-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="099f7-115">JSON Representation</span></span>
<span data-ttu-id="099f7-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="099f7-116">Here is a JSON representation of the resource.</span></span>
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





