---
title: managementConditionExpressionString 资源类型
description: 管理条件表达式字符串是管理条件表达式的字符串表示形式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4b77be0d5f59dc1cd681104efb0c0404746e574
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528168"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="15a26-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="15a26-103">managementConditionExpressionString resource type</span></span>

<span data-ttu-id="15a26-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="15a26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15a26-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="15a26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15a26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15a26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15a26-107">管理条件表达式字符串是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="15a26-107">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="15a26-108">继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="15a26-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15a26-109">属性</span><span class="sxs-lookup"><span data-stu-id="15a26-109">Properties</span></span>
|<span data-ttu-id="15a26-110">属性</span><span class="sxs-lookup"><span data-stu-id="15a26-110">Property</span></span>|<span data-ttu-id="15a26-111">类型</span><span class="sxs-lookup"><span data-stu-id="15a26-111">Type</span></span>|<span data-ttu-id="15a26-112">说明</span><span class="sxs-lookup"><span data-stu-id="15a26-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15a26-113">值</span><span class="sxs-lookup"><span data-stu-id="15a26-113">value</span></span>|<span data-ttu-id="15a26-114">String</span><span class="sxs-lookup"><span data-stu-id="15a26-114">String</span></span>|<span data-ttu-id="15a26-115">管理条件语句表达式字符串值。</span><span class="sxs-lookup"><span data-stu-id="15a26-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15a26-116">关系</span><span class="sxs-lookup"><span data-stu-id="15a26-116">Relationships</span></span>
<span data-ttu-id="15a26-117">无</span><span class="sxs-lookup"><span data-stu-id="15a26-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15a26-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15a26-118">JSON Representation</span></span>
<span data-ttu-id="15a26-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15a26-119">Here is a JSON representation of the resource.</span></span>
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



