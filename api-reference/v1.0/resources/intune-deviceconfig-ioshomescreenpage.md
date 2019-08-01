---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d898a1611c05b156ee4b16d042175b6b5c33284d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028173"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="1d703-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d703-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="1d703-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d703-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d703-105">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="1d703-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="1d703-106">属性</span><span class="sxs-lookup"><span data-stu-id="1d703-106">Properties</span></span>
|<span data-ttu-id="1d703-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d703-107">Property</span></span>|<span data-ttu-id="1d703-108">类型</span><span class="sxs-lookup"><span data-stu-id="1d703-108">Type</span></span>|<span data-ttu-id="1d703-109">说明</span><span class="sxs-lookup"><span data-stu-id="1d703-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d703-110">displayName</span><span class="sxs-lookup"><span data-stu-id="1d703-110">displayName</span></span>|<span data-ttu-id="1d703-111">String</span><span class="sxs-lookup"><span data-stu-id="1d703-111">String</span></span>|<span data-ttu-id="1d703-112">页面的名称</span><span class="sxs-lookup"><span data-stu-id="1d703-112">Name of the page</span></span>|
|<span data-ttu-id="1d703-113">图标</span><span class="sxs-lookup"><span data-stu-id="1d703-113">icons</span></span>|<span data-ttu-id="1d703-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d703-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="1d703-115">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="1d703-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="1d703-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1d703-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d703-117">关系</span><span class="sxs-lookup"><span data-stu-id="1d703-117">Relationships</span></span>
<span data-ttu-id="1d703-118">无</span><span class="sxs-lookup"><span data-stu-id="1d703-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d703-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d703-119">JSON Representation</span></span>
<span data-ttu-id="1d703-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d703-120">Here is a JSON representation of the resource.</span></span>
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



