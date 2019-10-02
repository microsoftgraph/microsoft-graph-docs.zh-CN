---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b80a4f41583617d32e514e29c791e000315593c5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359101"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="019d9-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="019d9-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="019d9-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="019d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="019d9-105">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="019d9-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="019d9-106">属性</span><span class="sxs-lookup"><span data-stu-id="019d9-106">Properties</span></span>
|<span data-ttu-id="019d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="019d9-107">Property</span></span>|<span data-ttu-id="019d9-108">类型</span><span class="sxs-lookup"><span data-stu-id="019d9-108">Type</span></span>|<span data-ttu-id="019d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="019d9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="019d9-110">displayName</span><span class="sxs-lookup"><span data-stu-id="019d9-110">displayName</span></span>|<span data-ttu-id="019d9-111">String</span><span class="sxs-lookup"><span data-stu-id="019d9-111">String</span></span>|<span data-ttu-id="019d9-112">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="019d9-112">Name of the folder page</span></span>|
|<span data-ttu-id="019d9-113">应用</span><span class="sxs-lookup"><span data-stu-id="019d9-113">apps</span></span>|<span data-ttu-id="019d9-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="019d9-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="019d9-115">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="019d9-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="019d9-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="019d9-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="019d9-117">关系</span><span class="sxs-lookup"><span data-stu-id="019d9-117">Relationships</span></span>
<span data-ttu-id="019d9-118">无</span><span class="sxs-lookup"><span data-stu-id="019d9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="019d9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="019d9-119">JSON Representation</span></span>
<span data-ttu-id="019d9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="019d9-120">Here is a JSON representation of the resource.</span></span>
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




