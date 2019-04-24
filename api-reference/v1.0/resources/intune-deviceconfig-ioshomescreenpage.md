---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4317ac80e7ff6273b809eb747da745f5cf5edb6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464552"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="99be7-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="99be7-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="99be7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99be7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99be7-105">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="99be7-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="99be7-106">属性</span><span class="sxs-lookup"><span data-stu-id="99be7-106">Properties</span></span>
|<span data-ttu-id="99be7-107">属性</span><span class="sxs-lookup"><span data-stu-id="99be7-107">Property</span></span>|<span data-ttu-id="99be7-108">类型</span><span class="sxs-lookup"><span data-stu-id="99be7-108">Type</span></span>|<span data-ttu-id="99be7-109">说明</span><span class="sxs-lookup"><span data-stu-id="99be7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99be7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="99be7-110">displayName</span></span>|<span data-ttu-id="99be7-111">String</span><span class="sxs-lookup"><span data-stu-id="99be7-111">String</span></span>|<span data-ttu-id="99be7-112">页面的名称</span><span class="sxs-lookup"><span data-stu-id="99be7-112">Name of the page</span></span>|
|<span data-ttu-id="99be7-113">图标</span><span class="sxs-lookup"><span data-stu-id="99be7-113">icons</span></span>|<span data-ttu-id="99be7-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99be7-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="99be7-115">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="99be7-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="99be7-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="99be7-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99be7-117">关系</span><span class="sxs-lookup"><span data-stu-id="99be7-117">Relationships</span></span>
<span data-ttu-id="99be7-118">无</span><span class="sxs-lookup"><span data-stu-id="99be7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99be7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99be7-119">JSON Representation</span></span>
<span data-ttu-id="99be7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99be7-120">Here is a JSON representation of the resource.</span></span>
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



