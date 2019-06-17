---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a3ce2a6ac9cacffb2dc5ac2cc4ad3c5fced14d2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978218"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="c2c6e-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2c6e-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="c2c6e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2c6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2c6e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2c6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2c6e-106">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="c2c6e-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="c2c6e-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2c6e-107">Properties</span></span>
|<span data-ttu-id="c2c6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2c6e-108">Property</span></span>|<span data-ttu-id="c2c6e-109">类型</span><span class="sxs-lookup"><span data-stu-id="c2c6e-109">Type</span></span>|<span data-ttu-id="c2c6e-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2c6e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c6e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c2c6e-111">displayName</span></span>|<span data-ttu-id="c2c6e-112">String</span><span class="sxs-lookup"><span data-stu-id="c2c6e-112">String</span></span>|<span data-ttu-id="c2c6e-113">页面的名称</span><span class="sxs-lookup"><span data-stu-id="c2c6e-113">Name of the page</span></span>|
|<span data-ttu-id="c2c6e-114">图标</span><span class="sxs-lookup"><span data-stu-id="c2c6e-114">icons</span></span>|<span data-ttu-id="c2c6e-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2c6e-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="c2c6e-116">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="c2c6e-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="c2c6e-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2c6e-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2c6e-118">关系</span><span class="sxs-lookup"><span data-stu-id="c2c6e-118">Relationships</span></span>
<span data-ttu-id="c2c6e-119">无</span><span class="sxs-lookup"><span data-stu-id="c2c6e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2c6e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2c6e-120">JSON Representation</span></span>
<span data-ttu-id="c2c6e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2c6e-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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





