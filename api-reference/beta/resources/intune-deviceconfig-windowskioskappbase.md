---
title: windowsKioskAppBase 资源类型
description: 一种类型的应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b13807fdb0319b3c9a15248fa2d50ffc46ac164
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977022"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="e9902-103">windowsKioskAppBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9902-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="e9902-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e9902-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9902-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e9902-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9902-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e9902-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9902-107">一种类型的应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="e9902-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="e9902-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9902-108">Properties</span></span>
|<span data-ttu-id="e9902-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9902-109">Property</span></span>|<span data-ttu-id="e9902-110">类型</span><span class="sxs-lookup"><span data-stu-id="e9902-110">Type</span></span>|<span data-ttu-id="e9902-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9902-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9902-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="e9902-112">startLayoutTileSize</span></span>|[<span data-ttu-id="e9902-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="e9902-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="e9902-114">开始版式应用程序图块大小。</span><span class="sxs-lookup"><span data-stu-id="e9902-114">The app tile size for the start layout.</span></span> <span data-ttu-id="e9902-115">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="e9902-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="e9902-116">name</span><span class="sxs-lookup"><span data-stu-id="e9902-116">name</span></span>|<span data-ttu-id="e9902-117">字符串</span><span class="sxs-lookup"><span data-stu-id="e9902-117">String</span></span>|<span data-ttu-id="e9902-118">代表应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="e9902-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9902-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="e9902-119">Relationships</span></span>
<span data-ttu-id="e9902-120">无</span><span class="sxs-lookup"><span data-stu-id="e9902-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9902-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9902-121">JSON Representation</span></span>
<span data-ttu-id="e9902-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9902-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





