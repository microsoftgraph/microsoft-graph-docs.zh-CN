---
title: windowsKioskDesktopApp 资源类型
description: 一种类型的应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53eb615dcd1ba2b88c6cdd4bb5a1b76b83b67eaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830973"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="58ea3-103">windowsKioskDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="58ea3-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="58ea3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="58ea3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58ea3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="58ea3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58ea3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="58ea3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58ea3-107">一种类型的应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="58ea3-107">The base class for a type of apps</span></span>

<span data-ttu-id="58ea3-108">继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="58ea3-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58ea3-109">属性</span><span class="sxs-lookup"><span data-stu-id="58ea3-109">Properties</span></span>
|<span data-ttu-id="58ea3-110">属性</span><span class="sxs-lookup"><span data-stu-id="58ea3-110">Property</span></span>|<span data-ttu-id="58ea3-111">类型</span><span class="sxs-lookup"><span data-stu-id="58ea3-111">Type</span></span>|<span data-ttu-id="58ea3-112">Description</span><span class="sxs-lookup"><span data-stu-id="58ea3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58ea3-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="58ea3-113">startLayoutTileSize</span></span>|[<span data-ttu-id="58ea3-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="58ea3-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="58ea3-115">开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。</span><span class="sxs-lookup"><span data-stu-id="58ea3-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="58ea3-116">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="58ea3-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="58ea3-117">name</span><span class="sxs-lookup"><span data-stu-id="58ea3-117">name</span></span>|<span data-ttu-id="58ea3-118">字符串</span><span class="sxs-lookup"><span data-stu-id="58ea3-118">String</span></span>|<span data-ttu-id="58ea3-119">从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称</span><span class="sxs-lookup"><span data-stu-id="58ea3-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="58ea3-120">路径</span><span class="sxs-lookup"><span data-stu-id="58ea3-120">path</span></span>|<span data-ttu-id="58ea3-121">字符串</span><span class="sxs-lookup"><span data-stu-id="58ea3-121">String</span></span>|<span data-ttu-id="58ea3-122">定义桌面应用程序的路径</span><span class="sxs-lookup"><span data-stu-id="58ea3-122">Define the path of a desktop app</span></span>|
|<span data-ttu-id="58ea3-123">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="58ea3-123">desktopApplicationId</span></span>|<span data-ttu-id="58ea3-124">字符串</span><span class="sxs-lookup"><span data-stu-id="58ea3-124">String</span></span>|<span data-ttu-id="58ea3-125">定义应用程序的 DesktopApplicationID</span><span class="sxs-lookup"><span data-stu-id="58ea3-125">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="58ea3-126">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="58ea3-126">desktopApplicationLinkPath</span></span>|<span data-ttu-id="58ea3-127">字符串</span><span class="sxs-lookup"><span data-stu-id="58ea3-127">String</span></span>|<span data-ttu-id="58ea3-128">定义应用程序的 DesktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="58ea3-128">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="58ea3-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="58ea3-129">Relationships</span></span>
<span data-ttu-id="58ea3-130">无</span><span class="sxs-lookup"><span data-stu-id="58ea3-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58ea3-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58ea3-131">JSON Representation</span></span>
<span data-ttu-id="58ea3-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58ea3-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





