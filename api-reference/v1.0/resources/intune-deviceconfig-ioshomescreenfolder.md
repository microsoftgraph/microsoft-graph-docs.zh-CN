---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad796d334a3830b6bc5efac3ab1f29fe26cd2b04
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359119"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="4978c-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="4978c-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="4978c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4978c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4978c-105">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="4978c-105">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="4978c-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4978c-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4978c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4978c-107">Properties</span></span>
|<span data-ttu-id="4978c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4978c-108">Property</span></span>|<span data-ttu-id="4978c-109">类型</span><span class="sxs-lookup"><span data-stu-id="4978c-109">Type</span></span>|<span data-ttu-id="4978c-110">说明</span><span class="sxs-lookup"><span data-stu-id="4978c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4978c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4978c-111">displayName</span></span>|<span data-ttu-id="4978c-112">String</span><span class="sxs-lookup"><span data-stu-id="4978c-112">String</span></span>|<span data-ttu-id="4978c-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="4978c-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="4978c-114">页面</span><span class="sxs-lookup"><span data-stu-id="4978c-114">pages</span></span>|<span data-ttu-id="4978c-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4978c-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="4978c-116">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="4978c-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="4978c-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4978c-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4978c-118">关系</span><span class="sxs-lookup"><span data-stu-id="4978c-118">Relationships</span></span>
<span data-ttu-id="4978c-119">无</span><span class="sxs-lookup"><span data-stu-id="4978c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4978c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4978c-120">JSON Representation</span></span>
<span data-ttu-id="4978c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4978c-121">Here is a JSON representation of the resource.</span></span>
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




