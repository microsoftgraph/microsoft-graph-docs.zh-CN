---
title: managementConditionExpression 资源类型
description: 管理条件表达式是一个将生成一个布尔值在计算时，即一个 true 或 false，指示管理条件语句激活/停用的表达式。 管理条件表达式可能组成表达式变量和布尔值表达式运算符的组合。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e572cdae0104cf5bbb929286b4c3452dfd38eeea
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415507"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="ca9bf-104">managementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca9bf-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="ca9bf-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ca9bf-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca9bf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca9bf-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca9bf-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca9bf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9bf-108">管理条件表达式是一个将生成一个布尔值在计算时，即一个 true 或 false，指示管理条件语句激活/停用的表达式。</span><span class="sxs-lookup"><span data-stu-id="ca9bf-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="ca9bf-109">管理条件表达式可能组成表达式变量和布尔值表达式运算符的组合。</span><span class="sxs-lookup"><span data-stu-id="ca9bf-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>

## <a name="properties"></a><span data-ttu-id="ca9bf-110">属性</span><span class="sxs-lookup"><span data-stu-id="ca9bf-110">Properties</span></span>
|<span data-ttu-id="ca9bf-111">属性</span><span class="sxs-lookup"><span data-stu-id="ca9bf-111">Property</span></span>|<span data-ttu-id="ca9bf-112">类型</span><span class="sxs-lookup"><span data-stu-id="ca9bf-112">Type</span></span>|<span data-ttu-id="ca9bf-113">说明</span><span class="sxs-lookup"><span data-stu-id="ca9bf-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="ca9bf-114">关系</span><span class="sxs-lookup"><span data-stu-id="ca9bf-114">Relationships</span></span>
<span data-ttu-id="ca9bf-115">无</span><span class="sxs-lookup"><span data-stu-id="ca9bf-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca9bf-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca9bf-116">JSON Representation</span></span>
<span data-ttu-id="ca9bf-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca9bf-117">Here is a JSON representation of the resource.</span></span>
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




