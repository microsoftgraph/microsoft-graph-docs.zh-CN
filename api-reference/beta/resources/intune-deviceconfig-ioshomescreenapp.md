---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 24c21b6260800250daa768df0684298f3bb142ae
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161822"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="0ee19-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ee19-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="0ee19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ee19-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ee19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee19-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ee19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee19-107">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="0ee19-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="0ee19-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ee19-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ee19-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ee19-109">Properties</span></span>
|<span data-ttu-id="0ee19-110">属性</span><span class="sxs-lookup"><span data-stu-id="0ee19-110">Property</span></span>|<span data-ttu-id="0ee19-111">类型</span><span class="sxs-lookup"><span data-stu-id="0ee19-111">Type</span></span>|<span data-ttu-id="0ee19-112">说明</span><span class="sxs-lookup"><span data-stu-id="0ee19-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee19-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee19-113">displayName</span></span>|<span data-ttu-id="0ee19-114">String</span><span class="sxs-lookup"><span data-stu-id="0ee19-114">String</span></span>|<span data-ttu-id="0ee19-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="0ee19-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="0ee19-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="0ee19-116">bundleID</span></span>|<span data-ttu-id="0ee19-117">String</span><span class="sxs-lookup"><span data-stu-id="0ee19-117">String</span></span>|<span data-ttu-id="0ee19-118">如果 isWebClip 为 false 或 Web 剪辑的 URL（如果 isWebClip 为 true，则应用 BundleID）。</span><span class="sxs-lookup"><span data-stu-id="0ee19-118">BundleID of the app if isWebClip is false or the URL of a web clip if isWebClip is true.</span></span>|
|<span data-ttu-id="0ee19-119">isWebClip</span><span class="sxs-lookup"><span data-stu-id="0ee19-119">isWebClip</span></span>|<span data-ttu-id="0ee19-120">布尔</span><span class="sxs-lookup"><span data-stu-id="0ee19-120">Boolean</span></span>|<span data-ttu-id="0ee19-121">如果为 true，捆绑包 ID 将处理为 Web 剪辑的 URL。</span><span class="sxs-lookup"><span data-stu-id="0ee19-121">When true, the bundle ID will be handled as a URL for a web clip.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ee19-122">关系</span><span class="sxs-lookup"><span data-stu-id="0ee19-122">Relationships</span></span>
<span data-ttu-id="0ee19-123">无</span><span class="sxs-lookup"><span data-stu-id="0ee19-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ee19-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ee19-124">JSON Representation</span></span>
<span data-ttu-id="0ee19-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee19-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String",
  "isWebClip": true
}
```




