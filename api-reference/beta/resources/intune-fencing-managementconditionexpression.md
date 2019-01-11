---
title: managementConditionExpression 资源类型
description: 管理条件表达式是一个将生成一个布尔值在计算时，即一个 true 或 false，指示管理条件语句激活/停用的表达式。 管理条件表达式可能组成表达式变量和布尔值表达式运算符的组合。
localization_priority: Normal
ms.openlocfilehash: f7f370b348ab13ef964eab1cc7025868e4380bac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857062"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="5c96a-104">managementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c96a-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="5c96a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5c96a-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c96a-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c96a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c96a-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c96a-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c96a-108">管理条件表达式是一个将生成一个布尔值在计算时，即一个 true 或 false，指示管理条件语句激活/停用的表达式。</span><span class="sxs-lookup"><span data-stu-id="5c96a-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="5c96a-109">管理条件表达式可能组成表达式变量和布尔值表达式运算符的组合。</span><span class="sxs-lookup"><span data-stu-id="5c96a-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>
## <a name="properties"></a><span data-ttu-id="5c96a-110">属性</span><span class="sxs-lookup"><span data-stu-id="5c96a-110">Properties</span></span>
|<span data-ttu-id="5c96a-111">属性</span><span class="sxs-lookup"><span data-stu-id="5c96a-111">Property</span></span>|<span data-ttu-id="5c96a-112">类型</span><span class="sxs-lookup"><span data-stu-id="5c96a-112">Type</span></span>|<span data-ttu-id="5c96a-113">说明</span><span class="sxs-lookup"><span data-stu-id="5c96a-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="5c96a-114">关系</span><span class="sxs-lookup"><span data-stu-id="5c96a-114">Relationships</span></span>
<span data-ttu-id="5c96a-115">无</span><span class="sxs-lookup"><span data-stu-id="5c96a-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c96a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c96a-116">JSON Representation</span></span>
<span data-ttu-id="5c96a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c96a-117">Here is a JSON representation of the resource.</span></span>
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





