---
title: managementConditionExpressionString 资源类型
description: 管理条件表达式字符串是管理条件表达式的字符串表示形式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4c9e96e6774787777c2d3ed8587b103af5eb1ca
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331642"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="c3f80-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3f80-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="c3f80-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3f80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3f80-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3f80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3f80-106">管理条件表达式字符串是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3f80-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="c3f80-107">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="c3f80-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3f80-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3f80-108">Properties</span></span>
|<span data-ttu-id="c3f80-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3f80-109">Property</span></span>|<span data-ttu-id="c3f80-110">类型</span><span class="sxs-lookup"><span data-stu-id="c3f80-110">Type</span></span>|<span data-ttu-id="c3f80-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3f80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3f80-112">值</span><span class="sxs-lookup"><span data-stu-id="c3f80-112">value</span></span>|<span data-ttu-id="c3f80-113">String</span><span class="sxs-lookup"><span data-stu-id="c3f80-113">String</span></span>|<span data-ttu-id="c3f80-114">管理条件语句表达式字符串值。</span><span class="sxs-lookup"><span data-stu-id="c3f80-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3f80-115">关系</span><span class="sxs-lookup"><span data-stu-id="c3f80-115">Relationships</span></span>
<span data-ttu-id="c3f80-116">无</span><span class="sxs-lookup"><span data-stu-id="c3f80-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3f80-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3f80-117">JSON Representation</span></span>
<span data-ttu-id="c3f80-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3f80-118">Here is a JSON representation of the resource.</span></span>
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



