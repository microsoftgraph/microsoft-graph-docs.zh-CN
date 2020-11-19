---
title: managementConditionExpressionString 资源类型
description: 管理条件表达式字符串是管理条件表达式的字符串表示形式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc8dacdb6d8443fd5525f75fc035e3fbcd3504b4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288287"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="58889-103">managementConditionExpressionString 资源类型</span><span class="sxs-lookup"><span data-stu-id="58889-103">managementConditionExpressionString resource type</span></span>

<span data-ttu-id="58889-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58889-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58889-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58889-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58889-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58889-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58889-107">管理条件表达式字符串是管理条件表达式的字符串表示形式。</span><span class="sxs-lookup"><span data-stu-id="58889-107">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="58889-108">继承自 [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="58889-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58889-109">属性</span><span class="sxs-lookup"><span data-stu-id="58889-109">Properties</span></span>
|<span data-ttu-id="58889-110">属性</span><span class="sxs-lookup"><span data-stu-id="58889-110">Property</span></span>|<span data-ttu-id="58889-111">类型</span><span class="sxs-lookup"><span data-stu-id="58889-111">Type</span></span>|<span data-ttu-id="58889-112">说明</span><span class="sxs-lookup"><span data-stu-id="58889-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58889-113">值</span><span class="sxs-lookup"><span data-stu-id="58889-113">value</span></span>|<span data-ttu-id="58889-114">String</span><span class="sxs-lookup"><span data-stu-id="58889-114">String</span></span>|<span data-ttu-id="58889-115">管理条件语句表达式字符串值。</span><span class="sxs-lookup"><span data-stu-id="58889-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58889-116">关系</span><span class="sxs-lookup"><span data-stu-id="58889-116">Relationships</span></span>
<span data-ttu-id="58889-117">无</span><span class="sxs-lookup"><span data-stu-id="58889-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58889-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58889-118">JSON Representation</span></span>
<span data-ttu-id="58889-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58889-119">Here is a JSON representation of the resource.</span></span>
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




