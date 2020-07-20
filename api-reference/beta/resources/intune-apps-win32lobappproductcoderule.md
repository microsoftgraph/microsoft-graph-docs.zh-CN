---
title: win32LobAppProductCodeRule 资源类型
description: 一个用于存储 Win32 LOB 应用程序的产品代码和版本规则数据的复杂类型。 不支持将此规则作为要求规则。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd3dde2386c76b5ed7dee6174789667d44839c58
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790815"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="6a984-104">win32LobAppProductCodeRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a984-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="6a984-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a984-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a984-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a984-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a984-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a984-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a984-108">一个用于存储 Win32 LOB 应用程序的产品代码和版本规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="6a984-108">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="6a984-109">不支持将此规则作为要求规则。</span><span class="sxs-lookup"><span data-stu-id="6a984-109">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="6a984-110">继承自[win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="6a984-110">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a984-111">属性</span><span class="sxs-lookup"><span data-stu-id="6a984-111">Properties</span></span>
|<span data-ttu-id="6a984-112">属性</span><span class="sxs-lookup"><span data-stu-id="6a984-112">Property</span></span>|<span data-ttu-id="6a984-113">类型</span><span class="sxs-lookup"><span data-stu-id="6a984-113">Type</span></span>|<span data-ttu-id="6a984-114">说明</span><span class="sxs-lookup"><span data-stu-id="6a984-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a984-115">ruleType</span><span class="sxs-lookup"><span data-stu-id="6a984-115">ruleType</span></span>|[<span data-ttu-id="6a984-116">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="6a984-116">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="6a984-117">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="6a984-117">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="6a984-118">继承自[win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="6a984-118">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="6a984-119">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="6a984-119">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="6a984-120">productCode</span><span class="sxs-lookup"><span data-stu-id="6a984-120">productCode</span></span>|<span data-ttu-id="6a984-121">String</span><span class="sxs-lookup"><span data-stu-id="6a984-121">String</span></span>|<span data-ttu-id="6a984-122">应用程序的产品代码。</span><span class="sxs-lookup"><span data-stu-id="6a984-122">The product code of the app.</span></span>|
|<span data-ttu-id="6a984-123">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="6a984-123">productVersionOperator</span></span>|[<span data-ttu-id="6a984-124">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="6a984-124">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="6a984-125">产品版本比较运算符。</span><span class="sxs-lookup"><span data-stu-id="6a984-125">The product version comparison operator.</span></span> <span data-ttu-id="6a984-126">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="6a984-126">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="6a984-127">productVersion</span><span class="sxs-lookup"><span data-stu-id="6a984-127">productVersion</span></span>|<span data-ttu-id="6a984-128">String</span><span class="sxs-lookup"><span data-stu-id="6a984-128">String</span></span>|<span data-ttu-id="6a984-129">产品版本比较值。</span><span class="sxs-lookup"><span data-stu-id="6a984-129">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a984-130">关系</span><span class="sxs-lookup"><span data-stu-id="6a984-130">Relationships</span></span>
<span data-ttu-id="6a984-131">无</span><span class="sxs-lookup"><span data-stu-id="6a984-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a984-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a984-132">JSON Representation</span></span>
<span data-ttu-id="6a984-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a984-133">Here is a JSON representation of the resource.</span></span>
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



