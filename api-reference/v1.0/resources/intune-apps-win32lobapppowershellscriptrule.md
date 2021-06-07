---
title: win32LobAppPowerShellScriptRule 资源类型
description: 用于存储 Win32 LOB 应用的 PowerShell 脚本规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcc9afa8f58462bda69c96990e37529667d20445
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758986"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="b4e19-103">win32LobAppPowerShellScriptRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4e19-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="b4e19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4e19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4e19-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4e19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4e19-106">用于存储 Win32 LOB 应用的 PowerShell 脚本规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="b4e19-106">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="b4e19-107">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="b4e19-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4e19-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4e19-108">Properties</span></span>
|<span data-ttu-id="b4e19-109">属性</span><span class="sxs-lookup"><span data-stu-id="b4e19-109">Property</span></span>|<span data-ttu-id="b4e19-110">类型</span><span class="sxs-lookup"><span data-stu-id="b4e19-110">Type</span></span>|<span data-ttu-id="b4e19-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4e19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e19-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="b4e19-112">ruleType</span></span>|[<span data-ttu-id="b4e19-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="b4e19-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="b4e19-114">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="b4e19-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="b4e19-115">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="b4e19-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="b4e19-116">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="b4e19-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="b4e19-117">displayName</span><span class="sxs-lookup"><span data-stu-id="b4e19-117">displayName</span></span>|<span data-ttu-id="b4e19-118">String</span><span class="sxs-lookup"><span data-stu-id="b4e19-118">String</span></span>|<span data-ttu-id="b4e19-119">规则显示名称的项。</span><span class="sxs-lookup"><span data-stu-id="b4e19-119">The display name for the rule.</span></span> <span data-ttu-id="b4e19-120">如果规则用于检测，则不要指定此值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-120">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="b4e19-121">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="b4e19-121">enforceSignatureCheck</span></span>|<span data-ttu-id="b4e19-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e19-122">Boolean</span></span>|<span data-ttu-id="b4e19-123">指示是否强制执行签名检查的值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-123">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="b4e19-124">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="b4e19-124">runAs32Bit</span></span>|<span data-ttu-id="b4e19-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4e19-125">Boolean</span></span>|<span data-ttu-id="b4e19-126">指示脚本是否应该作为 32 位运行的值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-126">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="b4e19-127">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="b4e19-127">runAsAccount</span></span>|[<span data-ttu-id="b4e19-128">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="b4e19-128">runAsAccountType</span></span>](../resources/intune-apps-runasaccounttype.md)|<span data-ttu-id="b4e19-129">脚本的执行上下文。</span><span class="sxs-lookup"><span data-stu-id="b4e19-129">The execution context of the script.</span></span> <span data-ttu-id="b4e19-130">如果规则用于检测，则不要指定此值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-130">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="b4e19-131">脚本检测规则将在与关联的应用安装上下文相同的上下文中运行。</span><span class="sxs-lookup"><span data-stu-id="b4e19-131">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="b4e19-132">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="b4e19-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="b4e19-133">scriptContent</span><span class="sxs-lookup"><span data-stu-id="b4e19-133">scriptContent</span></span>|<span data-ttu-id="b4e19-134">String</span><span class="sxs-lookup"><span data-stu-id="b4e19-134">String</span></span>|<span data-ttu-id="b4e19-135">base64 编码的脚本内容。</span><span class="sxs-lookup"><span data-stu-id="b4e19-135">The base64-encoded script content.</span></span>|
|<span data-ttu-id="b4e19-136">operationType</span><span class="sxs-lookup"><span data-stu-id="b4e19-136">operationType</span></span>|[<span data-ttu-id="b4e19-137">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="b4e19-137">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="b4e19-138">脚本输出比较操作类型。</span><span class="sxs-lookup"><span data-stu-id="b4e19-138">The script output comparison operation type.</span></span> <span data-ttu-id="b4e19-139">如果规则用于 (，) 使用 NotConfigured 作为默认值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-139">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="b4e19-140">可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version` 或 `boolean`。</span><span class="sxs-lookup"><span data-stu-id="b4e19-140">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="b4e19-141">operator</span><span class="sxs-lookup"><span data-stu-id="b4e19-141">operator</span></span>|[<span data-ttu-id="b4e19-142">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="b4e19-142">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="b4e19-143">脚本输出运算符。</span><span class="sxs-lookup"><span data-stu-id="b4e19-143">The script output operator.</span></span> <span data-ttu-id="b4e19-144">如果规则用于 (，) 使用 NotConfigured 作为默认值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-144">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="b4e19-145">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="b4e19-145">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="b4e19-146">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="b4e19-146">comparisonValue</span></span>|<span data-ttu-id="b4e19-147">String</span><span class="sxs-lookup"><span data-stu-id="b4e19-147">String</span></span>|<span data-ttu-id="b4e19-148">脚本输出比较值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-148">The script output comparison value.</span></span> <span data-ttu-id="b4e19-149">如果规则用于检测，则不指定值。</span><span class="sxs-lookup"><span data-stu-id="b4e19-149">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4e19-150">关系</span><span class="sxs-lookup"><span data-stu-id="b4e19-150">Relationships</span></span>
<span data-ttu-id="b4e19-151">无</span><span class="sxs-lookup"><span data-stu-id="b4e19-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4e19-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4e19-152">JSON Representation</span></span>
<span data-ttu-id="b4e19-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4e19-153">Here is a JSON representation of the resource.</span></span>
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
  "runAsAccount": "String",
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




