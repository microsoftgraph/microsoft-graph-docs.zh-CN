---
title: windowsKioskAppBase 资源类型
description: 一类应用程序的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 712c23e008e6c0b1434143383e4e8cd924ace509
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525528"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="81722-103">windowsKioskAppBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="81722-103">windowsKioskAppBase resource type</span></span>

<span data-ttu-id="81722-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="81722-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81722-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81722-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81722-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81722-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81722-107">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="81722-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="81722-108">属性</span><span class="sxs-lookup"><span data-stu-id="81722-108">Properties</span></span>
|<span data-ttu-id="81722-109">属性</span><span class="sxs-lookup"><span data-stu-id="81722-109">Property</span></span>|<span data-ttu-id="81722-110">类型</span><span class="sxs-lookup"><span data-stu-id="81722-110">Type</span></span>|<span data-ttu-id="81722-111">说明</span><span class="sxs-lookup"><span data-stu-id="81722-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81722-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="81722-112">startLayoutTileSize</span></span>|[<span data-ttu-id="81722-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="81722-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="81722-114">开始布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="81722-114">The app tile size for the start layout.</span></span> <span data-ttu-id="81722-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="81722-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="81722-116">name</span><span class="sxs-lookup"><span data-stu-id="81722-116">name</span></span>|<span data-ttu-id="81722-117">String</span><span class="sxs-lookup"><span data-stu-id="81722-117">String</span></span>|<span data-ttu-id="81722-118">表示应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="81722-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="81722-119">appType</span><span class="sxs-lookup"><span data-stu-id="81722-119">appType</span></span>|[<span data-ttu-id="81722-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="81722-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="81722-121">应用类型。</span><span class="sxs-lookup"><span data-stu-id="81722-121">The app type.</span></span> <span data-ttu-id="81722-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="81722-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="81722-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="81722-123">autoLaunch</span></span>|<span data-ttu-id="81722-124">布尔</span><span class="sxs-lookup"><span data-stu-id="81722-124">Boolean</span></span>|<span data-ttu-id="81722-125">允许在多应用展台模式下自动启动应用</span><span class="sxs-lookup"><span data-stu-id="81722-125">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="81722-126">关系</span><span class="sxs-lookup"><span data-stu-id="81722-126">Relationships</span></span>
<span data-ttu-id="81722-127">无</span><span class="sxs-lookup"><span data-stu-id="81722-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81722-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81722-128">JSON Representation</span></span>
<span data-ttu-id="81722-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81722-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```



