---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad2f9cb0f5530aeffbc840f2e7f38b5e0fde59a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526358"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="b4ede-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4ede-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="b4ede-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b4ede-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4ede-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4ede-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4ede-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4ede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4ede-107">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="b4ede-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="b4ede-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4ede-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4ede-109">属性</span><span class="sxs-lookup"><span data-stu-id="b4ede-109">Properties</span></span>
|<span data-ttu-id="b4ede-110">属性</span><span class="sxs-lookup"><span data-stu-id="b4ede-110">Property</span></span>|<span data-ttu-id="b4ede-111">类型</span><span class="sxs-lookup"><span data-stu-id="b4ede-111">Type</span></span>|<span data-ttu-id="b4ede-112">说明</span><span class="sxs-lookup"><span data-stu-id="b4ede-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4ede-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b4ede-113">displayName</span></span>|<span data-ttu-id="b4ede-114">String</span><span class="sxs-lookup"><span data-stu-id="b4ede-114">String</span></span>|<span data-ttu-id="b4ede-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="b4ede-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="b4ede-116">页面</span><span class="sxs-lookup"><span data-stu-id="b4ede-116">pages</span></span>|<span data-ttu-id="b4ede-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4ede-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="b4ede-118">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="b4ede-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="b4ede-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b4ede-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4ede-120">关系</span><span class="sxs-lookup"><span data-stu-id="b4ede-120">Relationships</span></span>
<span data-ttu-id="b4ede-121">无</span><span class="sxs-lookup"><span data-stu-id="b4ede-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4ede-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4ede-122">JSON Representation</span></span>
<span data-ttu-id="b4ede-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4ede-123">Here is a JSON representation of the resource.</span></span>
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



