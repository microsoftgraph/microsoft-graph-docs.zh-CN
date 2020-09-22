---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e60e0365656a9b1dee0bb78022edeaeef7e5e6f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984430"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="7829f-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="7829f-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="7829f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7829f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7829f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7829f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7829f-106">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="7829f-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="7829f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7829f-107">Properties</span></span>
|<span data-ttu-id="7829f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7829f-108">Property</span></span>|<span data-ttu-id="7829f-109">类型</span><span class="sxs-lookup"><span data-stu-id="7829f-109">Type</span></span>|<span data-ttu-id="7829f-110">说明</span><span class="sxs-lookup"><span data-stu-id="7829f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7829f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7829f-111">displayName</span></span>|<span data-ttu-id="7829f-112">String</span><span class="sxs-lookup"><span data-stu-id="7829f-112">String</span></span>|<span data-ttu-id="7829f-113">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="7829f-113">Name of the folder page</span></span>|
|<span data-ttu-id="7829f-114">应用</span><span class="sxs-lookup"><span data-stu-id="7829f-114">apps</span></span>|<span data-ttu-id="7829f-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7829f-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="7829f-116">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="7829f-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="7829f-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="7829f-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7829f-118">关系</span><span class="sxs-lookup"><span data-stu-id="7829f-118">Relationships</span></span>
<span data-ttu-id="7829f-119">无</span><span class="sxs-lookup"><span data-stu-id="7829f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7829f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7829f-120">JSON Representation</span></span>
<span data-ttu-id="7829f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7829f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```









