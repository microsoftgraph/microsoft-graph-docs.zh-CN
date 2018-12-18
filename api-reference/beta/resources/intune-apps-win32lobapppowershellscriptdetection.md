---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含要检测 Win32 应用程序的 PowerShell 脚本属性
author: tfitzmac
ms.openlocfilehash: 7f69b2c066ae90cfcd805b3d3cfe57193046d440
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327571"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="dfc3c-103">win32LobAppPowerShellScriptDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfc3c-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="dfc3c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dfc3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfc3c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dfc3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfc3c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfc3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfc3c-107">包含要检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="dfc3c-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="dfc3c-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="dfc3c-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dfc3c-109">属性</span><span class="sxs-lookup"><span data-stu-id="dfc3c-109">Properties</span></span>
|<span data-ttu-id="dfc3c-110">属性</span><span class="sxs-lookup"><span data-stu-id="dfc3c-110">Property</span></span>|<span data-ttu-id="dfc3c-111">类型</span><span class="sxs-lookup"><span data-stu-id="dfc3c-111">Type</span></span>|<span data-ttu-id="dfc3c-112">说明</span><span class="sxs-lookup"><span data-stu-id="dfc3c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfc3c-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="dfc3c-113">enforceSignatureCheck</span></span>|<span data-ttu-id="dfc3c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfc3c-114">Boolean</span></span>|<span data-ttu-id="dfc3c-115">一个值，指示是否强制执行签名检查</span><span class="sxs-lookup"><span data-stu-id="dfc3c-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="dfc3c-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="dfc3c-116">runAs32Bit</span></span>|<span data-ttu-id="dfc3c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfc3c-117">Boolean</span></span>|<span data-ttu-id="dfc3c-118">指示是否应运行此脚本为 32 位的值</span><span class="sxs-lookup"><span data-stu-id="dfc3c-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="dfc3c-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="dfc3c-119">scriptContent</span></span>|<span data-ttu-id="dfc3c-120">字符串</span><span class="sxs-lookup"><span data-stu-id="dfc3c-120">String</span></span>|<span data-ttu-id="dfc3c-121">以 base64 编码的脚本内容来检测 Win32 业务线 (LoB) 应用程序</span><span class="sxs-lookup"><span data-stu-id="dfc3c-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfc3c-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="dfc3c-122">Relationships</span></span>
<span data-ttu-id="dfc3c-123">无</span><span class="sxs-lookup"><span data-stu-id="dfc3c-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfc3c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfc3c-124">JSON Representation</span></span>
<span data-ttu-id="dfc3c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfc3c-125">Here is a JSON representation of the resource.</span></span>
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





