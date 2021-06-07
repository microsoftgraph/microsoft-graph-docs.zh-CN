---
title: win32LobAppRegistryRule 资源类型
description: 用于存储 Win32 LOB 应用的注册表规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfa6ed9e95a86abe1d87646a7c57f953be539f69
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758979"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="2731b-103">win32LobAppRegistryRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="2731b-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="2731b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2731b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2731b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2731b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2731b-106">用于存储 Win32 LOB 应用的注册表规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="2731b-106">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="2731b-107">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="2731b-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2731b-108">属性</span><span class="sxs-lookup"><span data-stu-id="2731b-108">Properties</span></span>
|<span data-ttu-id="2731b-109">属性</span><span class="sxs-lookup"><span data-stu-id="2731b-109">Property</span></span>|<span data-ttu-id="2731b-110">类型</span><span class="sxs-lookup"><span data-stu-id="2731b-110">Type</span></span>|<span data-ttu-id="2731b-111">说明</span><span class="sxs-lookup"><span data-stu-id="2731b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2731b-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="2731b-112">ruleType</span></span>|[<span data-ttu-id="2731b-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="2731b-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="2731b-114">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="2731b-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="2731b-115">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="2731b-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="2731b-116">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="2731b-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="2731b-117">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="2731b-117">check32BitOn64System</span></span>|<span data-ttu-id="2731b-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2731b-118">Boolean</span></span>|<span data-ttu-id="2731b-119">一个值，指示是否在 64 位系统上搜索 32 位注册表。</span><span class="sxs-lookup"><span data-stu-id="2731b-119">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="2731b-120">keyPath</span><span class="sxs-lookup"><span data-stu-id="2731b-120">keyPath</span></span>|<span data-ttu-id="2731b-121">String</span><span class="sxs-lookup"><span data-stu-id="2731b-121">String</span></span>|<span data-ttu-id="2731b-122">包含要检测的值的注册表项的完整路径。</span><span class="sxs-lookup"><span data-stu-id="2731b-122">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="2731b-123">valueName</span><span class="sxs-lookup"><span data-stu-id="2731b-123">valueName</span></span>|<span data-ttu-id="2731b-124">String</span><span class="sxs-lookup"><span data-stu-id="2731b-124">String</span></span>|<span data-ttu-id="2731b-125">要检测的注册表值的名称。</span><span class="sxs-lookup"><span data-stu-id="2731b-125">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="2731b-126">operationType</span><span class="sxs-lookup"><span data-stu-id="2731b-126">operationType</span></span>|[<span data-ttu-id="2731b-127">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="2731b-127">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="2731b-128">注册表操作类型。</span><span class="sxs-lookup"><span data-stu-id="2731b-128">The registry operation type.</span></span> <span data-ttu-id="2731b-129">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="2731b-129">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="2731b-130">operator</span><span class="sxs-lookup"><span data-stu-id="2731b-130">operator</span></span>|[<span data-ttu-id="2731b-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="2731b-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="2731b-132">注册表检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="2731b-132">The operator for registry detection.</span></span> <span data-ttu-id="2731b-133">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="2731b-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2731b-134">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="2731b-134">comparisonValue</span></span>|<span data-ttu-id="2731b-135">String</span><span class="sxs-lookup"><span data-stu-id="2731b-135">String</span></span>|<span data-ttu-id="2731b-136">注册表比较值。</span><span class="sxs-lookup"><span data-stu-id="2731b-136">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2731b-137">关系</span><span class="sxs-lookup"><span data-stu-id="2731b-137">Relationships</span></span>
<span data-ttu-id="2731b-138">无</span><span class="sxs-lookup"><span data-stu-id="2731b-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2731b-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2731b-139">JSON Representation</span></span>
<span data-ttu-id="2731b-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2731b-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRule",
  "ruleType": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




