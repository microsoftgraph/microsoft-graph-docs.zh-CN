---
title: iosWebContentFilterAutoFilter 资源类型
description: 代表 iOS Web 内容筛选器设置类型，它使 iOS 自动筛选功能并允许其他 URL 访问控制。 没有属性值来构造，iOS 设备将启用自动筛选器无论。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 03e3c4f51e673be1e2bada89e06a26048fe4e385
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916776"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="0f446-104">iosWebContentFilterAutoFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f446-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="0f446-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0f446-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f446-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f446-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f446-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0f446-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f446-108">代表 iOS Web 内容筛选器设置类型，它使 iOS 自动筛选功能并允许其他 URL 访问控制。</span><span class="sxs-lookup"><span data-stu-id="0f446-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="0f446-109">没有属性值来构造，iOS 设备将启用自动筛选器无论。</span><span class="sxs-lookup"><span data-stu-id="0f446-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="0f446-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="0f446-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f446-111">属性</span><span class="sxs-lookup"><span data-stu-id="0f446-111">Properties</span></span>
|<span data-ttu-id="0f446-112">属性</span><span class="sxs-lookup"><span data-stu-id="0f446-112">Property</span></span>|<span data-ttu-id="0f446-113">类型</span><span class="sxs-lookup"><span data-stu-id="0f446-113">Type</span></span>|<span data-ttu-id="0f446-114">说明</span><span class="sxs-lookup"><span data-stu-id="0f446-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f446-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="0f446-115">allowedUrls</span></span>|<span data-ttu-id="0f446-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f446-116">String collection</span></span>|<span data-ttu-id="0f446-117">允许的访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="0f446-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="0f446-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="0f446-118">blockedUrls</span></span>|<span data-ttu-id="0f446-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f446-119">String collection</span></span>|<span data-ttu-id="0f446-120">阻止访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="0f446-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f446-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="0f446-121">Relationships</span></span>
<span data-ttu-id="0f446-122">无</span><span class="sxs-lookup"><span data-stu-id="0f446-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f446-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f446-123">JSON Representation</span></span>
<span data-ttu-id="0f446-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f446-124">Here is a JSON representation of the resource.</span></span>
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





