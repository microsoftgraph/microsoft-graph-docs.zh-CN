---
title: iosWebContentFilterAutoFilter 资源类型
description: 代表 iOS Web 内容筛选器设置类型，它使 iOS 自动筛选功能并允许其他 URL 访问控制。 没有属性值来构造，iOS 设备将启用自动筛选器无论。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401227"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="3ab22-104">iosWebContentFilterAutoFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ab22-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="3ab22-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3ab22-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ab22-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ab22-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ab22-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ab22-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ab22-108">代表 iOS Web 内容筛选器设置类型，它使 iOS 自动筛选功能并允许其他 URL 访问控制。</span><span class="sxs-lookup"><span data-stu-id="3ab22-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="3ab22-109">没有属性值来构造，iOS 设备将启用自动筛选器无论。</span><span class="sxs-lookup"><span data-stu-id="3ab22-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="3ab22-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="3ab22-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ab22-111">属性</span><span class="sxs-lookup"><span data-stu-id="3ab22-111">Properties</span></span>
|<span data-ttu-id="3ab22-112">属性</span><span class="sxs-lookup"><span data-stu-id="3ab22-112">Property</span></span>|<span data-ttu-id="3ab22-113">类型</span><span class="sxs-lookup"><span data-stu-id="3ab22-113">Type</span></span>|<span data-ttu-id="3ab22-114">说明</span><span class="sxs-lookup"><span data-stu-id="3ab22-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ab22-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="3ab22-115">allowedUrls</span></span>|<span data-ttu-id="3ab22-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="3ab22-116">String collection</span></span>|<span data-ttu-id="3ab22-117">允许的访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="3ab22-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="3ab22-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="3ab22-118">blockedUrls</span></span>|<span data-ttu-id="3ab22-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="3ab22-119">String collection</span></span>|<span data-ttu-id="3ab22-120">阻止访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="3ab22-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ab22-121">关系</span><span class="sxs-lookup"><span data-stu-id="3ab22-121">Relationships</span></span>
<span data-ttu-id="3ab22-122">无</span><span class="sxs-lookup"><span data-stu-id="3ab22-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ab22-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ab22-123">JSON Representation</span></span>
<span data-ttu-id="3ab22-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ab22-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




