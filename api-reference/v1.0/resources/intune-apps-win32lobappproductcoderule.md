---
title: win32LobAppProductCodeRule 资源类型
description: 用于存储 Win32 LOB 应用的产品代码和版本规则数据的复杂类型。 此规则作为要求规则不受支持。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb77116ce3498023e011d83c6214c3050eaf1124
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742998"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="e8da3-104">win32LobAppProductCodeRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8da3-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="e8da3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8da3-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8da3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8da3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8da3-107">用于存储 Win32 LOB 应用的产品代码和版本规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="e8da3-107">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="e8da3-108">此规则作为要求规则不受支持。</span><span class="sxs-lookup"><span data-stu-id="e8da3-108">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="e8da3-109">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="e8da3-109">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8da3-110">属性</span><span class="sxs-lookup"><span data-stu-id="e8da3-110">Properties</span></span>
|<span data-ttu-id="e8da3-111">属性</span><span class="sxs-lookup"><span data-stu-id="e8da3-111">Property</span></span>|<span data-ttu-id="e8da3-112">类型</span><span class="sxs-lookup"><span data-stu-id="e8da3-112">Type</span></span>|<span data-ttu-id="e8da3-113">Description</span><span class="sxs-lookup"><span data-stu-id="e8da3-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8da3-114">ruleType</span><span class="sxs-lookup"><span data-stu-id="e8da3-114">ruleType</span></span>|[<span data-ttu-id="e8da3-115">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="e8da3-115">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="e8da3-116">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="e8da3-116">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="e8da3-117">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="e8da3-117">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="e8da3-118">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="e8da3-118">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="e8da3-119">productCode</span><span class="sxs-lookup"><span data-stu-id="e8da3-119">productCode</span></span>|<span data-ttu-id="e8da3-120">String</span><span class="sxs-lookup"><span data-stu-id="e8da3-120">String</span></span>|<span data-ttu-id="e8da3-121">应用的产品代码。</span><span class="sxs-lookup"><span data-stu-id="e8da3-121">The product code of the app.</span></span>|
|<span data-ttu-id="e8da3-122">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="e8da3-122">productVersionOperator</span></span>|[<span data-ttu-id="e8da3-123">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="e8da3-123">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="e8da3-124">产品版本比较运算符。</span><span class="sxs-lookup"><span data-stu-id="e8da3-124">The product version comparison operator.</span></span> <span data-ttu-id="e8da3-125">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="e8da3-125">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e8da3-126">productVersion</span><span class="sxs-lookup"><span data-stu-id="e8da3-126">productVersion</span></span>|<span data-ttu-id="e8da3-127">String</span><span class="sxs-lookup"><span data-stu-id="e8da3-127">String</span></span>|<span data-ttu-id="e8da3-128">产品版本比较值。</span><span class="sxs-lookup"><span data-stu-id="e8da3-128">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8da3-129">关系</span><span class="sxs-lookup"><span data-stu-id="e8da3-129">Relationships</span></span>
<span data-ttu-id="e8da3-130">无</span><span class="sxs-lookup"><span data-stu-id="e8da3-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8da3-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8da3-131">JSON Representation</span></span>
<span data-ttu-id="e8da3-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8da3-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeRule",
  "ruleType": "String",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```




