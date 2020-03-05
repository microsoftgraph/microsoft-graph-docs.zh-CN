---
title: iosWebContentFilterAutoFilter 资源类型
description: 表示 iOS Web 内容筛选器设置类型，该类型启用 iOS 自动筛选功能并允许其他 URL 访问控制。 在不使用属性值的情况下构建时，iOS 设备将启用自动筛选器（而不考虑）。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b3bcf8c66aff4220b7e2b394819beb35255bfba3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529820"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="7dce9-104">iosWebContentFilterAutoFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="7dce9-104">iosWebContentFilterAutoFilter resource type</span></span>

<span data-ttu-id="7dce9-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7dce9-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dce9-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7dce9-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dce9-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7dce9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dce9-108">表示 iOS Web 内容筛选器设置类型，该类型启用 iOS 自动筛选功能并允许其他 URL 访问控制。</span><span class="sxs-lookup"><span data-stu-id="7dce9-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="7dce9-109">在不使用属性值的情况下构建时，iOS 设备将启用自动筛选器（而不考虑）。</span><span class="sxs-lookup"><span data-stu-id="7dce9-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="7dce9-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="7dce9-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7dce9-111">属性</span><span class="sxs-lookup"><span data-stu-id="7dce9-111">Properties</span></span>
|<span data-ttu-id="7dce9-112">属性</span><span class="sxs-lookup"><span data-stu-id="7dce9-112">Property</span></span>|<span data-ttu-id="7dce9-113">类型</span><span class="sxs-lookup"><span data-stu-id="7dce9-113">Type</span></span>|<span data-ttu-id="7dce9-114">说明</span><span class="sxs-lookup"><span data-stu-id="7dce9-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dce9-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="7dce9-115">allowedUrls</span></span>|<span data-ttu-id="7dce9-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="7dce9-116">String collection</span></span>|<span data-ttu-id="7dce9-117">允许访问的其他 Url</span><span class="sxs-lookup"><span data-stu-id="7dce9-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="7dce9-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="7dce9-118">blockedUrls</span></span>|<span data-ttu-id="7dce9-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="7dce9-119">String collection</span></span>|<span data-ttu-id="7dce9-120">为 access 阻止的其他 Url</span><span class="sxs-lookup"><span data-stu-id="7dce9-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dce9-121">关系</span><span class="sxs-lookup"><span data-stu-id="7dce9-121">Relationships</span></span>
<span data-ttu-id="7dce9-122">无</span><span class="sxs-lookup"><span data-stu-id="7dce9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dce9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7dce9-123">JSON Representation</span></span>
<span data-ttu-id="7dce9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dce9-124">Here is a JSON representation of the resource.</span></span>
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



