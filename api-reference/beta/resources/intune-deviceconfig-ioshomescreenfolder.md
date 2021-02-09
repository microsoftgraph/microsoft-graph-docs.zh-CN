---
title: iosHomeScreenFolder 资源类型
description: 一个包含主屏幕上应用页面和 Web 剪辑的文件夹。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ad090d7e5a01eaf3dda10c6d9edd5cfafacb1a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161815"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="3a98f-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a98f-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="3a98f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a98f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a98f-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a98f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a98f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a98f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a98f-107">一个包含主屏幕上应用页面和 Web 剪辑的文件夹。</span><span class="sxs-lookup"><span data-stu-id="3a98f-107">A folder containing pages of apps and web clips on the Home Screen.</span></span>


<span data-ttu-id="3a98f-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="3a98f-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a98f-109">属性</span><span class="sxs-lookup"><span data-stu-id="3a98f-109">Properties</span></span>
|<span data-ttu-id="3a98f-110">属性</span><span class="sxs-lookup"><span data-stu-id="3a98f-110">Property</span></span>|<span data-ttu-id="3a98f-111">类型</span><span class="sxs-lookup"><span data-stu-id="3a98f-111">Type</span></span>|<span data-ttu-id="3a98f-112">说明</span><span class="sxs-lookup"><span data-stu-id="3a98f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a98f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="3a98f-113">displayName</span></span>|<span data-ttu-id="3a98f-114">String</span><span class="sxs-lookup"><span data-stu-id="3a98f-114">String</span></span>|<span data-ttu-id="3a98f-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="3a98f-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="3a98f-116">页面</span><span class="sxs-lookup"><span data-stu-id="3a98f-116">pages</span></span>|<span data-ttu-id="3a98f-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3a98f-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="3a98f-118">必须是应用程序或 Web 剪辑的主屏幕布局图标的页面。</span><span class="sxs-lookup"><span data-stu-id="3a98f-118">Pages of Home Screen Layout Icons which must be applications or web clips.</span></span> <span data-ttu-id="3a98f-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3a98f-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a98f-120">关系</span><span class="sxs-lookup"><span data-stu-id="3a98f-120">Relationships</span></span>
<span data-ttu-id="3a98f-121">无</span><span class="sxs-lookup"><span data-stu-id="3a98f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a98f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a98f-122">JSON Representation</span></span>
<span data-ttu-id="3a98f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a98f-123">Here is a JSON representation of the resource.</span></span>
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
          "bundleID": "String",
          "isWebClip": true
        }
      ]
    }
  ]
}
```




