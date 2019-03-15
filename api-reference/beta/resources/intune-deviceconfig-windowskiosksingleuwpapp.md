---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识您的展台配置的 UWP 应用信息的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0a3b56c7bc9856b98708b63c247479e6ccf9c9b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571156"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="ebce7-103">windowsKioskSingleUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebce7-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="ebce7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebce7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebce7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebce7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebce7-106">用于标识您的展台配置的 UWP 应用信息的类</span><span class="sxs-lookup"><span data-stu-id="ebce7-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="ebce7-107">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebce7-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebce7-108">属性</span><span class="sxs-lookup"><span data-stu-id="ebce7-108">Properties</span></span>
|<span data-ttu-id="ebce7-109">属性</span><span class="sxs-lookup"><span data-stu-id="ebce7-109">Property</span></span>|<span data-ttu-id="ebce7-110">类型</span><span class="sxs-lookup"><span data-stu-id="ebce7-110">Type</span></span>|<span data-ttu-id="ebce7-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebce7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebce7-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="ebce7-112">uwpApp</span></span>|[<span data-ttu-id="ebce7-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="ebce7-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="ebce7-114">这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)</span><span class="sxs-lookup"><span data-stu-id="ebce7-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebce7-115">关系</span><span class="sxs-lookup"><span data-stu-id="ebce7-115">Relationships</span></span>
<span data-ttu-id="ebce7-116">无</span><span class="sxs-lookup"><span data-stu-id="ebce7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebce7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebce7-117">JSON Representation</span></span>
<span data-ttu-id="ebce7-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebce7-118">Here is a JSON representation of the resource.</span></span>
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




