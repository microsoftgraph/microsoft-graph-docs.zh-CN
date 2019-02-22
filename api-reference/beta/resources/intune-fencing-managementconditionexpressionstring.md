---
title: managementConditionExpressionString 资源类型
description: 管理条件表达式字符串是管理条件表达式的字符串表示形式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4552ab6cc97676ced32ae7e7f5649262c4f4f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151007"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="1cc5e-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cc5e-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="1cc5e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1cc5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cc5e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cc5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cc5e-106">管理条件表达式字符串是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cc5e-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="1cc5e-107">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="1cc5e-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1cc5e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cc5e-108">Properties</span></span>
|<span data-ttu-id="1cc5e-109">属性</span><span class="sxs-lookup"><span data-stu-id="1cc5e-109">Property</span></span>|<span data-ttu-id="1cc5e-110">类型</span><span class="sxs-lookup"><span data-stu-id="1cc5e-110">Type</span></span>|<span data-ttu-id="1cc5e-111">说明</span><span class="sxs-lookup"><span data-stu-id="1cc5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cc5e-112">value</span><span class="sxs-lookup"><span data-stu-id="1cc5e-112">value</span></span>|<span data-ttu-id="1cc5e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1cc5e-113">String</span></span>|<span data-ttu-id="1cc5e-114">管理条件语句表达式字符串值。</span><span class="sxs-lookup"><span data-stu-id="1cc5e-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cc5e-115">关系</span><span class="sxs-lookup"><span data-stu-id="1cc5e-115">Relationships</span></span>
<span data-ttu-id="1cc5e-116">无</span><span class="sxs-lookup"><span data-stu-id="1cc5e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cc5e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cc5e-117">JSON Representation</span></span>
<span data-ttu-id="1cc5e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cc5e-118">Here is a JSON representation of the resource.</span></span>
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




