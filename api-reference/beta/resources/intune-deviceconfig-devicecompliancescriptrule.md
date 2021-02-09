---
title: deviceComplianceScriptRule 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 169c286043e4c1ec7b9b16e45fa6fb4520781211
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154899"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="1f22a-103">deviceComplianceScriptRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f22a-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="1f22a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f22a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f22a-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f22a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f22a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f22a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f22a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1f22a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1f22a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f22a-108">Properties</span></span>
|<span data-ttu-id="1f22a-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f22a-109">Property</span></span>|<span data-ttu-id="1f22a-110">类型</span><span class="sxs-lookup"><span data-stu-id="1f22a-110">Type</span></span>|<span data-ttu-id="1f22a-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f22a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f22a-112">settingName</span><span class="sxs-lookup"><span data-stu-id="1f22a-112">settingName</span></span>|<span data-ttu-id="1f22a-113">String</span><span class="sxs-lookup"><span data-stu-id="1f22a-113">String</span></span>|<span data-ttu-id="1f22a-114">设置规则中指定的名称。</span><span class="sxs-lookup"><span data-stu-id="1f22a-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="1f22a-115">operator</span><span class="sxs-lookup"><span data-stu-id="1f22a-115">operator</span></span>|[<span data-ttu-id="1f22a-116">operator</span><span class="sxs-lookup"><span data-stu-id="1f22a-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="1f22a-117">规则中指定的运算符。</span><span class="sxs-lookup"><span data-stu-id="1f22a-117">Operator specified in the rule.</span></span> <span data-ttu-id="1f22a-118">可能的值是： `none` ， ， ， ， ， ， `and` ， `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` 。</span><span class="sxs-lookup"><span data-stu-id="1f22a-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="1f22a-119">deviceComplianceScriptRulOperator</span><span class="sxs-lookup"><span data-stu-id="1f22a-119">deviceComplianceScriptRulOperator</span></span>|[<span data-ttu-id="1f22a-120">deviceComplianceScriptRulOperator</span><span class="sxs-lookup"><span data-stu-id="1f22a-120">deviceComplianceScriptRulOperator</span></span>](../resources/intune-deviceconfig-devicecompliancescriptruloperator.md)|<span data-ttu-id="1f22a-121">规则中指定的运算符。</span><span class="sxs-lookup"><span data-stu-id="1f22a-121">Operator specified in the rule.</span></span> <span data-ttu-id="1f22a-122">可能的值是： `none` ， ， ， ， ， ， `and` ， `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` 。</span><span class="sxs-lookup"><span data-stu-id="1f22a-122">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="1f22a-123">DataType</span><span class="sxs-lookup"><span data-stu-id="1f22a-123">dataType</span></span>|[<span data-ttu-id="1f22a-124">dataType</span><span class="sxs-lookup"><span data-stu-id="1f22a-124">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="1f22a-125">规则中指定的数据类型。</span><span class="sxs-lookup"><span data-stu-id="1f22a-125">Data type specified in the rule.</span></span> <span data-ttu-id="1f22a-126">可能的值是： `none` `boolean` ， ， ， ， `int64` ， ， ， ， `double` `string` `dateTime` `version` `base64` `xml` `booleanArray` ， `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` ， 。</span><span class="sxs-lookup"><span data-stu-id="1f22a-126">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="1f22a-127">deviceComplianceScriptRuleDataType</span><span class="sxs-lookup"><span data-stu-id="1f22a-127">deviceComplianceScriptRuleDataType</span></span>|[<span data-ttu-id="1f22a-128">deviceComplianceScriptRuleDataType</span><span class="sxs-lookup"><span data-stu-id="1f22a-128">deviceComplianceScriptRuleDataType</span></span>](../resources/intune-deviceconfig-devicecompliancescriptruledatatype.md)|<span data-ttu-id="1f22a-129">规则中指定的数据类型。</span><span class="sxs-lookup"><span data-stu-id="1f22a-129">Data type specified in the rule.</span></span> <span data-ttu-id="1f22a-130">可能的值是： `none` `boolean` ， ， ， ， `int64` ， ， ， ， `double` `string` `dateTime` `version` `base64` `xml` `booleanArray` ， `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` ， 。</span><span class="sxs-lookup"><span data-stu-id="1f22a-130">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="1f22a-131">操作nd</span><span class="sxs-lookup"><span data-stu-id="1f22a-131">operand</span></span>|<span data-ttu-id="1f22a-132">String</span><span class="sxs-lookup"><span data-stu-id="1f22a-132">String</span></span>|<span data-ttu-id="1f22a-133">规则中指定的操作数。</span><span class="sxs-lookup"><span data-stu-id="1f22a-133">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f22a-134">关系</span><span class="sxs-lookup"><span data-stu-id="1f22a-134">Relationships</span></span>
<span data-ttu-id="1f22a-135">无</span><span class="sxs-lookup"><span data-stu-id="1f22a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f22a-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f22a-136">JSON Representation</span></span>
<span data-ttu-id="1f22a-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f22a-137">Here is a JSON representation of the resource.</span></span>
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
  "deviceComplianceScriptRulOperator": "String",
  "dataType": "String",
  "deviceComplianceScriptRuleDataType": "String",
  "operand": "String"
}
```




