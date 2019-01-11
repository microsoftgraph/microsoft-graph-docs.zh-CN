---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含要检测 Win32 应用程序的 PowerShell 脚本属性
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bdd3c0e6864a3568b4f1efb7c1c18a25f3e7c84d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863026"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="cdeda-103">win32LobAppPowerShellScriptDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdeda-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="cdeda-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cdeda-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdeda-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cdeda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdeda-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cdeda-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdeda-107">包含要检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="cdeda-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="cdeda-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="cdeda-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cdeda-109">属性</span><span class="sxs-lookup"><span data-stu-id="cdeda-109">Properties</span></span>
|<span data-ttu-id="cdeda-110">属性</span><span class="sxs-lookup"><span data-stu-id="cdeda-110">Property</span></span>|<span data-ttu-id="cdeda-111">类型</span><span class="sxs-lookup"><span data-stu-id="cdeda-111">Type</span></span>|<span data-ttu-id="cdeda-112">Description</span><span class="sxs-lookup"><span data-stu-id="cdeda-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdeda-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="cdeda-113">enforceSignatureCheck</span></span>|<span data-ttu-id="cdeda-114">布尔</span><span class="sxs-lookup"><span data-stu-id="cdeda-114">Boolean</span></span>|<span data-ttu-id="cdeda-115">一个值，指示是否强制执行签名检查</span><span class="sxs-lookup"><span data-stu-id="cdeda-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="cdeda-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="cdeda-116">runAs32Bit</span></span>|<span data-ttu-id="cdeda-117">布尔</span><span class="sxs-lookup"><span data-stu-id="cdeda-117">Boolean</span></span>|<span data-ttu-id="cdeda-118">指示是否应运行此脚本为 32 位的值</span><span class="sxs-lookup"><span data-stu-id="cdeda-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="cdeda-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="cdeda-119">scriptContent</span></span>|<span data-ttu-id="cdeda-120">字符串</span><span class="sxs-lookup"><span data-stu-id="cdeda-120">String</span></span>|<span data-ttu-id="cdeda-121">以 base64 编码的脚本内容来检测 Win32 业务线 (LoB) 应用程序</span><span class="sxs-lookup"><span data-stu-id="cdeda-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdeda-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="cdeda-122">Relationships</span></span>
<span data-ttu-id="cdeda-123">无</span><span class="sxs-lookup"><span data-stu-id="cdeda-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cdeda-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdeda-124">JSON Representation</span></span>
<span data-ttu-id="cdeda-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdeda-125">Here is a JSON representation of the resource.</span></span>
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





