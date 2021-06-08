---
title: iosHomeScreenFolderPage 资源类型
description: 主页上包含应用和 Web 剪辑的文件夹的页面。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a8fc93d365dc842886f3346b86ff632f3ced7cb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760062"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="b0d76-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0d76-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="b0d76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0d76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0d76-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0d76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0d76-106">主页上包含应用和 Web 剪辑的文件夹的页面。</span><span class="sxs-lookup"><span data-stu-id="b0d76-106">A page for a folder containing apps and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="b0d76-107">属性</span><span class="sxs-lookup"><span data-stu-id="b0d76-107">Properties</span></span>
|<span data-ttu-id="b0d76-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0d76-108">Property</span></span>|<span data-ttu-id="b0d76-109">类型</span><span class="sxs-lookup"><span data-stu-id="b0d76-109">Type</span></span>|<span data-ttu-id="b0d76-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0d76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0d76-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b0d76-111">displayName</span></span>|<span data-ttu-id="b0d76-112">String</span><span class="sxs-lookup"><span data-stu-id="b0d76-112">String</span></span>|<span data-ttu-id="b0d76-113">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="b0d76-113">Name of the folder page</span></span>|
|<span data-ttu-id="b0d76-114">应用</span><span class="sxs-lookup"><span data-stu-id="b0d76-114">apps</span></span>|<span data-ttu-id="b0d76-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0d76-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="b0d76-116">要显示在文件夹内的页面上的应用和 Web 剪辑列表。</span><span class="sxs-lookup"><span data-stu-id="b0d76-116">A list of apps and web clips to appear on a page within a folder.</span></span> <span data-ttu-id="b0d76-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b0d76-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0d76-118">关系</span><span class="sxs-lookup"><span data-stu-id="b0d76-118">Relationships</span></span>
<span data-ttu-id="b0d76-119">无</span><span class="sxs-lookup"><span data-stu-id="b0d76-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0d76-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0d76-120">JSON Representation</span></span>
<span data-ttu-id="b0d76-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0d76-121">Here is a JSON representation of the resource.</span></span>
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




