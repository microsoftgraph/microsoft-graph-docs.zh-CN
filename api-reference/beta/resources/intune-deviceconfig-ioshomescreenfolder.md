---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4571baad6e1e0967b8b38ced9b96fd977f154fd7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280422"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="36125-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="36125-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="36125-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36125-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36125-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36125-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36125-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36125-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36125-107">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="36125-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="36125-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="36125-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36125-109">属性</span><span class="sxs-lookup"><span data-stu-id="36125-109">Properties</span></span>
|<span data-ttu-id="36125-110">属性</span><span class="sxs-lookup"><span data-stu-id="36125-110">Property</span></span>|<span data-ttu-id="36125-111">类型</span><span class="sxs-lookup"><span data-stu-id="36125-111">Type</span></span>|<span data-ttu-id="36125-112">说明</span><span class="sxs-lookup"><span data-stu-id="36125-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36125-113">displayName</span><span class="sxs-lookup"><span data-stu-id="36125-113">displayName</span></span>|<span data-ttu-id="36125-114">字符串</span><span class="sxs-lookup"><span data-stu-id="36125-114">String</span></span>|<span data-ttu-id="36125-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="36125-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="36125-116">页面</span><span class="sxs-lookup"><span data-stu-id="36125-116">pages</span></span>|<span data-ttu-id="36125-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36125-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="36125-118">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="36125-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="36125-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="36125-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36125-120">关系</span><span class="sxs-lookup"><span data-stu-id="36125-120">Relationships</span></span>
<span data-ttu-id="36125-121">无</span><span class="sxs-lookup"><span data-stu-id="36125-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36125-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36125-122">JSON Representation</span></span>
<span data-ttu-id="36125-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36125-123">Here is a JSON representation of the resource.</span></span>
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




