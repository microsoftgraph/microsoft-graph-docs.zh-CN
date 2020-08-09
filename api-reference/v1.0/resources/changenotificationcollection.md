---
title: changeNotificationCollection 资源类型
description: 表示发送给订阅者的订阅通知的集合。
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1eadd0fbc14fe9e6581ab6fa3375837653fc0859
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598505"
---
# <a name="changenotificationcollection-resource-type"></a><span data-ttu-id="1d53c-103">changeNotificationCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d53c-103">changeNotificationCollection resource type</span></span>

<span data-ttu-id="1d53c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d53c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d53c-105">表示发送给订阅者的资源更改通知的集合。</span><span class="sxs-lookup"><span data-stu-id="1d53c-105">Represents a collection of resource change notifications sent to the subscriber.</span></span>

<span data-ttu-id="1d53c-106">有关详细信息，请参阅[使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="1d53c-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1d53c-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d53c-107">Methods</span></span>

<span data-ttu-id="1d53c-108">无。</span><span class="sxs-lookup"><span data-stu-id="1d53c-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="1d53c-109">属性</span><span class="sxs-lookup"><span data-stu-id="1d53c-109">Properties</span></span>

| <span data-ttu-id="1d53c-110">属性</span><span class="sxs-lookup"><span data-stu-id="1d53c-110">Property</span></span> | <span data-ttu-id="1d53c-111">类型</span><span class="sxs-lookup"><span data-stu-id="1d53c-111">Type</span></span> | <span data-ttu-id="1d53c-112">说明</span><span class="sxs-lookup"><span data-stu-id="1d53c-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1d53c-113">值</span><span class="sxs-lookup"><span data-stu-id="1d53c-113">value</span></span> | <span data-ttu-id="1d53c-114"> ([changeNotification](changenotification.md)) 的集合</span><span class="sxs-lookup"><span data-stu-id="1d53c-114">collection([changeNotification](changenotification.md))</span></span> | <span data-ttu-id="1d53c-115">发送到通知 URL 的一组通知。</span><span class="sxs-lookup"><span data-stu-id="1d53c-115">The set of notifications being sent to the notification URL.</span></span> <span data-ttu-id="1d53c-116">必填。</span><span class="sxs-lookup"><span data-stu-id="1d53c-116">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d53c-117">关系</span><span class="sxs-lookup"><span data-stu-id="1d53c-117">Relationships</span></span>

<span data-ttu-id="1d53c-118">无。</span><span class="sxs-lookup"><span data-stu-id="1d53c-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d53c-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d53c-119">JSON representation</span></span>

<span data-ttu-id="1d53c-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d53c-120">The following is a JSON representation of the resource.</span></span>

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
