---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1a4f7f4180bce05d331fcc116826956f4feed70c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844574"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="71d85-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="71d85-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="71d85-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="71d85-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71d85-105">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="71d85-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="71d85-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="71d85-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71d85-107">属性</span><span class="sxs-lookup"><span data-stu-id="71d85-107">Properties</span></span>
|<span data-ttu-id="71d85-108">属性</span><span class="sxs-lookup"><span data-stu-id="71d85-108">Property</span></span>|<span data-ttu-id="71d85-109">类型</span><span class="sxs-lookup"><span data-stu-id="71d85-109">Type</span></span>|<span data-ttu-id="71d85-110">说明</span><span class="sxs-lookup"><span data-stu-id="71d85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d85-111">displayName</span><span class="sxs-lookup"><span data-stu-id="71d85-111">displayName</span></span>|<span data-ttu-id="71d85-112">String</span><span class="sxs-lookup"><span data-stu-id="71d85-112">String</span></span>|<span data-ttu-id="71d85-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="71d85-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="71d85-114">页面</span><span class="sxs-lookup"><span data-stu-id="71d85-114">pages</span></span>|<span data-ttu-id="71d85-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71d85-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="71d85-116">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="71d85-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="71d85-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="71d85-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71d85-118">关系</span><span class="sxs-lookup"><span data-stu-id="71d85-118">Relationships</span></span>
<span data-ttu-id="71d85-119">无</span><span class="sxs-lookup"><span data-stu-id="71d85-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71d85-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71d85-120">JSON Representation</span></span>
<span data-ttu-id="71d85-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71d85-121">Here is a JSON representation of the resource.</span></span>
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



