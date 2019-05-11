---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识您的展台配置的 UWP 应用信息的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 276cbe4c231425540037dcc9a9e0afe977220bc0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944010"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="7452e-103">windowsKioskSingleUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="7452e-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="7452e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7452e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7452e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7452e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7452e-106">用于标识您的展台配置的 UWP 应用信息的类</span><span class="sxs-lookup"><span data-stu-id="7452e-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="7452e-107">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7452e-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7452e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7452e-108">Properties</span></span>
|<span data-ttu-id="7452e-109">属性</span><span class="sxs-lookup"><span data-stu-id="7452e-109">Property</span></span>|<span data-ttu-id="7452e-110">类型</span><span class="sxs-lookup"><span data-stu-id="7452e-110">Type</span></span>|<span data-ttu-id="7452e-111">说明</span><span class="sxs-lookup"><span data-stu-id="7452e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7452e-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="7452e-112">uwpApp</span></span>|[<span data-ttu-id="7452e-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="7452e-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="7452e-114">这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)</span><span class="sxs-lookup"><span data-stu-id="7452e-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="7452e-115">关系</span><span class="sxs-lookup"><span data-stu-id="7452e-115">Relationships</span></span>
<span data-ttu-id="7452e-116">无</span><span class="sxs-lookup"><span data-stu-id="7452e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7452e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7452e-117">JSON Representation</span></span>
<span data-ttu-id="7452e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7452e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




