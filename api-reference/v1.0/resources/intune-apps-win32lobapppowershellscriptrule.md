---
title: win32LobAppPowerShellScriptRule 资源类型
description: 用于存储 Win32 LOB 应用程序的 PowerShell 脚本规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25ca86e44b6244e592214459c4ebcfbd0f228231
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020250"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="a0d57-103">win32LobAppPowerShellScriptRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0d57-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="a0d57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0d57-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0d57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0d57-106">用于存储 Win32 LOB 应用程序的 PowerShell 脚本规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="a0d57-106">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="a0d57-107">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="a0d57-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0d57-108">属性</span><span class="sxs-lookup"><span data-stu-id="a0d57-108">Properties</span></span>
|<span data-ttu-id="a0d57-109">属性</span><span class="sxs-lookup"><span data-stu-id="a0d57-109">Property</span></span>|<span data-ttu-id="a0d57-110">类型</span><span class="sxs-lookup"><span data-stu-id="a0d57-110">Type</span></span>|<span data-ttu-id="a0d57-111">说明</span><span class="sxs-lookup"><span data-stu-id="a0d57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d57-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="a0d57-112">ruleType</span></span>|[<span data-ttu-id="a0d57-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="a0d57-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="a0d57-114">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="a0d57-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="a0d57-115">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="a0d57-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="a0d57-116">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="a0d57-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="a0d57-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a0d57-117">displayName</span></span>|<span data-ttu-id="a0d57-118">String</span><span class="sxs-lookup"><span data-stu-id="a0d57-118">String</span></span>|<span data-ttu-id="a0d57-119">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a0d57-119">The display name for the rule.</span></span> <span data-ttu-id="a0d57-120">如果规则用于检测，请勿指定此值。</span><span class="sxs-lookup"><span data-stu-id="a0d57-120">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="a0d57-121">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="a0d57-121">enforceSignatureCheck</span></span>|<span data-ttu-id="a0d57-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0d57-122">Boolean</span></span>|<span data-ttu-id="a0d57-123">一个指示是否强制执行签名检查的值。</span><span class="sxs-lookup"><span data-stu-id="a0d57-123">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="a0d57-124">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="a0d57-124">runAs32Bit</span></span>|<span data-ttu-id="a0d57-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0d57-125">Boolean</span></span>|<span data-ttu-id="a0d57-126">一个指示脚本是否应作为32位运行的值。</span><span class="sxs-lookup"><span data-stu-id="a0d57-126">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="a0d57-127">scriptContent</span><span class="sxs-lookup"><span data-stu-id="a0d57-127">scriptContent</span></span>|<span data-ttu-id="a0d57-128">String</span><span class="sxs-lookup"><span data-stu-id="a0d57-128">String</span></span>|<span data-ttu-id="a0d57-129">Base64 编码的脚本内容。</span><span class="sxs-lookup"><span data-stu-id="a0d57-129">The base64-encoded script content.</span></span>|
|<span data-ttu-id="a0d57-130">operationType</span><span class="sxs-lookup"><span data-stu-id="a0d57-130">operationType</span></span>|[<span data-ttu-id="a0d57-131">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="a0d57-131">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="a0d57-132">脚本输出比较操作类型。</span><span class="sxs-lookup"><span data-stu-id="a0d57-132">The script output comparison operation type.</span></span> <span data-ttu-id="a0d57-133">如果规则用于检测，则使用 NotConfigured (默认值) 。</span><span class="sxs-lookup"><span data-stu-id="a0d57-133">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="a0d57-134">可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version` 或 `boolean`。</span><span class="sxs-lookup"><span data-stu-id="a0d57-134">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="a0d57-135">operator</span><span class="sxs-lookup"><span data-stu-id="a0d57-135">operator</span></span>|[<span data-ttu-id="a0d57-136">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="a0d57-136">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="a0d57-137">脚本输出运算符。</span><span class="sxs-lookup"><span data-stu-id="a0d57-137">The script output operator.</span></span> <span data-ttu-id="a0d57-138">如果规则用于检测，则使用 NotConfigured (默认值) 。</span><span class="sxs-lookup"><span data-stu-id="a0d57-138">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="a0d57-139">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="a0d57-139">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a0d57-140">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="a0d57-140">comparisonValue</span></span>|<span data-ttu-id="a0d57-141">String</span><span class="sxs-lookup"><span data-stu-id="a0d57-141">String</span></span>|<span data-ttu-id="a0d57-142">脚本输出比较值。</span><span class="sxs-lookup"><span data-stu-id="a0d57-142">The script output comparison value.</span></span> <span data-ttu-id="a0d57-143">如果规则用于检测，请勿指定值。</span><span class="sxs-lookup"><span data-stu-id="a0d57-143">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0d57-144">关系</span><span class="sxs-lookup"><span data-stu-id="a0d57-144">Relationships</span></span>
<span data-ttu-id="a0d57-145">无</span><span class="sxs-lookup"><span data-stu-id="a0d57-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0d57-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0d57-146">JSON Representation</span></span>
<span data-ttu-id="a0d57-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0d57-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRule",
  "ruleType": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```





