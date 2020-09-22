---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d3f7dce03725a7ce30a24110efd1d47e0af5e371
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032458"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="6f27d-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f27d-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="6f27d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f27d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f27d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f27d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f27d-106">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="6f27d-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="6f27d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f27d-107">Properties</span></span>
|<span data-ttu-id="6f27d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f27d-108">Property</span></span>|<span data-ttu-id="6f27d-109">类型</span><span class="sxs-lookup"><span data-stu-id="6f27d-109">Type</span></span>|<span data-ttu-id="6f27d-110">说明</span><span class="sxs-lookup"><span data-stu-id="6f27d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f27d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6f27d-111">displayName</span></span>|<span data-ttu-id="6f27d-112">String</span><span class="sxs-lookup"><span data-stu-id="6f27d-112">String</span></span>|<span data-ttu-id="6f27d-113">页面的名称</span><span class="sxs-lookup"><span data-stu-id="6f27d-113">Name of the page</span></span>|
|<span data-ttu-id="6f27d-114">图标</span><span class="sxs-lookup"><span data-stu-id="6f27d-114">icons</span></span>|<span data-ttu-id="6f27d-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f27d-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="6f27d-116">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="6f27d-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="6f27d-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6f27d-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f27d-118">关系</span><span class="sxs-lookup"><span data-stu-id="6f27d-118">Relationships</span></span>
<span data-ttu-id="6f27d-119">无</span><span class="sxs-lookup"><span data-stu-id="6f27d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f27d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f27d-120">JSON Representation</span></span>
<span data-ttu-id="6f27d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f27d-121">Here is a JSON representation of the resource.</span></span>
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









