---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f06d15dce4ce765111ba02a200b59576a614828e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530680"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="97340-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="97340-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="97340-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97340-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97340-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97340-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97340-106">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="97340-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="97340-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="97340-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97340-108">属性</span><span class="sxs-lookup"><span data-stu-id="97340-108">Properties</span></span>
|<span data-ttu-id="97340-109">属性</span><span class="sxs-lookup"><span data-stu-id="97340-109">Property</span></span>|<span data-ttu-id="97340-110">类型</span><span class="sxs-lookup"><span data-stu-id="97340-110">Type</span></span>|<span data-ttu-id="97340-111">说明</span><span class="sxs-lookup"><span data-stu-id="97340-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97340-112">displayName</span><span class="sxs-lookup"><span data-stu-id="97340-112">displayName</span></span>|<span data-ttu-id="97340-113">String</span><span class="sxs-lookup"><span data-stu-id="97340-113">String</span></span>|<span data-ttu-id="97340-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="97340-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="97340-115">页面</span><span class="sxs-lookup"><span data-stu-id="97340-115">pages</span></span>|<span data-ttu-id="97340-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97340-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="97340-117">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="97340-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="97340-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="97340-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97340-119">关系</span><span class="sxs-lookup"><span data-stu-id="97340-119">Relationships</span></span>
<span data-ttu-id="97340-120">无</span><span class="sxs-lookup"><span data-stu-id="97340-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97340-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97340-121">JSON Representation</span></span>
<span data-ttu-id="97340-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97340-122">Here is a JSON representation of the resource.</span></span>
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




