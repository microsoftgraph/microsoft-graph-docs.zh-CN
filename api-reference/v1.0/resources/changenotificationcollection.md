---
title: changeNotificationCollection 资源类型
description: 表示发送给订阅者的订阅通知的集合。
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: cd3e5508d4281de8c791259882a413127315e0b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037890"
---
# <a name="changenotificationcollection-resource-type"></a><span data-ttu-id="1833d-103">changeNotificationCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="1833d-103">changeNotificationCollection resource type</span></span>

<span data-ttu-id="1833d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1833d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1833d-105">表示发送给订阅者的资源更改通知的集合。</span><span class="sxs-lookup"><span data-stu-id="1833d-105">Represents a collection of resource change notifications sent to the subscriber.</span></span>

<span data-ttu-id="1833d-106">有关详细信息，请参阅 [使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="1833d-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1833d-107">方法</span><span class="sxs-lookup"><span data-stu-id="1833d-107">Methods</span></span>

<span data-ttu-id="1833d-108">无。</span><span class="sxs-lookup"><span data-stu-id="1833d-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="1833d-109">属性</span><span class="sxs-lookup"><span data-stu-id="1833d-109">Properties</span></span>

| <span data-ttu-id="1833d-110">属性</span><span class="sxs-lookup"><span data-stu-id="1833d-110">Property</span></span> | <span data-ttu-id="1833d-111">类型</span><span class="sxs-lookup"><span data-stu-id="1833d-111">Type</span></span> | <span data-ttu-id="1833d-112">说明</span><span class="sxs-lookup"><span data-stu-id="1833d-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1833d-113">值</span><span class="sxs-lookup"><span data-stu-id="1833d-113">value</span></span> | <span data-ttu-id="1833d-114"> ([changeNotification](changenotification.md)) 的集合</span><span class="sxs-lookup"><span data-stu-id="1833d-114">collection([changeNotification](changenotification.md))</span></span> | <span data-ttu-id="1833d-115">发送到通知 URL 的一组通知。</span><span class="sxs-lookup"><span data-stu-id="1833d-115">The set of notifications being sent to the notification URL.</span></span> <span data-ttu-id="1833d-116">必需。</span><span class="sxs-lookup"><span data-stu-id="1833d-116">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1833d-117">关系</span><span class="sxs-lookup"><span data-stu-id="1833d-117">Relationships</span></span>

<span data-ttu-id="1833d-118">无。</span><span class="sxs-lookup"><span data-stu-id="1833d-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1833d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1833d-119">JSON representation</span></span>

<span data-ttu-id="1833d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1833d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}-->

```json
{
  "value": [],
  "validationTokens": [
    "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
  ]
}
```

<!-- uuid: 8cc2599e-9740-4191-93fa-bc13c6f91564
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification collection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

