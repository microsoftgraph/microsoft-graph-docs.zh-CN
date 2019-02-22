---
title: windowsKioskAppBase 资源类型
description: 一类应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0247febfbeebe7fc047df4bb14a9d421b79bf01
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145295"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="3c850-103">windowsKioskAppBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c850-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="3c850-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c850-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c850-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c850-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c850-106">一类应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="3c850-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="3c850-107">属性</span><span class="sxs-lookup"><span data-stu-id="3c850-107">Properties</span></span>
|<span data-ttu-id="3c850-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c850-108">Property</span></span>|<span data-ttu-id="3c850-109">类型</span><span class="sxs-lookup"><span data-stu-id="3c850-109">Type</span></span>|<span data-ttu-id="3c850-110">说明</span><span class="sxs-lookup"><span data-stu-id="3c850-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c850-111">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="3c850-111">startLayoutTileSize</span></span>|[<span data-ttu-id="3c850-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="3c850-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="3c850-113">开始布局的应用程序磁贴大小。</span><span class="sxs-lookup"><span data-stu-id="3c850-113">The app tile size for the start layout.</span></span> <span data-ttu-id="3c850-114">可取值为：`hidden`、`small`、`medium`、`wide`、`large`。</span><span class="sxs-lookup"><span data-stu-id="3c850-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="3c850-115">name</span><span class="sxs-lookup"><span data-stu-id="3c850-115">name</span></span>|<span data-ttu-id="3c850-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3c850-116">String</span></span>|<span data-ttu-id="3c850-117">表示应用程序的友好名称</span><span class="sxs-lookup"><span data-stu-id="3c850-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="3c850-118">appType</span><span class="sxs-lookup"><span data-stu-id="3c850-118">appType</span></span>|[<span data-ttu-id="3c850-119">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="3c850-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="3c850-120">应用类型。</span><span class="sxs-lookup"><span data-stu-id="3c850-120">The app type.</span></span> <span data-ttu-id="3c850-121">可取值为：`unknown`、`store`、`desktop`、`aumId`。</span><span class="sxs-lookup"><span data-stu-id="3c850-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c850-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="3c850-122">Relationships</span></span>
<span data-ttu-id="3c850-123">无</span><span class="sxs-lookup"><span data-stu-id="3c850-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c850-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c850-124">JSON Representation</span></span>
<span data-ttu-id="3c850-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c850-125">Here is a JSON representation of the resource.</span></span>
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




