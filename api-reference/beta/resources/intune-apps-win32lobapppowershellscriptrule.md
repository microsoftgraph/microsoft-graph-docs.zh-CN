---
title: win32LobAppPowerShellScriptRule 资源类型
description: 用于存储 Win32 LOB 应用程序的 PowerShell 脚本规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ce2080b2907f8c691282b44ba6f6ff1ec57a6ed
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792707"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="10022-103">win32LobAppPowerShellScriptRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="10022-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="10022-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10022-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10022-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10022-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10022-107">用于存储 Win32 LOB 应用程序的 PowerShell 脚本规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="10022-107">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="10022-108">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="10022-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="10022-109">属性</span><span class="sxs-lookup"><span data-stu-id="10022-109">Properties</span></span>
|<span data-ttu-id="10022-110">属性</span><span class="sxs-lookup"><span data-stu-id="10022-110">Property</span></span>|<span data-ttu-id="10022-111">类型</span><span class="sxs-lookup"><span data-stu-id="10022-111">Type</span></span>|<span data-ttu-id="10022-112">说明</span><span class="sxs-lookup"><span data-stu-id="10022-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10022-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="10022-113">ruleType</span></span>|[<span data-ttu-id="10022-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="10022-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="10022-115">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="10022-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="10022-116">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="10022-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="10022-117">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="10022-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="10022-118">displayName</span><span class="sxs-lookup"><span data-stu-id="10022-118">displayName</span></span>|<span data-ttu-id="10022-119">String</span><span class="sxs-lookup"><span data-stu-id="10022-119">String</span></span>|<span data-ttu-id="10022-120">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="10022-120">The display name for the rule.</span></span> <span data-ttu-id="10022-121">如果规则用于检测，请勿指定此值。</span><span class="sxs-lookup"><span data-stu-id="10022-121">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="10022-122">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="10022-122">enforceSignatureCheck</span></span>|<span data-ttu-id="10022-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="10022-123">Boolean</span></span>|<span data-ttu-id="10022-124">一个指示是否强制执行签名检查的值。</span><span class="sxs-lookup"><span data-stu-id="10022-124">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="10022-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="10022-125">runAs32Bit</span></span>|<span data-ttu-id="10022-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="10022-126">Boolean</span></span>|<span data-ttu-id="10022-127">一个指示脚本是否应作为32位运行的值。</span><span class="sxs-lookup"><span data-stu-id="10022-127">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="10022-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="10022-128">runAsAccount</span></span>|[<span data-ttu-id="10022-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="10022-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="10022-130">脚本的执行上下文。</span><span class="sxs-lookup"><span data-stu-id="10022-130">The execution context of the script.</span></span> <span data-ttu-id="10022-131">如果规则用于检测，请勿指定此值。</span><span class="sxs-lookup"><span data-stu-id="10022-131">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="10022-132">脚本检测规则将在与关联的应用程序安装上下文相同的上下文中运行。</span><span class="sxs-lookup"><span data-stu-id="10022-132">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="10022-133">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="10022-133">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="10022-134">scriptContent</span><span class="sxs-lookup"><span data-stu-id="10022-134">scriptContent</span></span>|<span data-ttu-id="10022-135">String</span><span class="sxs-lookup"><span data-stu-id="10022-135">String</span></span>|<span data-ttu-id="10022-136">Base64 编码的脚本内容。</span><span class="sxs-lookup"><span data-stu-id="10022-136">The base64-encoded script content.</span></span>|
|<span data-ttu-id="10022-137">operationType</span><span class="sxs-lookup"><span data-stu-id="10022-137">operationType</span></span>|[<span data-ttu-id="10022-138">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="10022-138">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="10022-139">脚本输出比较操作类型。</span><span class="sxs-lookup"><span data-stu-id="10022-139">The script output comparison operation type.</span></span> <span data-ttu-id="10022-140">如果规则用于检测，则使用 NotConfigured (默认值) 。</span><span class="sxs-lookup"><span data-stu-id="10022-140">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="10022-141">可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version` 或 `boolean`。</span><span class="sxs-lookup"><span data-stu-id="10022-141">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="10022-142">operator</span><span class="sxs-lookup"><span data-stu-id="10022-142">operator</span></span>|[<span data-ttu-id="10022-143">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="10022-143">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="10022-144">脚本输出运算符。</span><span class="sxs-lookup"><span data-stu-id="10022-144">The script output operator.</span></span> <span data-ttu-id="10022-145">如果规则用于检测，则使用 NotConfigured (默认值) 。</span><span class="sxs-lookup"><span data-stu-id="10022-145">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="10022-146">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="10022-146">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="10022-147">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="10022-147">comparisonValue</span></span>|<span data-ttu-id="10022-148">String</span><span class="sxs-lookup"><span data-stu-id="10022-148">String</span></span>|<span data-ttu-id="10022-149">脚本输出比较值。</span><span class="sxs-lookup"><span data-stu-id="10022-149">The script output comparison value.</span></span> <span data-ttu-id="10022-150">如果规则用于检测，请勿指定值。</span><span class="sxs-lookup"><span data-stu-id="10022-150">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10022-151">关系</span><span class="sxs-lookup"><span data-stu-id="10022-151">Relationships</span></span>
<span data-ttu-id="10022-152">无</span><span class="sxs-lookup"><span data-stu-id="10022-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10022-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10022-153">JSON Representation</span></span>
<span data-ttu-id="10022-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10022-154">Here is a JSON representation of the resource.</span></span>
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



