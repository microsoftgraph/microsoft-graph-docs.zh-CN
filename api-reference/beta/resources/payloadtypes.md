---
title: payloadTypes 资源类型
description: 表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 2d740c5b19b363fa2534984bf059cd186b065e89
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939605"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="feb7c-103">payloadTypes 资源类型</span><span class="sxs-lookup"><span data-stu-id="feb7c-103">payloadTypes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feb7c-104">此资源表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。</span><span class="sxs-lookup"><span data-stu-id="feb7c-104">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="feb7c-105">属性</span><span class="sxs-lookup"><span data-stu-id="feb7c-105">Properties</span></span>

| <span data-ttu-id="feb7c-106">属性</span><span class="sxs-lookup"><span data-stu-id="feb7c-106">Property</span></span>     | <span data-ttu-id="feb7c-107">类型</span><span class="sxs-lookup"><span data-stu-id="feb7c-107">Type</span></span>        | <span data-ttu-id="feb7c-108">描述</span><span class="sxs-lookup"><span data-stu-id="feb7c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="feb7c-109">rawContent</span><span class="sxs-lookup"><span data-stu-id="feb7c-109">rawContent</span></span>|<span data-ttu-id="feb7c-110">字符串</span><span class="sxs-lookup"><span data-stu-id="feb7c-110">String</span></span>|<span data-ttu-id="feb7c-111">收到此通知的所有受支持的平台（Windows、iOS、Android 或 WebPush）上的应用程序客户端将传递给和使用的原始用户通知的通知内容。</span><span class="sxs-lookup"><span data-stu-id="feb7c-111">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="feb7c-112">RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。</span><span class="sxs-lookup"><span data-stu-id="feb7c-112">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="feb7c-113">visualContent</span><span class="sxs-lookup"><span data-stu-id="feb7c-113">visualContent</span></span>|[<span data-ttu-id="feb7c-114">visualProperties</span><span class="sxs-lookup"><span data-stu-id="feb7c-114">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="feb7c-115">可视用户通知的可视内容，该通知将由每个受支持的平台（仅适用于 Windows、iOS 和 Android）上的通知平台使用，并为用户呈现。</span><span class="sxs-lookup"><span data-stu-id="feb7c-115">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="feb7c-116">RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。</span><span class="sxs-lookup"><span data-stu-id="feb7c-116">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="feb7c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="feb7c-117">JSON representation</span></span>

<span data-ttu-id="feb7c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="feb7c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.payloadTypes",
  "baseType": null
}-->

```json
{
  "rawContent": "String",
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "payloadTypes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->