---
title: managementConditionExpressionString 资源类型
description: 管理条件字符串表达式是管理条件表达式的字符串表示形式。
ms.openlocfilehash: 456df27900aa10ead7e2bc090e5e06e0bcd7754f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048447"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="bc3b3-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc3b3-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="bc3b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc3b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc3b3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc3b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc3b3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bc3b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc3b3-107">管理条件字符串表达式是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc3b3-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="bc3b3-108">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="bc3b3-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc3b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc3b3-109">Properties</span></span>
|<span data-ttu-id="bc3b3-110">属性</span><span class="sxs-lookup"><span data-stu-id="bc3b3-110">Property</span></span>|<span data-ttu-id="bc3b3-111">类型</span><span class="sxs-lookup"><span data-stu-id="bc3b3-111">Type</span></span>|<span data-ttu-id="bc3b3-112">说明</span><span class="sxs-lookup"><span data-stu-id="bc3b3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc3b3-113">value</span><span class="sxs-lookup"><span data-stu-id="bc3b3-113">value</span></span>|<span data-ttu-id="bc3b3-114">字符串</span><span class="sxs-lookup"><span data-stu-id="bc3b3-114">String</span></span>|<span data-ttu-id="bc3b3-115">管理条件语句表达式的字符串值。</span><span class="sxs-lookup"><span data-stu-id="bc3b3-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc3b3-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="bc3b3-116">Relationships</span></span>
<span data-ttu-id="bc3b3-117">无</span><span class="sxs-lookup"><span data-stu-id="bc3b3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc3b3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc3b3-118">JSON Representation</span></span>
<span data-ttu-id="bc3b3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc3b3-119">Here is a JSON representation of the resource.</span></span>
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





