---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f18061e8bc8c974eab443d389b94be80134924f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993908"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="2b2f5-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b2f5-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="2b2f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b2f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b2f5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b2f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b2f5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b2f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b2f5-107">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="2b2f5-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="2b2f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b2f5-108">Properties</span></span>
|<span data-ttu-id="2b2f5-109">属性</span><span class="sxs-lookup"><span data-stu-id="2b2f5-109">Property</span></span>|<span data-ttu-id="2b2f5-110">类型</span><span class="sxs-lookup"><span data-stu-id="2b2f5-110">Type</span></span>|<span data-ttu-id="2b2f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b2f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b2f5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2b2f5-112">displayName</span></span>|<span data-ttu-id="2b2f5-113">String</span><span class="sxs-lookup"><span data-stu-id="2b2f5-113">String</span></span>|<span data-ttu-id="2b2f5-114">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="2b2f5-114">Name of the folder page</span></span>|
|<span data-ttu-id="2b2f5-115">应用</span><span class="sxs-lookup"><span data-stu-id="2b2f5-115">apps</span></span>|<span data-ttu-id="2b2f5-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b2f5-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="2b2f5-117">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="2b2f5-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="2b2f5-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2b2f5-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b2f5-119">关系</span><span class="sxs-lookup"><span data-stu-id="2b2f5-119">Relationships</span></span>
<span data-ttu-id="2b2f5-120">无</span><span class="sxs-lookup"><span data-stu-id="2b2f5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b2f5-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b2f5-121">JSON Representation</span></span>
<span data-ttu-id="2b2f5-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b2f5-122">Here is a JSON representation of the resource.</span></span>
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






