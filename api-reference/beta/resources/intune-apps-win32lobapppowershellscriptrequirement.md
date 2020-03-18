---
title: win32LobAppPowerShellScriptRequirement 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef7eaa00605214b10438b8c28ba3752903d26bc7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797596"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="c9dc0-103">win32LobAppPowerShellScriptRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9dc0-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

> <span data-ttu-id="c9dc0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9dc0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9dc0-106">包含用于检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="c9dc0-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="c9dc0-107">继承自[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="c9dc0-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9dc0-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9dc0-108">Properties</span></span>
|<span data-ttu-id="c9dc0-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9dc0-109">Property</span></span>|<span data-ttu-id="c9dc0-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9dc0-110">Type</span></span>|<span data-ttu-id="c9dc0-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9dc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9dc0-112">operator</span><span class="sxs-lookup"><span data-stu-id="c9dc0-112">operator</span></span>|[<span data-ttu-id="c9dc0-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="c9dc0-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="c9dc0-114">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="c9dc0-115">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="c9dc0-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="c9dc0-116">detectionValue</span></span>|<span data-ttu-id="c9dc0-117">String</span><span class="sxs-lookup"><span data-stu-id="c9dc0-117">String</span></span>|<span data-ttu-id="c9dc0-118">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="c9dc0-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="c9dc0-119">displayName</span><span class="sxs-lookup"><span data-stu-id="c9dc0-119">displayName</span></span>|<span data-ttu-id="c9dc0-120">String</span><span class="sxs-lookup"><span data-stu-id="c9dc0-120">String</span></span>|<span data-ttu-id="c9dc0-121">此规则的唯一显示名称</span><span class="sxs-lookup"><span data-stu-id="c9dc0-121">The unique display name for this rule</span></span>|
|<span data-ttu-id="c9dc0-122">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="c9dc0-122">enforceSignatureCheck</span></span>|<span data-ttu-id="c9dc0-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="c9dc0-123">Boolean</span></span>|<span data-ttu-id="c9dc0-124">一个指示是否强制执行签名检查的值</span><span class="sxs-lookup"><span data-stu-id="c9dc0-124">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="c9dc0-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="c9dc0-125">runAs32Bit</span></span>|<span data-ttu-id="c9dc0-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="c9dc0-126">Boolean</span></span>|<span data-ttu-id="c9dc0-127">一个指示此脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="c9dc0-127">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="c9dc0-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c9dc0-128">runAsAccount</span></span>|[<span data-ttu-id="c9dc0-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c9dc0-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c9dc0-130">指示脚本在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-130">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="c9dc0-131">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-131">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c9dc0-132">scriptContent</span><span class="sxs-lookup"><span data-stu-id="c9dc0-132">scriptContent</span></span>|<span data-ttu-id="c9dc0-133">String</span><span class="sxs-lookup"><span data-stu-id="c9dc0-133">String</span></span>|<span data-ttu-id="c9dc0-134">用于检测 Win32 业务线（LoB）应用程序的 base64 编码的脚本内容</span><span class="sxs-lookup"><span data-stu-id="c9dc0-134">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="c9dc0-135">detectionType</span><span class="sxs-lookup"><span data-stu-id="c9dc0-135">detectionType</span></span>|[<span data-ttu-id="c9dc0-136">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="c9dc0-136">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="c9dc0-137">脚本输出的检测类型。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-137">The detection type for script output.</span></span> <span data-ttu-id="c9dc0-138">可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version`、`boolean`。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-138">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9dc0-139">关系</span><span class="sxs-lookup"><span data-stu-id="c9dc0-139">Relationships</span></span>
<span data-ttu-id="c9dc0-140">无</span><span class="sxs-lookup"><span data-stu-id="c9dc0-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9dc0-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9dc0-141">JSON Representation</span></span>
<span data-ttu-id="c9dc0-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9dc0-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```



