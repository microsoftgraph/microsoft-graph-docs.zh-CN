---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00c67b7a0679d92ef6aac78bc0317e461dcd2f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554637"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="dcb31-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcb31-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="dcb31-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcb31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb31-105">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="dcb31-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="dcb31-106">属性</span><span class="sxs-lookup"><span data-stu-id="dcb31-106">Properties</span></span>
|<span data-ttu-id="dcb31-107">属性</span><span class="sxs-lookup"><span data-stu-id="dcb31-107">Property</span></span>|<span data-ttu-id="dcb31-108">类型</span><span class="sxs-lookup"><span data-stu-id="dcb31-108">Type</span></span>|<span data-ttu-id="dcb31-109">说明</span><span class="sxs-lookup"><span data-stu-id="dcb31-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb31-110">displayName</span><span class="sxs-lookup"><span data-stu-id="dcb31-110">displayName</span></span>|<span data-ttu-id="dcb31-111">String</span><span class="sxs-lookup"><span data-stu-id="dcb31-111">String</span></span>|<span data-ttu-id="dcb31-112">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="dcb31-112">Name of the folder page</span></span>|
|<span data-ttu-id="dcb31-113">应用</span><span class="sxs-lookup"><span data-stu-id="dcb31-113">apps</span></span>|<span data-ttu-id="dcb31-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dcb31-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="dcb31-115">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="dcb31-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="dcb31-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="dcb31-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcb31-117">关系</span><span class="sxs-lookup"><span data-stu-id="dcb31-117">Relationships</span></span>
<span data-ttu-id="dcb31-118">无</span><span class="sxs-lookup"><span data-stu-id="dcb31-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcb31-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcb31-119">JSON Representation</span></span>
<span data-ttu-id="dcb31-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcb31-120">Here is a JSON representation of the resource.</span></span>
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



