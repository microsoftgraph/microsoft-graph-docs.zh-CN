---
title: resourceData 资源类型
description: 表示附加到发送给订阅者更改通知的数据源。
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: b2ddfd62a797cbf5674f522d6fa3c93eca528c30
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469365"
---
# <a name="resourcedata-resource-type"></a><span data-ttu-id="bc684-103">resourceData 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc684-103">resourceData resource type</span></span>

<span data-ttu-id="bc684-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc684-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc684-105">表示附加到发送给订阅者更改通知的数据源。</span><span class="sxs-lookup"><span data-stu-id="bc684-105">Represents the resouce data attached to the change notification sent to the subscriber.</span></span>

<span data-ttu-id="bc684-106">有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="bc684-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bc684-107">方法</span><span class="sxs-lookup"><span data-stu-id="bc684-107">Methods</span></span>

<span data-ttu-id="bc684-108">无。</span><span class="sxs-lookup"><span data-stu-id="bc684-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="bc684-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc684-109">Properties</span></span>

<span data-ttu-id="bc684-110">对于 Outlook 资源 **，resourceData** 包含以下字段：</span><span class="sxs-lookup"><span data-stu-id="bc684-110">For Outlook resources, **resourceData** contains the following fields:</span></span>

| <span data-ttu-id="bc684-111">属性</span><span class="sxs-lookup"><span data-stu-id="bc684-111">Property</span></span> | <span data-ttu-id="bc684-112">类型</span><span class="sxs-lookup"><span data-stu-id="bc684-112">Type</span></span> | <span data-ttu-id="bc684-113">说明</span><span class="sxs-lookup"><span data-stu-id="bc684-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="bc684-114">@odata.type</span><span class="sxs-lookup"><span data-stu-id="bc684-114">@odata.type</span></span> | <span data-ttu-id="bc684-115">string</span><span class="sxs-lookup"><span data-stu-id="bc684-115">string</span></span> | <span data-ttu-id="bc684-116">Microsoft Graph 中描述所表示对象的 OData 实体类型。</span><span class="sxs-lookup"><span data-stu-id="bc684-116">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="bc684-117">@odata.id</span><span class="sxs-lookup"><span data-stu-id="bc684-117">@odata.id</span></span> | <span data-ttu-id="bc684-118">string</span><span class="sxs-lookup"><span data-stu-id="bc684-118">string</span></span> | <span data-ttu-id="bc684-119">对象的 OData 标识符。</span><span class="sxs-lookup"><span data-stu-id="bc684-119">The OData identifier of the object.</span></span> |
| <span data-ttu-id="bc684-120">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="bc684-120">@odata.etag</span></span> | <span data-ttu-id="bc684-121">string</span><span class="sxs-lookup"><span data-stu-id="bc684-121">string</span></span> | <span data-ttu-id="bc684-122">表示对象版本的 HTTP 实体标记。</span><span class="sxs-lookup"><span data-stu-id="bc684-122">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="bc684-123">id</span><span class="sxs-lookup"><span data-stu-id="bc684-123">id</span></span> | <span data-ttu-id="bc684-124">string</span><span class="sxs-lookup"><span data-stu-id="bc684-124">string</span></span> | <span data-ttu-id="bc684-125">对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="bc684-125">The identifier of the object.</span></span> |

> <span data-ttu-id="bc684-126">**注意：**`id` **resourceData 中提供的值** 在生成更改通知时有效。</span><span class="sxs-lookup"><span data-stu-id="bc684-126">**Note:** The `id` value provided in **resourceData** is valid at the time the change notification was generated.</span></span> <span data-ttu-id="bc684-127">某些操作（如将邮件移动到另一个文件夹）可能会导致处理更改通知时不再 `id` 有效。</span><span class="sxs-lookup"><span data-stu-id="bc684-127">Some actions, such as moving a message to another folder, might result in the `id` no longer being valid when the change notification is processed.</span></span>

## <a name="relationships"></a><span data-ttu-id="bc684-128">关系</span><span class="sxs-lookup"><span data-stu-id="bc684-128">Relationships</span></span>

<span data-ttu-id="bc684-129">无。</span><span class="sxs-lookup"><span data-stu-id="bc684-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc684-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc684-130">JSON representation</span></span>

<span data-ttu-id="bc684-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc684-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "id": "1565293727947",
  "@odata.type": "#Microsoft.Graph.ChatMessage",
  "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
}
```

<!-- uuid: eb6c98ec-8257-4826-910e-5c603265257f
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource data resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


