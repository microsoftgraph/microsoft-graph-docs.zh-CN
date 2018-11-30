---
title: iosHomeScreenFolderPage 资源类型
description: 包含主屏幕上的应用的文件夹
ms.openlocfilehash: 7cf34cd3bbd4f196db70da3a88ba3768c3d4d630
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042940"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="0d3ab-103">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d3ab-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="0d3ab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0d3ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d3ab-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0d3ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d3ab-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0d3ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d3ab-107">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="0d3ab-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="0d3ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d3ab-108">Properties</span></span>
|<span data-ttu-id="0d3ab-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d3ab-109">Property</span></span>|<span data-ttu-id="0d3ab-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d3ab-110">Type</span></span>|<span data-ttu-id="0d3ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d3ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d3ab-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0d3ab-112">displayName</span></span>|<span data-ttu-id="0d3ab-113">String</span><span class="sxs-lookup"><span data-stu-id="0d3ab-113">String</span></span>|<span data-ttu-id="0d3ab-114">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="0d3ab-114">Name of the folder page</span></span>|
|<span data-ttu-id="0d3ab-115">应用</span><span class="sxs-lookup"><span data-stu-id="0d3ab-115">apps</span></span>|<span data-ttu-id="0d3ab-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d3ab-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="0d3ab-117">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="0d3ab-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="0d3ab-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0d3ab-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d3ab-119">关系</span><span class="sxs-lookup"><span data-stu-id="0d3ab-119">Relationships</span></span>
<span data-ttu-id="0d3ab-120">无</span><span class="sxs-lookup"><span data-stu-id="0d3ab-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0d3ab-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d3ab-121">JSON Representation</span></span>
<span data-ttu-id="0d3ab-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d3ab-122">Here is a JSON representation of the resource.</span></span>
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





