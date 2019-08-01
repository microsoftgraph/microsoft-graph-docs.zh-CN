---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76a8237442e0e807e0a1383c8032cf4e6361516e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028208"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="2b7c0-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b7c0-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="2b7c0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b7c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7c0-105">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="2b7c0-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="2b7c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b7c0-106">Properties</span></span>
|<span data-ttu-id="2b7c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b7c0-107">Property</span></span>|<span data-ttu-id="2b7c0-108">类型</span><span class="sxs-lookup"><span data-stu-id="2b7c0-108">Type</span></span>|<span data-ttu-id="2b7c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b7c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b7c0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2b7c0-110">displayName</span></span>|<span data-ttu-id="2b7c0-111">String</span><span class="sxs-lookup"><span data-stu-id="2b7c0-111">String</span></span>|<span data-ttu-id="2b7c0-112">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="2b7c0-112">Name of the folder page</span></span>|
|<span data-ttu-id="2b7c0-113">应用</span><span class="sxs-lookup"><span data-stu-id="2b7c0-113">apps</span></span>|<span data-ttu-id="2b7c0-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b7c0-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="2b7c0-115">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="2b7c0-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="2b7c0-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2b7c0-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b7c0-117">关系</span><span class="sxs-lookup"><span data-stu-id="2b7c0-117">Relationships</span></span>
<span data-ttu-id="2b7c0-118">无</span><span class="sxs-lookup"><span data-stu-id="2b7c0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b7c0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b7c0-119">JSON Representation</span></span>
<span data-ttu-id="2b7c0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b7c0-120">Here is a JSON representation of the resource.</span></span>
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



