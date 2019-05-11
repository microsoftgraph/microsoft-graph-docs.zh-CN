---
title: iosWebContentFilterAutoFilter 资源类型
description: 表示 iOS Web 内容筛选器设置类型, 该类型启用 iOS 自动筛选功能并允许其他 URL 访问控制。 在不使用属性值的情况下构建时, iOS 设备将启用自动筛选器 (而不考虑)。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6bf2da4320c228123e24ae67bd21b13f2c21eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946068"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="fba08-104">iosWebContentFilterAutoFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="fba08-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="fba08-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fba08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fba08-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fba08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fba08-107">表示 iOS Web 内容筛选器设置类型, 该类型启用 iOS 自动筛选功能并允许其他 URL 访问控制。</span><span class="sxs-lookup"><span data-stu-id="fba08-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="fba08-108">在不使用属性值的情况下构建时, iOS 设备将启用自动筛选器 (而不考虑)。</span><span class="sxs-lookup"><span data-stu-id="fba08-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="fba08-109">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="fba08-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fba08-110">属性</span><span class="sxs-lookup"><span data-stu-id="fba08-110">Properties</span></span>
|<span data-ttu-id="fba08-111">属性</span><span class="sxs-lookup"><span data-stu-id="fba08-111">Property</span></span>|<span data-ttu-id="fba08-112">类型</span><span class="sxs-lookup"><span data-stu-id="fba08-112">Type</span></span>|<span data-ttu-id="fba08-113">说明</span><span class="sxs-lookup"><span data-stu-id="fba08-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fba08-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="fba08-114">allowedUrls</span></span>|<span data-ttu-id="fba08-115">String collection</span><span class="sxs-lookup"><span data-stu-id="fba08-115">String collection</span></span>|<span data-ttu-id="fba08-116">允许访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="fba08-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="fba08-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="fba08-117">blockedUrls</span></span>|<span data-ttu-id="fba08-118">String collection</span><span class="sxs-lookup"><span data-stu-id="fba08-118">String collection</span></span>|<span data-ttu-id="fba08-119">为 access 阻止的其他 Url</span><span class="sxs-lookup"><span data-stu-id="fba08-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="fba08-120">关系</span><span class="sxs-lookup"><span data-stu-id="fba08-120">Relationships</span></span>
<span data-ttu-id="fba08-121">无</span><span class="sxs-lookup"><span data-stu-id="fba08-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba08-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fba08-122">JSON Representation</span></span>
<span data-ttu-id="fba08-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fba08-123">Here is a JSON representation of the resource.</span></span>
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




