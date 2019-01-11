---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a2019b114d785867fedca2f054f7280b37fae934
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841158"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="6c3ef-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c3ef-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="6c3ef-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c3ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c3ef-105">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="6c3ef-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="6c3ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="6c3ef-106">Properties</span></span>
|<span data-ttu-id="6c3ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="6c3ef-107">Property</span></span>|<span data-ttu-id="6c3ef-108">类型</span><span class="sxs-lookup"><span data-stu-id="6c3ef-108">Type</span></span>|<span data-ttu-id="6c3ef-109">说明</span><span class="sxs-lookup"><span data-stu-id="6c3ef-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3ef-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6c3ef-110">displayName</span></span>|<span data-ttu-id="6c3ef-111">String</span><span class="sxs-lookup"><span data-stu-id="6c3ef-111">String</span></span>|<span data-ttu-id="6c3ef-112">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="6c3ef-112">Name of the folder page</span></span>|
|<span data-ttu-id="6c3ef-113">应用</span><span class="sxs-lookup"><span data-stu-id="6c3ef-113">apps</span></span>|<span data-ttu-id="6c3ef-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c3ef-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="6c3ef-115">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="6c3ef-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="6c3ef-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6c3ef-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c3ef-117">关系</span><span class="sxs-lookup"><span data-stu-id="6c3ef-117">Relationships</span></span>
<span data-ttu-id="6c3ef-118">无</span><span class="sxs-lookup"><span data-stu-id="6c3ef-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c3ef-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c3ef-119">JSON Representation</span></span>
<span data-ttu-id="6c3ef-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c3ef-120">Here is a JSON representation of the resource.</span></span>
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



