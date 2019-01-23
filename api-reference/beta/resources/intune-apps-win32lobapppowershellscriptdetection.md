---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含要检测 Win32 应用程序的 PowerShell 脚本属性
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5c02228589042d0abf36c34c5818c5a4610514e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399638"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="81d89-103">win32LobAppPowerShellScriptDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="81d89-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="81d89-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="81d89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81d89-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81d89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81d89-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81d89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81d89-107">包含要检测 Win32 应用程序的 PowerShell 脚本属性</span><span class="sxs-lookup"><span data-stu-id="81d89-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="81d89-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="81d89-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81d89-109">属性</span><span class="sxs-lookup"><span data-stu-id="81d89-109">Properties</span></span>
|<span data-ttu-id="81d89-110">属性</span><span class="sxs-lookup"><span data-stu-id="81d89-110">Property</span></span>|<span data-ttu-id="81d89-111">类型</span><span class="sxs-lookup"><span data-stu-id="81d89-111">Type</span></span>|<span data-ttu-id="81d89-112">说明</span><span class="sxs-lookup"><span data-stu-id="81d89-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d89-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="81d89-113">enforceSignatureCheck</span></span>|<span data-ttu-id="81d89-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="81d89-114">Boolean</span></span>|<span data-ttu-id="81d89-115">一个值，指示是否强制执行签名检查</span><span class="sxs-lookup"><span data-stu-id="81d89-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="81d89-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="81d89-116">runAs32Bit</span></span>|<span data-ttu-id="81d89-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="81d89-117">Boolean</span></span>|<span data-ttu-id="81d89-118">指示是否应运行此脚本为 32 位的值</span><span class="sxs-lookup"><span data-stu-id="81d89-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="81d89-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="81d89-119">scriptContent</span></span>|<span data-ttu-id="81d89-120">String</span><span class="sxs-lookup"><span data-stu-id="81d89-120">String</span></span>|<span data-ttu-id="81d89-121">以 base64 编码的脚本内容来检测 Win32 业务线 (LoB) 应用程序</span><span class="sxs-lookup"><span data-stu-id="81d89-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="81d89-122">关系</span><span class="sxs-lookup"><span data-stu-id="81d89-122">Relationships</span></span>
<span data-ttu-id="81d89-123">无</span><span class="sxs-lookup"><span data-stu-id="81d89-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81d89-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81d89-124">JSON Representation</span></span>
<span data-ttu-id="81d89-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81d89-125">Here is a JSON representation of the resource.</span></span>
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




