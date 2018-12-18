---
title: windowsKioskUWPApp 资源类型
description: 一种类型的应用程序的基类
author: tfitzmac
ms.openlocfilehash: 328a91065692a7b315ade5dae86c15d6def320eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305178"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="32de8-103">windowsKioskUWPApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="32de8-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="32de8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32de8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32de8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32de8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32de8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="32de8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32de8-107">一种类型的应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="32de8-107">The base class for a type of apps</span></span>

<span data-ttu-id="32de8-108">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="32de8-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32de8-109">属性</span><span class="sxs-lookup"><span data-stu-id="32de8-109">Properties</span></span>
|<span data-ttu-id="32de8-110">属性</span><span class="sxs-lookup"><span data-stu-id="32de8-110">Property</span></span>|<span data-ttu-id="32de8-111">类型</span><span class="sxs-lookup"><span data-stu-id="32de8-111">Type</span></span>|<span data-ttu-id="32de8-112">说明</span><span class="sxs-lookup"><span data-stu-id="32de8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32de8-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="32de8-113">startLayoutTileSize</span></span>|[<span data-ttu-id="32de8-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="32de8-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="32de8-115">开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。</span><span class="sxs-lookup"><span data-stu-id="32de8-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="32de8-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="32de8-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="32de8-117">name</span><span class="sxs-lookup"><span data-stu-id="32de8-117">name</span></span>|<span data-ttu-id="32de8-118">字符串</span><span class="sxs-lookup"><span data-stu-id="32de8-118">String</span></span>|<span data-ttu-id="32de8-119">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称</span><span class="sxs-lookup"><span data-stu-id="32de8-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="32de8-120">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="32de8-120">appUserModelId</span></span>|<span data-ttu-id="32de8-121">字符串</span><span class="sxs-lookup"><span data-stu-id="32de8-121">String</span></span>|<span data-ttu-id="32de8-122">这是仅应用程序用户模型 ID (AUMID) 将可用于启动在展台模式中使用</span><span class="sxs-lookup"><span data-stu-id="32de8-122">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="32de8-123">appId</span><span class="sxs-lookup"><span data-stu-id="32de8-123">appId</span></span>|<span data-ttu-id="32de8-124">String</span><span class="sxs-lookup"><span data-stu-id="32de8-124">String</span></span>|<span data-ttu-id="32de8-125">此引用 Intune 应用程序将作为网亭配置的同一个分配到的目标</span><span class="sxs-lookup"><span data-stu-id="32de8-125">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="32de8-126">containedAppId</span><span class="sxs-lookup"><span data-stu-id="32de8-126">containedAppId</span></span>|<span data-ttu-id="32de8-127">字符串</span><span class="sxs-lookup"><span data-stu-id="32de8-127">String</span></span>|<span data-ttu-id="32de8-128">此引用包含应用程序中 Intune 应用程序</span><span class="sxs-lookup"><span data-stu-id="32de8-128">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="32de8-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="32de8-129">Relationships</span></span>
<span data-ttu-id="32de8-130">无</span><span class="sxs-lookup"><span data-stu-id="32de8-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="32de8-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32de8-131">JSON Representation</span></span>
<span data-ttu-id="32de8-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32de8-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





