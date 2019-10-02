---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6024ba4d097c99a7abf501b89803dba13bcb096
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359073"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="be969-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="be969-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="be969-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be969-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be969-105">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="be969-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="be969-106">属性</span><span class="sxs-lookup"><span data-stu-id="be969-106">Properties</span></span>
|<span data-ttu-id="be969-107">属性</span><span class="sxs-lookup"><span data-stu-id="be969-107">Property</span></span>|<span data-ttu-id="be969-108">类型</span><span class="sxs-lookup"><span data-stu-id="be969-108">Type</span></span>|<span data-ttu-id="be969-109">说明</span><span class="sxs-lookup"><span data-stu-id="be969-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be969-110">displayName</span><span class="sxs-lookup"><span data-stu-id="be969-110">displayName</span></span>|<span data-ttu-id="be969-111">String</span><span class="sxs-lookup"><span data-stu-id="be969-111">String</span></span>|<span data-ttu-id="be969-112">页面的名称</span><span class="sxs-lookup"><span data-stu-id="be969-112">Name of the page</span></span>|
|<span data-ttu-id="be969-113">图标</span><span class="sxs-lookup"><span data-stu-id="be969-113">icons</span></span>|<span data-ttu-id="be969-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be969-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="be969-115">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="be969-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="be969-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="be969-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be969-117">关系</span><span class="sxs-lookup"><span data-stu-id="be969-117">Relationships</span></span>
<span data-ttu-id="be969-118">无</span><span class="sxs-lookup"><span data-stu-id="be969-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be969-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be969-119">JSON Representation</span></span>
<span data-ttu-id="be969-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be969-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
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
  ]
}
```




