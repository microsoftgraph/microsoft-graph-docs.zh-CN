---
title: payloadTypes 资源类型
description: 表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 034770f2614bacdb9d160f4ff8d2efb4cd0a2c24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998094"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="fd555-103">payloadTypes 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd555-103">payloadTypes resource type</span></span>

<span data-ttu-id="fd555-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd555-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd555-105">此资源表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。</span><span class="sxs-lookup"><span data-stu-id="fd555-105">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="fd555-106">属性</span><span class="sxs-lookup"><span data-stu-id="fd555-106">Properties</span></span>

| <span data-ttu-id="fd555-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd555-107">Property</span></span>     | <span data-ttu-id="fd555-108">类型</span><span class="sxs-lookup"><span data-stu-id="fd555-108">Type</span></span>        | <span data-ttu-id="fd555-109">说明</span><span class="sxs-lookup"><span data-stu-id="fd555-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd555-110">rawContent</span><span class="sxs-lookup"><span data-stu-id="fd555-110">rawContent</span></span>|<span data-ttu-id="fd555-111">String</span><span class="sxs-lookup"><span data-stu-id="fd555-111">String</span></span>|<span data-ttu-id="fd555-112">将在所有受支持的平台上的应用程序客户端传递和使用的原始用户通知的通知内容 (Windows、iOS、Android 或 WebPush) 收到此通知。</span><span class="sxs-lookup"><span data-stu-id="fd555-112">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="fd555-113">RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。</span><span class="sxs-lookup"><span data-stu-id="fd555-113">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="fd555-114">visualContent</span><span class="sxs-lookup"><span data-stu-id="fd555-114">visualContent</span></span>|[<span data-ttu-id="fd555-115">visualProperties</span><span class="sxs-lookup"><span data-stu-id="fd555-115">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="fd555-116">可视化用户通知的可视内容（将由每个受支持的平台上的通知平台使用） (Windows、iOS 和 Android 仅) 并为用户呈现。</span><span class="sxs-lookup"><span data-stu-id="fd555-116">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="fd555-117">RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。</span><span class="sxs-lookup"><span data-stu-id="fd555-117">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fd555-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd555-118">JSON representation</span></span>

<span data-ttu-id="fd555-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd555-119">The following is a JSON representation of the resource.</span></span>

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

