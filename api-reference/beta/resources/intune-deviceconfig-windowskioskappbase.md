---
title: windowsKioskAppBase 资源类型
description: 一类应用程序的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4212dfd0362ed6253c10a2b2796241c74678dda2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736210"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="1720b-103">windowsKioskAppBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="1720b-103">windowsKioskAppBase resource type</span></span>

<span data-ttu-id="1720b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1720b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1720b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1720b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1720b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1720b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1720b-107">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="1720b-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="1720b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1720b-108">Properties</span></span>
|<span data-ttu-id="1720b-109">属性</span><span class="sxs-lookup"><span data-stu-id="1720b-109">Property</span></span>|<span data-ttu-id="1720b-110">类型</span><span class="sxs-lookup"><span data-stu-id="1720b-110">Type</span></span>|<span data-ttu-id="1720b-111">说明</span><span class="sxs-lookup"><span data-stu-id="1720b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1720b-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="1720b-112">startLayoutTileSize</span></span>|[<span data-ttu-id="1720b-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="1720b-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="1720b-114">开始布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="1720b-114">The app tile size for the start layout.</span></span> <span data-ttu-id="1720b-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="1720b-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="1720b-116">name</span><span class="sxs-lookup"><span data-stu-id="1720b-116">name</span></span>|<span data-ttu-id="1720b-117">String</span><span class="sxs-lookup"><span data-stu-id="1720b-117">String</span></span>|<span data-ttu-id="1720b-118">表示应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="1720b-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="1720b-119">appType</span><span class="sxs-lookup"><span data-stu-id="1720b-119">appType</span></span>|[<span data-ttu-id="1720b-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="1720b-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="1720b-121">应用类型。</span><span class="sxs-lookup"><span data-stu-id="1720b-121">The app type.</span></span> <span data-ttu-id="1720b-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="1720b-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="1720b-123">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="1720b-123">autoLaunch</span></span>|<span data-ttu-id="1720b-124">布尔</span><span class="sxs-lookup"><span data-stu-id="1720b-124">Boolean</span></span>|<span data-ttu-id="1720b-125">允许在多应用展台模式下自动启动应用</span><span class="sxs-lookup"><span data-stu-id="1720b-125">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="1720b-126">关系</span><span class="sxs-lookup"><span data-stu-id="1720b-126">Relationships</span></span>
<span data-ttu-id="1720b-127">无</span><span class="sxs-lookup"><span data-stu-id="1720b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1720b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1720b-128">JSON Representation</span></span>
<span data-ttu-id="1720b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1720b-129">Here is a JSON representation of the resource.</span></span>
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





