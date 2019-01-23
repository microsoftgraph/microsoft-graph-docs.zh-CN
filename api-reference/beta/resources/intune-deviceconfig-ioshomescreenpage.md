---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b2b6e4ba9cc70253e929a0f434a292aeafd24bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398546"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="8696a-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="8696a-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="8696a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8696a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8696a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8696a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8696a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8696a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8696a-107">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="8696a-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="8696a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8696a-108">Properties</span></span>
|<span data-ttu-id="8696a-109">属性</span><span class="sxs-lookup"><span data-stu-id="8696a-109">Property</span></span>|<span data-ttu-id="8696a-110">类型</span><span class="sxs-lookup"><span data-stu-id="8696a-110">Type</span></span>|<span data-ttu-id="8696a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8696a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8696a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8696a-112">displayName</span></span>|<span data-ttu-id="8696a-113">String</span><span class="sxs-lookup"><span data-stu-id="8696a-113">String</span></span>|<span data-ttu-id="8696a-114">页面的名称</span><span class="sxs-lookup"><span data-stu-id="8696a-114">Name of the page</span></span>|
|<span data-ttu-id="8696a-115">图标</span><span class="sxs-lookup"><span data-stu-id="8696a-115">icons</span></span>|<span data-ttu-id="8696a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8696a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="8696a-117">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="8696a-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="8696a-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8696a-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8696a-119">关系</span><span class="sxs-lookup"><span data-stu-id="8696a-119">Relationships</span></span>
<span data-ttu-id="8696a-120">无</span><span class="sxs-lookup"><span data-stu-id="8696a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8696a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8696a-121">JSON Representation</span></span>
<span data-ttu-id="8696a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8696a-122">Here is a JSON representation of the resource.</span></span>
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




