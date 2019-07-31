---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0ad0dd613182bdd54574e0ef25b107f8b6b6dc2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012252"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="af544-103">win32LobAppPowerShellScriptDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="af544-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="af544-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af544-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af544-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af544-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af544-106">包含用于检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="af544-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="af544-107">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="af544-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af544-108">属性</span><span class="sxs-lookup"><span data-stu-id="af544-108">Properties</span></span>
|<span data-ttu-id="af544-109">属性</span><span class="sxs-lookup"><span data-stu-id="af544-109">Property</span></span>|<span data-ttu-id="af544-110">类型</span><span class="sxs-lookup"><span data-stu-id="af544-110">Type</span></span>|<span data-ttu-id="af544-111">说明</span><span class="sxs-lookup"><span data-stu-id="af544-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af544-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="af544-112">enforceSignatureCheck</span></span>|<span data-ttu-id="af544-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="af544-113">Boolean</span></span>|<span data-ttu-id="af544-114">一个指示是否强制执行签名检查的值</span><span class="sxs-lookup"><span data-stu-id="af544-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="af544-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="af544-115">runAs32Bit</span></span>|<span data-ttu-id="af544-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="af544-116">Boolean</span></span>|<span data-ttu-id="af544-117">一个指示此脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="af544-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="af544-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="af544-118">scriptContent</span></span>|<span data-ttu-id="af544-119">String</span><span class="sxs-lookup"><span data-stu-id="af544-119">String</span></span>|<span data-ttu-id="af544-120">用于检测 Win32 业务线 (LoB) 应用程序的 base64 编码的脚本内容</span><span class="sxs-lookup"><span data-stu-id="af544-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="af544-121">关系</span><span class="sxs-lookup"><span data-stu-id="af544-121">Relationships</span></span>
<span data-ttu-id="af544-122">无</span><span class="sxs-lookup"><span data-stu-id="af544-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af544-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af544-123">JSON Representation</span></span>
<span data-ttu-id="af544-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af544-124">Here is a JSON representation of the resource.</span></span>
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





