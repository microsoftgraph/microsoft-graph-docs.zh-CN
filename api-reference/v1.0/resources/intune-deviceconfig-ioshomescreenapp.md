---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83b9c116f31a8f129394e618cf86e3382c1d528a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359116"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="c2dff-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2dff-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="c2dff-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2dff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2dff-105">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="c2dff-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="c2dff-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2dff-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2dff-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2dff-107">Properties</span></span>
|<span data-ttu-id="c2dff-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2dff-108">Property</span></span>|<span data-ttu-id="c2dff-109">类型</span><span class="sxs-lookup"><span data-stu-id="c2dff-109">Type</span></span>|<span data-ttu-id="c2dff-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2dff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2dff-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c2dff-111">displayName</span></span>|<span data-ttu-id="c2dff-112">String</span><span class="sxs-lookup"><span data-stu-id="c2dff-112">String</span></span>|<span data-ttu-id="c2dff-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="c2dff-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c2dff-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="c2dff-114">bundleID</span></span>|<span data-ttu-id="c2dff-115">String</span><span class="sxs-lookup"><span data-stu-id="c2dff-115">String</span></span>|<span data-ttu-id="c2dff-116">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="c2dff-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2dff-117">关系</span><span class="sxs-lookup"><span data-stu-id="c2dff-117">Relationships</span></span>
<span data-ttu-id="c2dff-118">无</span><span class="sxs-lookup"><span data-stu-id="c2dff-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2dff-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2dff-119">JSON Representation</span></span>
<span data-ttu-id="c2dff-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2dff-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```




