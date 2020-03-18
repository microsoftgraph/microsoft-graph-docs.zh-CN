---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93fca952cfda7bf1e49c17a3fe71b3a62384d0e6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791574"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="6c984-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c984-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="6c984-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c984-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c984-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c984-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c984-106">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="6c984-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="6c984-107">属性</span><span class="sxs-lookup"><span data-stu-id="6c984-107">Properties</span></span>
|<span data-ttu-id="6c984-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c984-108">Property</span></span>|<span data-ttu-id="6c984-109">类型</span><span class="sxs-lookup"><span data-stu-id="6c984-109">Type</span></span>|<span data-ttu-id="6c984-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c984-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c984-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6c984-111">displayName</span></span>|<span data-ttu-id="6c984-112">String</span><span class="sxs-lookup"><span data-stu-id="6c984-112">String</span></span>|<span data-ttu-id="6c984-113">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="6c984-113">Name of the folder page</span></span>|
|<span data-ttu-id="6c984-114">应用</span><span class="sxs-lookup"><span data-stu-id="6c984-114">apps</span></span>|<span data-ttu-id="6c984-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c984-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="6c984-116">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="6c984-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="6c984-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c984-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c984-118">关系</span><span class="sxs-lookup"><span data-stu-id="6c984-118">Relationships</span></span>
<span data-ttu-id="6c984-119">无</span><span class="sxs-lookup"><span data-stu-id="6c984-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c984-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c984-120">JSON Representation</span></span>
<span data-ttu-id="6c984-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c984-121">Here is a JSON representation of the resource.</span></span>
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



