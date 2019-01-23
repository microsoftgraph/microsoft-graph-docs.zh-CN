---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识网亭配置 UWP 应用程序信息的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e62dc6393cc2dc6a9133732a42527abdfadbd91e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409375"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="5b18f-103">windowsKioskSingleUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b18f-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="5b18f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5b18f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b18f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b18f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b18f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b18f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b18f-107">用于标识网亭配置 UWP 应用程序信息的类</span><span class="sxs-lookup"><span data-stu-id="5b18f-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="5b18f-108">继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b18f-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b18f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b18f-109">Properties</span></span>
|<span data-ttu-id="5b18f-110">属性</span><span class="sxs-lookup"><span data-stu-id="5b18f-110">Property</span></span>|<span data-ttu-id="5b18f-111">类型</span><span class="sxs-lookup"><span data-stu-id="5b18f-111">Type</span></span>|<span data-ttu-id="5b18f-112">说明</span><span class="sxs-lookup"><span data-stu-id="5b18f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b18f-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="5b18f-113">uwpApp</span></span>|[<span data-ttu-id="5b18f-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="5b18f-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="5b18f-115">这是仅应用程序用户模型 ID (AUMID) 将可用于启动在展台模式中使用</span><span class="sxs-lookup"><span data-stu-id="5b18f-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b18f-116">关系</span><span class="sxs-lookup"><span data-stu-id="5b18f-116">Relationships</span></span>
<span data-ttu-id="5b18f-117">无</span><span class="sxs-lookup"><span data-stu-id="5b18f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b18f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b18f-118">JSON Representation</span></span>
<span data-ttu-id="5b18f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b18f-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




