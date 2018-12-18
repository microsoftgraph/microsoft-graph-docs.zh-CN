---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: tfitzmac
ms.openlocfilehash: 147504fc356f3a4092b2ffd1c7d03275ff7dea31
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353639"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="382a6-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="382a6-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="382a6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="382a6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="382a6-105">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="382a6-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="382a6-106">属性</span><span class="sxs-lookup"><span data-stu-id="382a6-106">Properties</span></span>
|<span data-ttu-id="382a6-107">属性</span><span class="sxs-lookup"><span data-stu-id="382a6-107">Property</span></span>|<span data-ttu-id="382a6-108">类型</span><span class="sxs-lookup"><span data-stu-id="382a6-108">Type</span></span>|<span data-ttu-id="382a6-109">说明</span><span class="sxs-lookup"><span data-stu-id="382a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="382a6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="382a6-110">displayName</span></span>|<span data-ttu-id="382a6-111">String</span><span class="sxs-lookup"><span data-stu-id="382a6-111">String</span></span>|<span data-ttu-id="382a6-112">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="382a6-112">Name of the folder page</span></span>|
|<span data-ttu-id="382a6-113">应用</span><span class="sxs-lookup"><span data-stu-id="382a6-113">apps</span></span>|<span data-ttu-id="382a6-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="382a6-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="382a6-115">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="382a6-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="382a6-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="382a6-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="382a6-117">关系</span><span class="sxs-lookup"><span data-stu-id="382a6-117">Relationships</span></span>
<span data-ttu-id="382a6-118">无</span><span class="sxs-lookup"><span data-stu-id="382a6-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="382a6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="382a6-119">JSON Representation</span></span>
<span data-ttu-id="382a6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="382a6-120">Here is a JSON representation of the resource.</span></span>
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



