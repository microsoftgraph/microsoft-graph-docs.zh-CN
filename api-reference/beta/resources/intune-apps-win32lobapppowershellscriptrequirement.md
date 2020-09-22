---
title: win32LobAppPowerShellScriptRequirement 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b16f303f0a8ee4fd8855529a0908269e11c4d72d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092837"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="65450-103">win32LobAppPowerShellScriptRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="65450-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

<span data-ttu-id="65450-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65450-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65450-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65450-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65450-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65450-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65450-107">包含用于检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="65450-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="65450-108">继承自 [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="65450-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65450-109">属性</span><span class="sxs-lookup"><span data-stu-id="65450-109">Properties</span></span>
|<span data-ttu-id="65450-110">属性</span><span class="sxs-lookup"><span data-stu-id="65450-110">Property</span></span>|<span data-ttu-id="65450-111">类型</span><span class="sxs-lookup"><span data-stu-id="65450-111">Type</span></span>|<span data-ttu-id="65450-112">说明</span><span class="sxs-lookup"><span data-stu-id="65450-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65450-113">operator</span><span class="sxs-lookup"><span data-stu-id="65450-113">operator</span></span>|[<span data-ttu-id="65450-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="65450-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="65450-115">从 [Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="65450-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="65450-116">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="65450-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="65450-117">detectionValue</span><span class="sxs-lookup"><span data-stu-id="65450-117">detectionValue</span></span>|<span data-ttu-id="65450-118">字符串</span><span class="sxs-lookup"><span data-stu-id="65450-118">String</span></span>|<span data-ttu-id="65450-119">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="65450-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="65450-120">displayName</span><span class="sxs-lookup"><span data-stu-id="65450-120">displayName</span></span>|<span data-ttu-id="65450-121">字符串</span><span class="sxs-lookup"><span data-stu-id="65450-121">String</span></span>|<span data-ttu-id="65450-122">此规则的唯一显示名称</span><span class="sxs-lookup"><span data-stu-id="65450-122">The unique display name for this rule</span></span>|
|<span data-ttu-id="65450-123">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="65450-123">enforceSignatureCheck</span></span>|<span data-ttu-id="65450-124">布尔</span><span class="sxs-lookup"><span data-stu-id="65450-124">Boolean</span></span>|<span data-ttu-id="65450-125">一个指示是否强制执行签名检查的值</span><span class="sxs-lookup"><span data-stu-id="65450-125">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="65450-126">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="65450-126">runAs32Bit</span></span>|<span data-ttu-id="65450-127">布尔</span><span class="sxs-lookup"><span data-stu-id="65450-127">Boolean</span></span>|<span data-ttu-id="65450-128">一个指示此脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="65450-128">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="65450-129">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="65450-129">runAsAccount</span></span>|[<span data-ttu-id="65450-130">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="65450-130">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="65450-131">指示脚本在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="65450-131">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="65450-132">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="65450-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="65450-133">scriptContent</span><span class="sxs-lookup"><span data-stu-id="65450-133">scriptContent</span></span>|<span data-ttu-id="65450-134">字符串</span><span class="sxs-lookup"><span data-stu-id="65450-134">String</span></span>|<span data-ttu-id="65450-135">用于检测 Win32 业务线 (LoB) 应用程序的 base64 编码的脚本内容</span><span class="sxs-lookup"><span data-stu-id="65450-135">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="65450-136">detectionType</span><span class="sxs-lookup"><span data-stu-id="65450-136">detectionType</span></span>|[<span data-ttu-id="65450-137">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="65450-137">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="65450-138">脚本输出的检测类型。</span><span class="sxs-lookup"><span data-stu-id="65450-138">The detection type for script output.</span></span> <span data-ttu-id="65450-139">可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version`、`boolean`。</span><span class="sxs-lookup"><span data-stu-id="65450-139">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65450-140">关系</span><span class="sxs-lookup"><span data-stu-id="65450-140">Relationships</span></span>
<span data-ttu-id="65450-141">无</span><span class="sxs-lookup"><span data-stu-id="65450-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65450-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65450-142">JSON Representation</span></span>
<span data-ttu-id="65450-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65450-143">Here is a JSON representation of the resource.</span></span>
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






