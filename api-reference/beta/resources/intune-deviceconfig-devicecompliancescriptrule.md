---
title: deviceComplianceScriptRule 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c524202b8e15d077895c47c1c66256d58ca2c3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789325"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="66046-103">deviceComplianceScriptRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="66046-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="66046-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66046-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66046-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66046-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66046-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66046-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66046-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="66046-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="66046-108">属性</span><span class="sxs-lookup"><span data-stu-id="66046-108">Properties</span></span>
|<span data-ttu-id="66046-109">属性</span><span class="sxs-lookup"><span data-stu-id="66046-109">Property</span></span>|<span data-ttu-id="66046-110">类型</span><span class="sxs-lookup"><span data-stu-id="66046-110">Type</span></span>|<span data-ttu-id="66046-111">说明</span><span class="sxs-lookup"><span data-stu-id="66046-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66046-112">settingName</span><span class="sxs-lookup"><span data-stu-id="66046-112">settingName</span></span>|<span data-ttu-id="66046-113">String</span><span class="sxs-lookup"><span data-stu-id="66046-113">String</span></span>|<span data-ttu-id="66046-114">规则中指定的设置名称。</span><span class="sxs-lookup"><span data-stu-id="66046-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="66046-115">operator</span><span class="sxs-lookup"><span data-stu-id="66046-115">operator</span></span>|[<span data-ttu-id="66046-116">接线员</span><span class="sxs-lookup"><span data-stu-id="66046-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="66046-117">在规则中指定的运算符。</span><span class="sxs-lookup"><span data-stu-id="66046-117">Operator specified in the rule.</span></span> <span data-ttu-id="66046-118">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、、 `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` 。</span><span class="sxs-lookup"><span data-stu-id="66046-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="66046-119">DataType</span><span class="sxs-lookup"><span data-stu-id="66046-119">dataType</span></span>|[<span data-ttu-id="66046-120">Udt</span><span class="sxs-lookup"><span data-stu-id="66046-120">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="66046-121">规则中指定的数据类型。</span><span class="sxs-lookup"><span data-stu-id="66046-121">Data type specified in the rule.</span></span> <span data-ttu-id="66046-122">可能的值为：、、、、、、、、、、、、、、 `none` `boolean` `int64` `double` `string` `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` 。</span><span class="sxs-lookup"><span data-stu-id="66046-122">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="66046-123">运算符</span><span class="sxs-lookup"><span data-stu-id="66046-123">operand</span></span>|<span data-ttu-id="66046-124">String</span><span class="sxs-lookup"><span data-stu-id="66046-124">String</span></span>|<span data-ttu-id="66046-125">规则中指定的操作数。</span><span class="sxs-lookup"><span data-stu-id="66046-125">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66046-126">关系</span><span class="sxs-lookup"><span data-stu-id="66046-126">Relationships</span></span>
<span data-ttu-id="66046-127">无</span><span class="sxs-lookup"><span data-stu-id="66046-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66046-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66046-128">JSON Representation</span></span>
<span data-ttu-id="66046-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66046-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "dataType": "String",
  "operand": "String"
}
```



