---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d36591c566e93f9cf4d0c6a7e300224e74033a1b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422917"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="47735-103">win32LobAppPowerShellScriptDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="47735-103">win32LobAppPowerShellScriptDetection resource type</span></span>

<span data-ttu-id="47735-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47735-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47735-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47735-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47735-107">包含用于检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="47735-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="47735-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="47735-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47735-109">属性</span><span class="sxs-lookup"><span data-stu-id="47735-109">Properties</span></span>
|<span data-ttu-id="47735-110">属性</span><span class="sxs-lookup"><span data-stu-id="47735-110">Property</span></span>|<span data-ttu-id="47735-111">类型</span><span class="sxs-lookup"><span data-stu-id="47735-111">Type</span></span>|<span data-ttu-id="47735-112">说明</span><span class="sxs-lookup"><span data-stu-id="47735-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47735-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="47735-113">enforceSignatureCheck</span></span>|<span data-ttu-id="47735-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="47735-114">Boolean</span></span>|<span data-ttu-id="47735-115">一个指示是否强制执行签名检查的值</span><span class="sxs-lookup"><span data-stu-id="47735-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="47735-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="47735-116">runAs32Bit</span></span>|<span data-ttu-id="47735-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="47735-117">Boolean</span></span>|<span data-ttu-id="47735-118">一个指示此脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="47735-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="47735-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="47735-119">scriptContent</span></span>|<span data-ttu-id="47735-120">String</span><span class="sxs-lookup"><span data-stu-id="47735-120">String</span></span>|<span data-ttu-id="47735-121">用于检测 Win32 业务线（LoB）应用程序的 base64 编码的脚本内容</span><span class="sxs-lookup"><span data-stu-id="47735-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="47735-122">关系</span><span class="sxs-lookup"><span data-stu-id="47735-122">Relationships</span></span>
<span data-ttu-id="47735-123">无</span><span class="sxs-lookup"><span data-stu-id="47735-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47735-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47735-124">JSON Representation</span></span>
<span data-ttu-id="47735-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47735-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```



