---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识网亭配置 UWP 应用程序信息的类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c11469784e2c450b151c9a81a07f6c1568cf3a3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818142"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="c1f61-103">windowsKioskSingleUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1f61-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="c1f61-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c1f61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1f61-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1f61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1f61-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c1f61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1f61-107">用于标识网亭配置 UWP 应用程序信息的类</span><span class="sxs-lookup"><span data-stu-id="c1f61-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="c1f61-108">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1f61-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1f61-109">属性</span><span class="sxs-lookup"><span data-stu-id="c1f61-109">Properties</span></span>
|<span data-ttu-id="c1f61-110">属性</span><span class="sxs-lookup"><span data-stu-id="c1f61-110">Property</span></span>|<span data-ttu-id="c1f61-111">类型</span><span class="sxs-lookup"><span data-stu-id="c1f61-111">Type</span></span>|<span data-ttu-id="c1f61-112">Description</span><span class="sxs-lookup"><span data-stu-id="c1f61-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1f61-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="c1f61-113">uwpApp</span></span>|[<span data-ttu-id="c1f61-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="c1f61-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="c1f61-115">这是仅应用程序用户模型 ID (AUMID) 将可用于启动在展台模式中使用</span><span class="sxs-lookup"><span data-stu-id="c1f61-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1f61-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="c1f61-116">Relationships</span></span>
<span data-ttu-id="c1f61-117">无</span><span class="sxs-lookup"><span data-stu-id="c1f61-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1f61-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1f61-118">JSON Representation</span></span>
<span data-ttu-id="c1f61-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1f61-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





