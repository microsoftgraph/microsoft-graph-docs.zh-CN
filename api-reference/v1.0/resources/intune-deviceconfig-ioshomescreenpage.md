---
title: iosHomeScreenPage 资源类型
description: 包含主屏幕上的应用和文件夹的页面
author: tfitzmac
ms.openlocfilehash: b8aca5c671d0c8521cdf8a870a2f0ad3cd35ba1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321460"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="19d62-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="19d62-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="19d62-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="19d62-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19d62-105">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="19d62-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="19d62-106">属性</span><span class="sxs-lookup"><span data-stu-id="19d62-106">Properties</span></span>
|<span data-ttu-id="19d62-107">属性</span><span class="sxs-lookup"><span data-stu-id="19d62-107">Property</span></span>|<span data-ttu-id="19d62-108">类型</span><span class="sxs-lookup"><span data-stu-id="19d62-108">Type</span></span>|<span data-ttu-id="19d62-109">说明</span><span class="sxs-lookup"><span data-stu-id="19d62-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d62-110">displayName</span><span class="sxs-lookup"><span data-stu-id="19d62-110">displayName</span></span>|<span data-ttu-id="19d62-111">String</span><span class="sxs-lookup"><span data-stu-id="19d62-111">String</span></span>|<span data-ttu-id="19d62-112">页面的名称</span><span class="sxs-lookup"><span data-stu-id="19d62-112">Name of the page</span></span>|
|<span data-ttu-id="19d62-113">图标</span><span class="sxs-lookup"><span data-stu-id="19d62-113">icons</span></span>|<span data-ttu-id="19d62-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19d62-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="19d62-115">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="19d62-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="19d62-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="19d62-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d62-117">关系</span><span class="sxs-lookup"><span data-stu-id="19d62-117">Relationships</span></span>
<span data-ttu-id="19d62-118">无</span><span class="sxs-lookup"><span data-stu-id="19d62-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19d62-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19d62-119">JSON Representation</span></span>
<span data-ttu-id="19d62-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19d62-120">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
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



