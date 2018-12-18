---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: tfitzmac
ms.openlocfilehash: fc5f1899a9eadf88a1815558ed9c1dc9eff51114
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340633"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="ddf25-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="ddf25-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="ddf25-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ddf25-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddf25-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ddf25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddf25-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddf25-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddf25-107">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="ddf25-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="ddf25-108">属性</span><span class="sxs-lookup"><span data-stu-id="ddf25-108">Properties</span></span>
|<span data-ttu-id="ddf25-109">属性</span><span class="sxs-lookup"><span data-stu-id="ddf25-109">Property</span></span>|<span data-ttu-id="ddf25-110">类型</span><span class="sxs-lookup"><span data-stu-id="ddf25-110">Type</span></span>|<span data-ttu-id="ddf25-111">说明</span><span class="sxs-lookup"><span data-stu-id="ddf25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf25-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ddf25-112">displayName</span></span>|<span data-ttu-id="ddf25-113">String</span><span class="sxs-lookup"><span data-stu-id="ddf25-113">String</span></span>|<span data-ttu-id="ddf25-114">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="ddf25-114">Name of the folder page</span></span>|
|<span data-ttu-id="ddf25-115">应用</span><span class="sxs-lookup"><span data-stu-id="ddf25-115">apps</span></span>|<span data-ttu-id="ddf25-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddf25-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="ddf25-117">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="ddf25-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="ddf25-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ddf25-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddf25-119">关系</span><span class="sxs-lookup"><span data-stu-id="ddf25-119">Relationships</span></span>
<span data-ttu-id="ddf25-120">无</span><span class="sxs-lookup"><span data-stu-id="ddf25-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ddf25-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ddf25-121">JSON Representation</span></span>
<span data-ttu-id="ddf25-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddf25-122">Here is a JSON representation of the resource.</span></span>
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





