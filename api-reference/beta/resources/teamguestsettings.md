---
title: teamGuestSettings 资源类型
description: 要配置的是否来宾可以创建、 更新或删除通道团队中的设置。
ms.openlocfilehash: 744e19165121d101a720a86bec0242fc31137768
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045147"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="8583b-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8583b-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="8583b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8583b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8583b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8583b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8583b-106">要配置的是否来宾可以创建、 更新或删除通道[团队](team.md)中的设置。</span><span class="sxs-lookup"><span data-stu-id="8583b-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8583b-107">属性</span><span class="sxs-lookup"><span data-stu-id="8583b-107">Properties</span></span>
| <span data-ttu-id="8583b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8583b-108">Property</span></span>     | <span data-ttu-id="8583b-109">类型</span><span class="sxs-lookup"><span data-stu-id="8583b-109">Type</span></span>   |<span data-ttu-id="8583b-110">说明</span><span class="sxs-lookup"><span data-stu-id="8583b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8583b-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="8583b-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="8583b-112">布尔</span><span class="sxs-lookup"><span data-stu-id="8583b-112">Boolean</span></span>|<span data-ttu-id="8583b-113">如果设置为 true，则来宾可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="8583b-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="8583b-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="8583b-114">allowDeleteChannels</span></span>|<span data-ttu-id="8583b-115">布尔</span><span class="sxs-lookup"><span data-stu-id="8583b-115">Boolean</span></span>|<span data-ttu-id="8583b-116">如果设置为 true，则来宾可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="8583b-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8583b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8583b-117">JSON representation</span></span>

<span data-ttu-id="8583b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8583b-118">The following is a JSON representation of the resource.</span></span>

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
