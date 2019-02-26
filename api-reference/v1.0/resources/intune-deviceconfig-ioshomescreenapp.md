---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260933"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="8bca0-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bca0-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="8bca0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8bca0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bca0-105">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="8bca0-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="8bca0-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8bca0-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8bca0-107">属性</span><span class="sxs-lookup"><span data-stu-id="8bca0-107">Properties</span></span>
|<span data-ttu-id="8bca0-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bca0-108">Property</span></span>|<span data-ttu-id="8bca0-109">类型</span><span class="sxs-lookup"><span data-stu-id="8bca0-109">Type</span></span>|<span data-ttu-id="8bca0-110">说明</span><span class="sxs-lookup"><span data-stu-id="8bca0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bca0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8bca0-111">displayName</span></span>|<span data-ttu-id="8bca0-112">String</span><span class="sxs-lookup"><span data-stu-id="8bca0-112">String</span></span>|<span data-ttu-id="8bca0-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="8bca0-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="8bca0-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="8bca0-114">bundleID</span></span>|<span data-ttu-id="8bca0-115">String</span><span class="sxs-lookup"><span data-stu-id="8bca0-115">String</span></span>|<span data-ttu-id="8bca0-116">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="8bca0-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bca0-117">关系</span><span class="sxs-lookup"><span data-stu-id="8bca0-117">Relationships</span></span>
<span data-ttu-id="8bca0-118">无</span><span class="sxs-lookup"><span data-stu-id="8bca0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bca0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bca0-119">JSON Representation</span></span>
<span data-ttu-id="8bca0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bca0-120">Here is a JSON representation of the resource.</span></span>
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



