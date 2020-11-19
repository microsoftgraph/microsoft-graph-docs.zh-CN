---
title: deviceComplianceScriptRule 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29264e89f3c935d473161edb2c4fbad3bb88849b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260261"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="92a01-103">deviceComplianceScriptRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="92a01-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="92a01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92a01-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92a01-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a01-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="92a01-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="92a01-108">属性</span><span class="sxs-lookup"><span data-stu-id="92a01-108">Properties</span></span>
|<span data-ttu-id="92a01-109">属性</span><span class="sxs-lookup"><span data-stu-id="92a01-109">Property</span></span>|<span data-ttu-id="92a01-110">类型</span><span class="sxs-lookup"><span data-stu-id="92a01-110">Type</span></span>|<span data-ttu-id="92a01-111">描述</span><span class="sxs-lookup"><span data-stu-id="92a01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a01-112">settingName</span><span class="sxs-lookup"><span data-stu-id="92a01-112">settingName</span></span>|<span data-ttu-id="92a01-113">String</span><span class="sxs-lookup"><span data-stu-id="92a01-113">String</span></span>|<span data-ttu-id="92a01-114">规则中指定的设置名称。</span><span class="sxs-lookup"><span data-stu-id="92a01-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="92a01-115">operator</span><span class="sxs-lookup"><span data-stu-id="92a01-115">operator</span></span>|[<span data-ttu-id="92a01-116">operator</span><span class="sxs-lookup"><span data-stu-id="92a01-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="92a01-117">在规则中指定的运算符。</span><span class="sxs-lookup"><span data-stu-id="92a01-117">Operator specified in the rule.</span></span> <span data-ttu-id="92a01-118">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、、 `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` 。</span><span class="sxs-lookup"><span data-stu-id="92a01-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="92a01-119">DataType</span><span class="sxs-lookup"><span data-stu-id="92a01-119">dataType</span></span>|[<span data-ttu-id="92a01-120">dataType</span><span class="sxs-lookup"><span data-stu-id="92a01-120">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="92a01-121">规则中指定的数据类型。</span><span class="sxs-lookup"><span data-stu-id="92a01-121">Data type specified in the rule.</span></span> <span data-ttu-id="92a01-122">可能的值为：、、、、、、、、、、、、、、 `none` `boolean` `int64` `double` `string` `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` 。</span><span class="sxs-lookup"><span data-stu-id="92a01-122">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="92a01-123">运算符</span><span class="sxs-lookup"><span data-stu-id="92a01-123">operand</span></span>|<span data-ttu-id="92a01-124">String</span><span class="sxs-lookup"><span data-stu-id="92a01-124">String</span></span>|<span data-ttu-id="92a01-125">规则中指定的操作数。</span><span class="sxs-lookup"><span data-stu-id="92a01-125">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92a01-126">关系</span><span class="sxs-lookup"><span data-stu-id="92a01-126">Relationships</span></span>
<span data-ttu-id="92a01-127">无</span><span class="sxs-lookup"><span data-stu-id="92a01-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92a01-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92a01-128">JSON Representation</span></span>
<span data-ttu-id="92a01-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92a01-129">Here is a JSON representation of the resource.</span></span>
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




