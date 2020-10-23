---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f62ae053018865aca7b0794bbcbc501ece675c22
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705797"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="bee0e-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="bee0e-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="bee0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bee0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bee0e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bee0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bee0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bee0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bee0e-107">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="bee0e-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="bee0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="bee0e-108">Properties</span></span>
|<span data-ttu-id="bee0e-109">属性</span><span class="sxs-lookup"><span data-stu-id="bee0e-109">Property</span></span>|<span data-ttu-id="bee0e-110">类型</span><span class="sxs-lookup"><span data-stu-id="bee0e-110">Type</span></span>|<span data-ttu-id="bee0e-111">说明</span><span class="sxs-lookup"><span data-stu-id="bee0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee0e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bee0e-112">displayName</span></span>|<span data-ttu-id="bee0e-113">String</span><span class="sxs-lookup"><span data-stu-id="bee0e-113">String</span></span>|<span data-ttu-id="bee0e-114">页面的名称</span><span class="sxs-lookup"><span data-stu-id="bee0e-114">Name of the page</span></span>|
|<span data-ttu-id="bee0e-115">图标</span><span class="sxs-lookup"><span data-stu-id="bee0e-115">icons</span></span>|<span data-ttu-id="bee0e-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bee0e-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="bee0e-117">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="bee0e-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="bee0e-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bee0e-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bee0e-119">关系</span><span class="sxs-lookup"><span data-stu-id="bee0e-119">Relationships</span></span>
<span data-ttu-id="bee0e-120">无</span><span class="sxs-lookup"><span data-stu-id="bee0e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bee0e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bee0e-121">JSON Representation</span></span>
<span data-ttu-id="bee0e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bee0e-122">Here is a JSON representation of the resource.</span></span>
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





