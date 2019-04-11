---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8d1765cbad7f904c994aac1872f40231fc525c8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797513"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="996e6-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="996e6-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="996e6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="996e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="996e6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="996e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="996e6-106">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="996e6-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="996e6-107">属性</span><span class="sxs-lookup"><span data-stu-id="996e6-107">Properties</span></span>
|<span data-ttu-id="996e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="996e6-108">Property</span></span>|<span data-ttu-id="996e6-109">类型</span><span class="sxs-lookup"><span data-stu-id="996e6-109">Type</span></span>|<span data-ttu-id="996e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="996e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="996e6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="996e6-111">displayName</span></span>|<span data-ttu-id="996e6-112">String</span><span class="sxs-lookup"><span data-stu-id="996e6-112">String</span></span>|<span data-ttu-id="996e6-113">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="996e6-113">Name of the folder page</span></span>|
|<span data-ttu-id="996e6-114">应用</span><span class="sxs-lookup"><span data-stu-id="996e6-114">apps</span></span>|<span data-ttu-id="996e6-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="996e6-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="996e6-116">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="996e6-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="996e6-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="996e6-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="996e6-118">关系</span><span class="sxs-lookup"><span data-stu-id="996e6-118">Relationships</span></span>
<span data-ttu-id="996e6-119">无</span><span class="sxs-lookup"><span data-stu-id="996e6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="996e6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="996e6-120">JSON Representation</span></span>
<span data-ttu-id="996e6-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="996e6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```





