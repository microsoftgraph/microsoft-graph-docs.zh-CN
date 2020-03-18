---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5efcfdc14c2c32b51db04a93da4aff5730106219
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797610"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="ee9b9-103">win32LobAppPowerShellScriptDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee9b9-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="ee9b9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee9b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee9b9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee9b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee9b9-106">包含用于检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="ee9b9-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="ee9b9-107">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="ee9b9-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee9b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee9b9-108">Properties</span></span>
|<span data-ttu-id="ee9b9-109">属性</span><span class="sxs-lookup"><span data-stu-id="ee9b9-109">Property</span></span>|<span data-ttu-id="ee9b9-110">类型</span><span class="sxs-lookup"><span data-stu-id="ee9b9-110">Type</span></span>|<span data-ttu-id="ee9b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="ee9b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee9b9-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="ee9b9-112">enforceSignatureCheck</span></span>|<span data-ttu-id="ee9b9-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="ee9b9-113">Boolean</span></span>|<span data-ttu-id="ee9b9-114">一个指示是否强制执行签名检查的值</span><span class="sxs-lookup"><span data-stu-id="ee9b9-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="ee9b9-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="ee9b9-115">runAs32Bit</span></span>|<span data-ttu-id="ee9b9-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="ee9b9-116">Boolean</span></span>|<span data-ttu-id="ee9b9-117">一个指示此脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="ee9b9-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="ee9b9-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="ee9b9-118">scriptContent</span></span>|<span data-ttu-id="ee9b9-119">String</span><span class="sxs-lookup"><span data-stu-id="ee9b9-119">String</span></span>|<span data-ttu-id="ee9b9-120">用于检测 Win32 业务线（LoB）应用程序的 base64 编码的脚本内容</span><span class="sxs-lookup"><span data-stu-id="ee9b9-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee9b9-121">关系</span><span class="sxs-lookup"><span data-stu-id="ee9b9-121">Relationships</span></span>
<span data-ttu-id="ee9b9-122">无</span><span class="sxs-lookup"><span data-stu-id="ee9b9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee9b9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee9b9-123">JSON Representation</span></span>
<span data-ttu-id="ee9b9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee9b9-124">Here is a JSON representation of the resource.</span></span>
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



