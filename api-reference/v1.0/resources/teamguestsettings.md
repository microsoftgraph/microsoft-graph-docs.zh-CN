---
title: teamGuestSettings 资源类型
description: 要配置的是否来宾可以创建、 更新或删除通道团队中的设置。
ms.openlocfilehash: 3c59c84e0baa9db580a81eeb72a405ec5097c478
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010287"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="ff164-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff164-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="ff164-104">要配置的是否来宾可以创建、 更新或删除通道[团队](team.md)中的设置。</span><span class="sxs-lookup"><span data-stu-id="ff164-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ff164-105">属性</span><span class="sxs-lookup"><span data-stu-id="ff164-105">Properties</span></span>
| <span data-ttu-id="ff164-106">属性</span><span class="sxs-lookup"><span data-stu-id="ff164-106">Property</span></span>     | <span data-ttu-id="ff164-107">类型</span><span class="sxs-lookup"><span data-stu-id="ff164-107">Type</span></span>   |<span data-ttu-id="ff164-108">说明</span><span class="sxs-lookup"><span data-stu-id="ff164-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff164-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ff164-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ff164-110">布尔</span><span class="sxs-lookup"><span data-stu-id="ff164-110">Boolean</span></span>|<span data-ttu-id="ff164-111">如果设置为 true，则来宾可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="ff164-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="ff164-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ff164-112">allowDeleteChannels</span></span>|<span data-ttu-id="ff164-113">布尔</span><span class="sxs-lookup"><span data-stu-id="ff164-113">Boolean</span></span>|<span data-ttu-id="ff164-114">如果设置为 true，则来宾可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="ff164-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff164-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff164-115">JSON representation</span></span>

<span data-ttu-id="ff164-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff164-116">The following is a JSON representation of the resource.</span></span>

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
