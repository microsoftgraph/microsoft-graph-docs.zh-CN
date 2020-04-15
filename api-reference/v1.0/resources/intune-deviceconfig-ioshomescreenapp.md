---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed97494144d6e8bb7e4154a84d0b4f2e7c01cf3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410713"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="058aa-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="058aa-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="058aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="058aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="058aa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="058aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="058aa-106">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="058aa-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="058aa-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="058aa-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="058aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="058aa-108">Properties</span></span>
|<span data-ttu-id="058aa-109">属性</span><span class="sxs-lookup"><span data-stu-id="058aa-109">Property</span></span>|<span data-ttu-id="058aa-110">类型</span><span class="sxs-lookup"><span data-stu-id="058aa-110">Type</span></span>|<span data-ttu-id="058aa-111">说明</span><span class="sxs-lookup"><span data-stu-id="058aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="058aa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="058aa-112">displayName</span></span>|<span data-ttu-id="058aa-113">String</span><span class="sxs-lookup"><span data-stu-id="058aa-113">String</span></span>|<span data-ttu-id="058aa-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="058aa-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="058aa-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="058aa-115">bundleID</span></span>|<span data-ttu-id="058aa-116">String</span><span class="sxs-lookup"><span data-stu-id="058aa-116">String</span></span>|<span data-ttu-id="058aa-117">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="058aa-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="058aa-118">关系</span><span class="sxs-lookup"><span data-stu-id="058aa-118">Relationships</span></span>
<span data-ttu-id="058aa-119">无</span><span class="sxs-lookup"><span data-stu-id="058aa-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="058aa-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="058aa-120">JSON Representation</span></span>
<span data-ttu-id="058aa-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="058aa-121">Here is a JSON representation of the resource.</span></span>
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







