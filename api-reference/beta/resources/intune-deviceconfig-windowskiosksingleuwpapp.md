---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识您的展台配置的 UWP 应用信息的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3bb9c57de0e3e60d1c62adb62c3d1a274c6f853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574650"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="d5f85-103">windowsKioskSingleUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5f85-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="d5f85-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5f85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5f85-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5f85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5f85-106">用于标识您的展台配置的 UWP 应用信息的类</span><span class="sxs-lookup"><span data-stu-id="d5f85-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="d5f85-107">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f85-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5f85-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5f85-108">Properties</span></span>
|<span data-ttu-id="d5f85-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5f85-109">Property</span></span>|<span data-ttu-id="d5f85-110">类型</span><span class="sxs-lookup"><span data-stu-id="d5f85-110">Type</span></span>|<span data-ttu-id="d5f85-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5f85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5f85-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="d5f85-112">uwpApp</span></span>|[<span data-ttu-id="d5f85-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="d5f85-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="d5f85-114">这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)</span><span class="sxs-lookup"><span data-stu-id="d5f85-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5f85-115">关系</span><span class="sxs-lookup"><span data-stu-id="d5f85-115">Relationships</span></span>
<span data-ttu-id="d5f85-116">无</span><span class="sxs-lookup"><span data-stu-id="d5f85-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5f85-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5f85-117">JSON Representation</span></span>
<span data-ttu-id="d5f85-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5f85-118">Here is a JSON representation of the resource.</span></span>
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





