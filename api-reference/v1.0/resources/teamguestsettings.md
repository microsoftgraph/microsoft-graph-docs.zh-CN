---
title: teamGuestSettings 资源类型
description: 要配置的是否来宾可以创建、 更新或删除通道团队中的设置。
localization_priority: Normal
ms.openlocfilehash: f0947101fc8de83d1a56ffa922d9b1e2d79d520f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844873"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="b9227-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9227-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="b9227-104">要配置的是否来宾可以创建、 更新或删除通道[团队](team.md)中的设置。</span><span class="sxs-lookup"><span data-stu-id="b9227-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9227-105">属性</span><span class="sxs-lookup"><span data-stu-id="b9227-105">Properties</span></span>
| <span data-ttu-id="b9227-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9227-106">Property</span></span>     | <span data-ttu-id="b9227-107">类型</span><span class="sxs-lookup"><span data-stu-id="b9227-107">Type</span></span>   |<span data-ttu-id="b9227-108">Description</span><span class="sxs-lookup"><span data-stu-id="b9227-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9227-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="b9227-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="b9227-110">布尔</span><span class="sxs-lookup"><span data-stu-id="b9227-110">Boolean</span></span>|<span data-ttu-id="b9227-111">如果设置为 true，则来宾可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="b9227-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="b9227-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="b9227-112">allowDeleteChannels</span></span>|<span data-ttu-id="b9227-113">布尔</span><span class="sxs-lookup"><span data-stu-id="b9227-113">Boolean</span></span>|<span data-ttu-id="b9227-114">如果设置为 true，则来宾可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="b9227-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9227-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9227-115">JSON representation</span></span>

<span data-ttu-id="b9227-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9227-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
