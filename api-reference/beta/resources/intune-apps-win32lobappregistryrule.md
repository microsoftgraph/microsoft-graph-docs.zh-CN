---
title: win32LobAppRegistryRule 资源类型
description: 用于存储 Win32 LOB 应用程序的注册表规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e4fcce49fde2f1eb8eb33bc320f1204369b09cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790808"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="7b3d8-103">win32LobAppRegistryRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b3d8-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="7b3d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b3d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b3d8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b3d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3d8-107">用于存储 Win32 LOB 应用程序的注册表规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-107">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="7b3d8-108">继承自[win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="7b3d8-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7b3d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="7b3d8-109">Properties</span></span>
|<span data-ttu-id="7b3d8-110">属性</span><span class="sxs-lookup"><span data-stu-id="7b3d8-110">Property</span></span>|<span data-ttu-id="7b3d8-111">类型</span><span class="sxs-lookup"><span data-stu-id="7b3d8-111">Type</span></span>|<span data-ttu-id="7b3d8-112">说明</span><span class="sxs-lookup"><span data-stu-id="7b3d8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b3d8-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="7b3d8-113">ruleType</span></span>|[<span data-ttu-id="7b3d8-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="7b3d8-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="7b3d8-115">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="7b3d8-116">继承自[win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="7b3d8-117">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="7b3d8-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="7b3d8-118">check32BitOn64System</span></span>|<span data-ttu-id="7b3d8-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="7b3d8-119">Boolean</span></span>|<span data-ttu-id="7b3d8-120">一个值，指示是否在64位系统上搜索32位注册表。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-120">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="7b3d8-121">keyPath</span><span class="sxs-lookup"><span data-stu-id="7b3d8-121">keyPath</span></span>|<span data-ttu-id="7b3d8-122">String</span><span class="sxs-lookup"><span data-stu-id="7b3d8-122">String</span></span>|<span data-ttu-id="7b3d8-123">包含要检测的值的注册表项的完整路径。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-123">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="7b3d8-124">等值</span><span class="sxs-lookup"><span data-stu-id="7b3d8-124">valueName</span></span>|<span data-ttu-id="7b3d8-125">String</span><span class="sxs-lookup"><span data-stu-id="7b3d8-125">String</span></span>|<span data-ttu-id="7b3d8-126">要检测的注册表值的名称。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-126">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="7b3d8-127">operationType</span><span class="sxs-lookup"><span data-stu-id="7b3d8-127">operationType</span></span>|[<span data-ttu-id="7b3d8-128">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="7b3d8-128">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="7b3d8-129">注册表操作类型。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-129">The registry operation type.</span></span> <span data-ttu-id="7b3d8-130">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-130">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="7b3d8-131">operator</span><span class="sxs-lookup"><span data-stu-id="7b3d8-131">operator</span></span>|[<span data-ttu-id="7b3d8-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="7b3d8-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="7b3d8-133">用于注册表检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-133">The operator for registry detection.</span></span> <span data-ttu-id="7b3d8-134">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="7b3d8-135">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="7b3d8-135">comparisonValue</span></span>|<span data-ttu-id="7b3d8-136">String</span><span class="sxs-lookup"><span data-stu-id="7b3d8-136">String</span></span>|<span data-ttu-id="7b3d8-137">注册表比较值。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-137">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b3d8-138">关系</span><span class="sxs-lookup"><span data-stu-id="7b3d8-138">Relationships</span></span>
<span data-ttu-id="7b3d8-139">无</span><span class="sxs-lookup"><span data-stu-id="7b3d8-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b3d8-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b3d8-140">JSON Representation</span></span>
<span data-ttu-id="7b3d8-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b3d8-141">Here is a JSON representation of the resource.</span></span>
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



