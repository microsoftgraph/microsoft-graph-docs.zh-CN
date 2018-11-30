---
title: iosHomeScreenFolder 资源类型
description: 包含主屏幕上的应用页面的文件夹
ms.openlocfilehash: 005b35f014cf6ee6967cfa5dfaa235aede155be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047872"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="f1052-103">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1052-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="f1052-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1052-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1052-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1052-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1052-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1052-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1052-107">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="f1052-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="f1052-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f1052-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1052-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1052-109">Properties</span></span>
|<span data-ttu-id="f1052-110">属性</span><span class="sxs-lookup"><span data-stu-id="f1052-110">Property</span></span>|<span data-ttu-id="f1052-111">类型</span><span class="sxs-lookup"><span data-stu-id="f1052-111">Type</span></span>|<span data-ttu-id="f1052-112">说明</span><span class="sxs-lookup"><span data-stu-id="f1052-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1052-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f1052-113">displayName</span></span>|<span data-ttu-id="f1052-114">String</span><span class="sxs-lookup"><span data-stu-id="f1052-114">String</span></span>|<span data-ttu-id="f1052-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="f1052-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="f1052-116">页面</span><span class="sxs-lookup"><span data-stu-id="f1052-116">pages</span></span>|<span data-ttu-id="f1052-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1052-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="f1052-118">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="f1052-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="f1052-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f1052-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1052-120">关系</span><span class="sxs-lookup"><span data-stu-id="f1052-120">Relationships</span></span>
<span data-ttu-id="f1052-121">无</span><span class="sxs-lookup"><span data-stu-id="f1052-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1052-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1052-122">JSON Representation</span></span>
<span data-ttu-id="f1052-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1052-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```





