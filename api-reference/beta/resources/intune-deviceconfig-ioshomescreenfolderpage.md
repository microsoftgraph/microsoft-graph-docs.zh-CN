---
title: iosHomeScreenFolderPage 资源类型
description: 主页上包含应用和 Web 剪辑的文件夹的页面。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45a26205e6a4f03639984e2a72632bb8bfb5a332
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161808"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="8eb46-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="8eb46-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="8eb46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eb46-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8eb46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eb46-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8eb46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb46-107">主页上包含应用和 Web 剪辑的文件夹的页面。</span><span class="sxs-lookup"><span data-stu-id="8eb46-107">A page for a folder containing apps and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="8eb46-108">属性</span><span class="sxs-lookup"><span data-stu-id="8eb46-108">Properties</span></span>
|<span data-ttu-id="8eb46-109">属性</span><span class="sxs-lookup"><span data-stu-id="8eb46-109">Property</span></span>|<span data-ttu-id="8eb46-110">类型</span><span class="sxs-lookup"><span data-stu-id="8eb46-110">Type</span></span>|<span data-ttu-id="8eb46-111">说明</span><span class="sxs-lookup"><span data-stu-id="8eb46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb46-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb46-112">displayName</span></span>|<span data-ttu-id="8eb46-113">String</span><span class="sxs-lookup"><span data-stu-id="8eb46-113">String</span></span>|<span data-ttu-id="8eb46-114">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="8eb46-114">Name of the folder page</span></span>|
|<span data-ttu-id="8eb46-115">应用</span><span class="sxs-lookup"><span data-stu-id="8eb46-115">apps</span></span>|<span data-ttu-id="8eb46-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8eb46-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="8eb46-117">要显示在文件夹内的页面上的应用和 Web 剪辑列表。</span><span class="sxs-lookup"><span data-stu-id="8eb46-117">A list of apps and web clips to appear on a page within a folder.</span></span> <span data-ttu-id="8eb46-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8eb46-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eb46-119">关系</span><span class="sxs-lookup"><span data-stu-id="8eb46-119">Relationships</span></span>
<span data-ttu-id="8eb46-120">无</span><span class="sxs-lookup"><span data-stu-id="8eb46-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eb46-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8eb46-121">JSON Representation</span></span>
<span data-ttu-id="8eb46-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8eb46-122">Here is a JSON representation of the resource.</span></span>
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
      "bundleID": "String",
      "isWebClip": true
    }
  ]
}
```




