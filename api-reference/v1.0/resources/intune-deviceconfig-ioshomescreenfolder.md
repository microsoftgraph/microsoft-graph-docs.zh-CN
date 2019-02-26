---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a44800da46d771251a47df676af84ceb778cbbd6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257685"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="96153-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="96153-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="96153-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96153-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96153-105">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="96153-105">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="96153-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="96153-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96153-107">属性</span><span class="sxs-lookup"><span data-stu-id="96153-107">Properties</span></span>
|<span data-ttu-id="96153-108">属性</span><span class="sxs-lookup"><span data-stu-id="96153-108">Property</span></span>|<span data-ttu-id="96153-109">类型</span><span class="sxs-lookup"><span data-stu-id="96153-109">Type</span></span>|<span data-ttu-id="96153-110">说明</span><span class="sxs-lookup"><span data-stu-id="96153-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96153-111">displayName</span><span class="sxs-lookup"><span data-stu-id="96153-111">displayName</span></span>|<span data-ttu-id="96153-112">String</span><span class="sxs-lookup"><span data-stu-id="96153-112">String</span></span>|<span data-ttu-id="96153-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="96153-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="96153-114">页面</span><span class="sxs-lookup"><span data-stu-id="96153-114">pages</span></span>|<span data-ttu-id="96153-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96153-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="96153-116">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="96153-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="96153-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="96153-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96153-118">关系</span><span class="sxs-lookup"><span data-stu-id="96153-118">Relationships</span></span>
<span data-ttu-id="96153-119">无</span><span class="sxs-lookup"><span data-stu-id="96153-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96153-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96153-120">JSON Representation</span></span>
<span data-ttu-id="96153-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96153-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```



