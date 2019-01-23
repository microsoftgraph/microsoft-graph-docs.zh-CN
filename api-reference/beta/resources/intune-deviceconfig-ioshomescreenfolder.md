---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 36ea4a00b9310623027179e1d6d2e1c64888c470
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407506"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="d4c04-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4c04-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="d4c04-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d4c04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4c04-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4c04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4c04-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4c04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c04-107">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="d4c04-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="d4c04-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d4c04-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4c04-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4c04-109">Properties</span></span>
|<span data-ttu-id="d4c04-110">属性</span><span class="sxs-lookup"><span data-stu-id="d4c04-110">Property</span></span>|<span data-ttu-id="d4c04-111">类型</span><span class="sxs-lookup"><span data-stu-id="d4c04-111">Type</span></span>|<span data-ttu-id="d4c04-112">说明</span><span class="sxs-lookup"><span data-stu-id="d4c04-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c04-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d4c04-113">displayName</span></span>|<span data-ttu-id="d4c04-114">String</span><span class="sxs-lookup"><span data-stu-id="d4c04-114">String</span></span>|<span data-ttu-id="d4c04-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="d4c04-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d4c04-116">页面</span><span class="sxs-lookup"><span data-stu-id="d4c04-116">pages</span></span>|<span data-ttu-id="d4c04-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4c04-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="d4c04-118">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="d4c04-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="d4c04-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d4c04-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4c04-120">关系</span><span class="sxs-lookup"><span data-stu-id="d4c04-120">Relationships</span></span>
<span data-ttu-id="d4c04-121">无</span><span class="sxs-lookup"><span data-stu-id="d4c04-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4c04-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4c04-122">JSON Representation</span></span>
<span data-ttu-id="d4c04-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4c04-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```




