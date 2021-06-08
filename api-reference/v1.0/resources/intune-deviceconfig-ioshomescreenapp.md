---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de16278256e9c6860a3cdead2ab5e940d0878a1a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760076"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="e8bdc-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8bdc-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="e8bdc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8bdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8bdc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8bdc-106">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="e8bdc-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="e8bdc-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8bdc-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8bdc-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8bdc-108">Properties</span></span>
|<span data-ttu-id="e8bdc-109">属性</span><span class="sxs-lookup"><span data-stu-id="e8bdc-109">Property</span></span>|<span data-ttu-id="e8bdc-110">类型</span><span class="sxs-lookup"><span data-stu-id="e8bdc-110">Type</span></span>|<span data-ttu-id="e8bdc-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8bdc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8bdc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e8bdc-112">displayName</span></span>|<span data-ttu-id="e8bdc-113">String</span><span class="sxs-lookup"><span data-stu-id="e8bdc-113">String</span></span>|<span data-ttu-id="e8bdc-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="e8bdc-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="e8bdc-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="e8bdc-115">bundleID</span></span>|<span data-ttu-id="e8bdc-116">String</span><span class="sxs-lookup"><span data-stu-id="e8bdc-116">String</span></span>|<span data-ttu-id="e8bdc-117">如果 isWebClip 为 false，则 BundleID 或 Web 剪辑的 URL（如果 isWebClip 为 true）。</span><span class="sxs-lookup"><span data-stu-id="e8bdc-117">BundleID of the app if isWebClip is false or the URL of a web clip if isWebClip is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8bdc-118">关系</span><span class="sxs-lookup"><span data-stu-id="e8bdc-118">Relationships</span></span>
<span data-ttu-id="e8bdc-119">无</span><span class="sxs-lookup"><span data-stu-id="e8bdc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8bdc-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8bdc-120">JSON Representation</span></span>
<span data-ttu-id="e8bdc-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8bdc-121">Here is a JSON representation of the resource.</span></span>
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




