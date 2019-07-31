---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e7231cd67291cfadd7fb3cec114c31e7af246c49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004244"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="cc644-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc644-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="cc644-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc644-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc644-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc644-106">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="cc644-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="cc644-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="cc644-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc644-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc644-108">Properties</span></span>
|<span data-ttu-id="cc644-109">属性</span><span class="sxs-lookup"><span data-stu-id="cc644-109">Property</span></span>|<span data-ttu-id="cc644-110">类型</span><span class="sxs-lookup"><span data-stu-id="cc644-110">Type</span></span>|<span data-ttu-id="cc644-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc644-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc644-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cc644-112">displayName</span></span>|<span data-ttu-id="cc644-113">String</span><span class="sxs-lookup"><span data-stu-id="cc644-113">String</span></span>|<span data-ttu-id="cc644-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="cc644-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="cc644-115">页面</span><span class="sxs-lookup"><span data-stu-id="cc644-115">pages</span></span>|<span data-ttu-id="cc644-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc644-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="cc644-117">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="cc644-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="cc644-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="cc644-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc644-119">关系</span><span class="sxs-lookup"><span data-stu-id="cc644-119">Relationships</span></span>
<span data-ttu-id="cc644-120">无</span><span class="sxs-lookup"><span data-stu-id="cc644-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc644-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc644-121">JSON Representation</span></span>
<span data-ttu-id="cc644-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc644-122">Here is a JSON representation of the resource.</span></span>
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





