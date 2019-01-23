---
title: windowsKioskAppBase 资源类型
description: 一种类型的应用程序的基类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407142"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="4045f-103">windowsKioskAppBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="4045f-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="4045f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4045f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4045f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4045f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4045f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4045f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4045f-107">一种类型的应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="4045f-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="4045f-108">属性</span><span class="sxs-lookup"><span data-stu-id="4045f-108">Properties</span></span>
|<span data-ttu-id="4045f-109">属性</span><span class="sxs-lookup"><span data-stu-id="4045f-109">Property</span></span>|<span data-ttu-id="4045f-110">类型</span><span class="sxs-lookup"><span data-stu-id="4045f-110">Type</span></span>|<span data-ttu-id="4045f-111">说明</span><span class="sxs-lookup"><span data-stu-id="4045f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4045f-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="4045f-112">startLayoutTileSize</span></span>|[<span data-ttu-id="4045f-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="4045f-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="4045f-114">开始版式应用程序图块大小。</span><span class="sxs-lookup"><span data-stu-id="4045f-114">The app tile size for the start layout.</span></span> <span data-ttu-id="4045f-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="4045f-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="4045f-116">name</span><span class="sxs-lookup"><span data-stu-id="4045f-116">name</span></span>|<span data-ttu-id="4045f-117">String</span><span class="sxs-lookup"><span data-stu-id="4045f-117">String</span></span>|<span data-ttu-id="4045f-118">代表应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="4045f-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="4045f-119">appType</span><span class="sxs-lookup"><span data-stu-id="4045f-119">appType</span></span>|[<span data-ttu-id="4045f-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="4045f-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="4045f-121">该应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="4045f-121">The app type.</span></span> <span data-ttu-id="4045f-122">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="4045f-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4045f-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="4045f-123">Relationships</span></span>
<span data-ttu-id="4045f-124">无</span><span class="sxs-lookup"><span data-stu-id="4045f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4045f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4045f-125">JSON Representation</span></span>
<span data-ttu-id="4045f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4045f-126">Here is a JSON representation of the resource.</span></span>
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
  "appType": "String"
}
```




