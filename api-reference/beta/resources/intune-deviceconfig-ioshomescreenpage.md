---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
ms.openlocfilehash: 4f89d32d68b1caef782fa9a023145ad8ea896155
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042622"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="4004a-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="4004a-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="4004a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4004a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4004a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4004a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4004a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4004a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4004a-107">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="4004a-107">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="4004a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4004a-108">Properties</span></span>
|<span data-ttu-id="4004a-109">属性</span><span class="sxs-lookup"><span data-stu-id="4004a-109">Property</span></span>|<span data-ttu-id="4004a-110">类型</span><span class="sxs-lookup"><span data-stu-id="4004a-110">Type</span></span>|<span data-ttu-id="4004a-111">说明</span><span class="sxs-lookup"><span data-stu-id="4004a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4004a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4004a-112">displayName</span></span>|<span data-ttu-id="4004a-113">String</span><span class="sxs-lookup"><span data-stu-id="4004a-113">String</span></span>|<span data-ttu-id="4004a-114">页面的名称</span><span class="sxs-lookup"><span data-stu-id="4004a-114">Name of the page</span></span>|
|<span data-ttu-id="4004a-115">图标</span><span class="sxs-lookup"><span data-stu-id="4004a-115">icons</span></span>|<span data-ttu-id="4004a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4004a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="4004a-117">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="4004a-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="4004a-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4004a-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4004a-119">关系</span><span class="sxs-lookup"><span data-stu-id="4004a-119">Relationships</span></span>
<span data-ttu-id="4004a-120">无</span><span class="sxs-lookup"><span data-stu-id="4004a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4004a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4004a-121">JSON Representation</span></span>
<span data-ttu-id="4004a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4004a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```





