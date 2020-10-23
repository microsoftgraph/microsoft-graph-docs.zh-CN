---
title: win32LobAppPowerShellScriptRequirement 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 262800b2285ba2483f97f35f0d39f9d3e7209ee0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694046"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="e98f0-103">win32LobAppPowerShellScriptRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="e98f0-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

<span data-ttu-id="e98f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e98f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e98f0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e98f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e98f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e98f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e98f0-107">包含用于检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="e98f0-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="e98f0-108">继承自 [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="e98f0-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e98f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="e98f0-109">Properties</span></span>
|<span data-ttu-id="e98f0-110">属性</span><span class="sxs-lookup"><span data-stu-id="e98f0-110">Property</span></span>|<span data-ttu-id="e98f0-111">类型</span><span class="sxs-lookup"><span data-stu-id="e98f0-111">Type</span></span>|<span data-ttu-id="e98f0-112">说明</span><span class="sxs-lookup"><span data-stu-id="e98f0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e98f0-113">operator</span><span class="sxs-lookup"><span data-stu-id="e98f0-113">operator</span></span>|[<span data-ttu-id="e98f0-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="e98f0-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="e98f0-115">从 [Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="e98f0-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="e98f0-116">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="e98f0-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e98f0-117">detectionValue</span><span class="sxs-lookup"><span data-stu-id="e98f0-117">detectionValue</span></span>|<span data-ttu-id="e98f0-118">String</span><span class="sxs-lookup"><span data-stu-id="e98f0-118">String</span></span>|<span data-ttu-id="e98f0-119">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="e98f0-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="e98f0-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e98f0-120">displayName</span></span>|<span data-ttu-id="e98f0-121">String</span><span class="sxs-lookup"><span data-stu-id="e98f0-121">String</span></span>|<span data-ttu-id="e98f0-122">此规则的唯一显示名称</span><span class="sxs-lookup"><span data-stu-id="e98f0-122">The unique display name for this rule</span></span>|
|<span data-ttu-id="e98f0-123">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="e98f0-123">enforceSignatureCheck</span></span>|<span data-ttu-id="e98f0-124">布尔</span><span class="sxs-lookup"><span data-stu-id="e98f0-124">Boolean</span></span>|<span data-ttu-id="e98f0-125">一个指示是否强制执行签名检查的值</span><span class="sxs-lookup"><span data-stu-id="e98f0-125">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="e98f0-126">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="e98f0-126">runAs32Bit</span></span>|<span data-ttu-id="e98f0-127">布尔</span><span class="sxs-lookup"><span data-stu-id="e98f0-127">Boolean</span></span>|<span data-ttu-id="e98f0-128">一个指示此脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="e98f0-128">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="e98f0-129">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="e98f0-129">runAsAccount</span></span>|[<span data-ttu-id="e98f0-130">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="e98f0-130">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="e98f0-131">指示脚本在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="e98f0-131">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="e98f0-132">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="e98f0-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="e98f0-133">scriptContent</span><span class="sxs-lookup"><span data-stu-id="e98f0-133">scriptContent</span></span>|<span data-ttu-id="e98f0-134">String</span><span class="sxs-lookup"><span data-stu-id="e98f0-134">String</span></span>|<span data-ttu-id="e98f0-135">用于检测 Win32 业务线 (LoB) 应用程序的 base64 编码的脚本内容</span><span class="sxs-lookup"><span data-stu-id="e98f0-135">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e98f0-136">detectionType</span><span class="sxs-lookup"><span data-stu-id="e98f0-136">detectionType</span></span>|[<span data-ttu-id="e98f0-137">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="e98f0-137">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="e98f0-138">脚本输出的检测类型。</span><span class="sxs-lookup"><span data-stu-id="e98f0-138">The detection type for script output.</span></span> <span data-ttu-id="e98f0-139">可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version`、`boolean`。</span><span class="sxs-lookup"><span data-stu-id="e98f0-139">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e98f0-140">关系</span><span class="sxs-lookup"><span data-stu-id="e98f0-140">Relationships</span></span>
<span data-ttu-id="e98f0-141">无</span><span class="sxs-lookup"><span data-stu-id="e98f0-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e98f0-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e98f0-142">JSON Representation</span></span>
<span data-ttu-id="e98f0-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e98f0-143">Here is a JSON representation of the resource.</span></span>
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





