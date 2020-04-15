---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fea1480b8b84a68d67a1bad499fa6c5b53841d35
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410589"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="c35cc-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="c35cc-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="c35cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c35cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c35cc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c35cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c35cc-106">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="c35cc-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="c35cc-107">属性</span><span class="sxs-lookup"><span data-stu-id="c35cc-107">Properties</span></span>
|<span data-ttu-id="c35cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="c35cc-108">Property</span></span>|<span data-ttu-id="c35cc-109">类型</span><span class="sxs-lookup"><span data-stu-id="c35cc-109">Type</span></span>|<span data-ttu-id="c35cc-110">说明</span><span class="sxs-lookup"><span data-stu-id="c35cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c35cc-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c35cc-111">displayName</span></span>|<span data-ttu-id="c35cc-112">String</span><span class="sxs-lookup"><span data-stu-id="c35cc-112">String</span></span>|<span data-ttu-id="c35cc-113">页面的名称</span><span class="sxs-lookup"><span data-stu-id="c35cc-113">Name of the page</span></span>|
|<span data-ttu-id="c35cc-114">图标</span><span class="sxs-lookup"><span data-stu-id="c35cc-114">icons</span></span>|<span data-ttu-id="c35cc-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c35cc-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="c35cc-116">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="c35cc-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="c35cc-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c35cc-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c35cc-118">关系</span><span class="sxs-lookup"><span data-stu-id="c35cc-118">Relationships</span></span>
<span data-ttu-id="c35cc-119">无</span><span class="sxs-lookup"><span data-stu-id="c35cc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c35cc-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c35cc-120">JSON Representation</span></span>
<span data-ttu-id="c35cc-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c35cc-121">Here is a JSON representation of the resource.</span></span>
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







