---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa9462f8fb0640584515d1c209abd03de0e6200
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424173"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="66b1c-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="66b1c-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="66b1c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="66b1c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66b1c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66b1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66b1c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66b1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66b1c-107">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="66b1c-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="66b1c-108">属性</span><span class="sxs-lookup"><span data-stu-id="66b1c-108">Properties</span></span>
|<span data-ttu-id="66b1c-109">属性</span><span class="sxs-lookup"><span data-stu-id="66b1c-109">Property</span></span>|<span data-ttu-id="66b1c-110">类型</span><span class="sxs-lookup"><span data-stu-id="66b1c-110">Type</span></span>|<span data-ttu-id="66b1c-111">说明</span><span class="sxs-lookup"><span data-stu-id="66b1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b1c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="66b1c-112">displayName</span></span>|<span data-ttu-id="66b1c-113">String</span><span class="sxs-lookup"><span data-stu-id="66b1c-113">String</span></span>|<span data-ttu-id="66b1c-114">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="66b1c-114">Name of the folder page</span></span>|
|<span data-ttu-id="66b1c-115">应用</span><span class="sxs-lookup"><span data-stu-id="66b1c-115">apps</span></span>|<span data-ttu-id="66b1c-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66b1c-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="66b1c-117">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="66b1c-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="66b1c-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="66b1c-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66b1c-119">关系</span><span class="sxs-lookup"><span data-stu-id="66b1c-119">Relationships</span></span>
<span data-ttu-id="66b1c-120">无</span><span class="sxs-lookup"><span data-stu-id="66b1c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66b1c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66b1c-121">JSON Representation</span></span>
<span data-ttu-id="66b1c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66b1c-122">Here is a JSON representation of the resource.</span></span>
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




