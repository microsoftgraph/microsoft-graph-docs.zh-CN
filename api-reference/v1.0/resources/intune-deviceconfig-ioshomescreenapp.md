---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 55dacfcd7e16647c618d869fadc16d5b3c1cbc92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984465"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="c3ff7-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3ff7-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="c3ff7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3ff7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3ff7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3ff7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ff7-106">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="c3ff7-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="c3ff7-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c3ff7-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3ff7-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3ff7-108">Properties</span></span>
|<span data-ttu-id="c3ff7-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3ff7-109">Property</span></span>|<span data-ttu-id="c3ff7-110">类型</span><span class="sxs-lookup"><span data-stu-id="c3ff7-110">Type</span></span>|<span data-ttu-id="c3ff7-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3ff7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ff7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c3ff7-112">displayName</span></span>|<span data-ttu-id="c3ff7-113">String</span><span class="sxs-lookup"><span data-stu-id="c3ff7-113">String</span></span>|<span data-ttu-id="c3ff7-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="c3ff7-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c3ff7-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="c3ff7-115">bundleID</span></span>|<span data-ttu-id="c3ff7-116">String</span><span class="sxs-lookup"><span data-stu-id="c3ff7-116">String</span></span>|<span data-ttu-id="c3ff7-117">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="c3ff7-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3ff7-118">关系</span><span class="sxs-lookup"><span data-stu-id="c3ff7-118">Relationships</span></span>
<span data-ttu-id="c3ff7-119">无</span><span class="sxs-lookup"><span data-stu-id="c3ff7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3ff7-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3ff7-120">JSON Representation</span></span>
<span data-ttu-id="c3ff7-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3ff7-121">Here is a JSON representation of the resource.</span></span>
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









