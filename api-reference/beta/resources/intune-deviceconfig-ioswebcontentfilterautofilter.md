---
title: iosWebContentFilterAutoFilter 资源类型
description: 表示 iOS Web 内容筛选器设置类型, 该类型启用 iOS 自动筛选功能并允许其他 URL 访问控制。 在不使用属性值的情况下构建时, iOS 设备将启用自动筛选器 (而不考虑)。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6065ae50712f65662fd9e751ea6a5b0c5c865f3a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356870"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="6b9d7-104">iosWebContentFilterAutoFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b9d7-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="6b9d7-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b9d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b9d7-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b9d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9d7-107">表示 iOS Web 内容筛选器设置类型, 该类型启用 iOS 自动筛选功能并允许其他 URL 访问控制。</span><span class="sxs-lookup"><span data-stu-id="6b9d7-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="6b9d7-108">在不使用属性值的情况下构建时, iOS 设备将启用自动筛选器 (而不考虑)。</span><span class="sxs-lookup"><span data-stu-id="6b9d7-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="6b9d7-109">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="6b9d7-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b9d7-110">属性</span><span class="sxs-lookup"><span data-stu-id="6b9d7-110">Properties</span></span>
|<span data-ttu-id="6b9d7-111">属性</span><span class="sxs-lookup"><span data-stu-id="6b9d7-111">Property</span></span>|<span data-ttu-id="6b9d7-112">类型</span><span class="sxs-lookup"><span data-stu-id="6b9d7-112">Type</span></span>|<span data-ttu-id="6b9d7-113">说明</span><span class="sxs-lookup"><span data-stu-id="6b9d7-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9d7-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="6b9d7-114">allowedUrls</span></span>|<span data-ttu-id="6b9d7-115">String collection</span><span class="sxs-lookup"><span data-stu-id="6b9d7-115">String collection</span></span>|<span data-ttu-id="6b9d7-116">允许访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="6b9d7-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="6b9d7-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="6b9d7-117">blockedUrls</span></span>|<span data-ttu-id="6b9d7-118">String collection</span><span class="sxs-lookup"><span data-stu-id="6b9d7-118">String collection</span></span>|<span data-ttu-id="6b9d7-119">为 access 阻止的其他 Url</span><span class="sxs-lookup"><span data-stu-id="6b9d7-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b9d7-120">关系</span><span class="sxs-lookup"><span data-stu-id="6b9d7-120">Relationships</span></span>
<span data-ttu-id="6b9d7-121">无</span><span class="sxs-lookup"><span data-stu-id="6b9d7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b9d7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b9d7-122">JSON Representation</span></span>
<span data-ttu-id="6b9d7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b9d7-123">Here is a JSON representation of the resource.</span></span>
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



