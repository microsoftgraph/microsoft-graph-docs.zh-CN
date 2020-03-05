---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fe3117eae0e514bea979281220da12820574cb4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520897"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="ae091-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae091-104">searchRequest resource type</span></span>

<span data-ttu-id="ae091-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ae091-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae091-106">要发送到查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="ae091-106">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="ae091-107">它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="ae091-107">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="ae091-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae091-108">Properties</span></span>

| <span data-ttu-id="ae091-109">属性</span><span class="sxs-lookup"><span data-stu-id="ae091-109">Property</span></span>     | <span data-ttu-id="ae091-110">类型</span><span class="sxs-lookup"><span data-stu-id="ae091-110">Type</span></span>        | <span data-ttu-id="ae091-111">说明</span><span class="sxs-lookup"><span data-stu-id="ae091-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae091-112">stored_fields</span><span class="sxs-lookup"><span data-stu-id="ae091-112">stored_fields</span></span>|<span data-ttu-id="ae091-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="ae091-113">String collection</span></span> |<span data-ttu-id="ae091-114">包含要为搜索 _so urces 对象返回的字段。</span><span class="sxs-lookup"><span data-stu-id="ae091-114">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="ae091-115">注释仅当在响应中指定了`externalItem` entityType = 时，这才适用。</span><span class="sxs-lookup"><span data-stu-id="ae091-115">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="ae091-116">contentSources</span><span class="sxs-lookup"><span data-stu-id="ae091-116">contentSources</span></span>|<span data-ttu-id="ae091-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="ae091-117">String collection</span></span>|<span data-ttu-id="ae091-118">包含要设定的连接。</span><span class="sxs-lookup"><span data-stu-id="ae091-118">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="ae091-119">遵循以下格式：在`/external/connections/connectionid`连接器`connectionid`管理中定义 ConnectionId 的位置。</span><span class="sxs-lookup"><span data-stu-id="ae091-119">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="ae091-120">注释 contentSource 仅当 entityType =`externalItem`时适用。</span><span class="sxs-lookup"><span data-stu-id="ae091-120">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="ae091-121">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="ae091-121">enableTopResults</span></span>|<span data-ttu-id="ae091-122">布尔</span><span class="sxs-lookup"><span data-stu-id="ae091-122">Boolean</span></span>|<span data-ttu-id="ae091-123">这将触发邮件的混合排序：前3个邮件最相关</span><span class="sxs-lookup"><span data-stu-id="ae091-123">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="ae091-124">这仅适用于 entityType =`message`。</span><span class="sxs-lookup"><span data-stu-id="ae091-124">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="ae091-125">entityTypes</span><span class="sxs-lookup"><span data-stu-id="ae091-125">entityTypes</span></span>|<span data-ttu-id="ae091-126">`entityType` 集合</span><span class="sxs-lookup"><span data-stu-id="ae091-126">`entityType` collection</span></span>| <span data-ttu-id="ae091-127">可取值为：`event`、`message`、`driveItem`、`externalFile`、`externalItem`。</span><span class="sxs-lookup"><span data-stu-id="ae091-127">Possible values are: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span></span>|
|<span data-ttu-id="ae091-128">发件人</span><span class="sxs-lookup"><span data-stu-id="ae091-128">from</span></span>|<span data-ttu-id="ae091-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ae091-129">Int32</span></span>|<span data-ttu-id="ae091-130">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="ae091-130">Specifies the offset for the search results.</span></span> <span data-ttu-id="ae091-131">偏移量0返回的第一个结果。</span><span class="sxs-lookup"><span data-stu-id="ae091-131">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="ae091-132">查询</span><span class="sxs-lookup"><span data-stu-id="ae091-132">query</span></span>|[<span data-ttu-id="ae091-133">searchQuery</span><span class="sxs-lookup"><span data-stu-id="ae091-133">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="ae091-134">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="ae091-134">Contains the query terms.</span></span>|
|<span data-ttu-id="ae091-135">size</span><span class="sxs-lookup"><span data-stu-id="ae091-135">size</span></span>|<span data-ttu-id="ae091-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ae091-136">Int32</span></span>|<span data-ttu-id="ae091-137">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="ae091-137">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae091-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae091-138">JSON representation</span></span>

<span data-ttu-id="ae091-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae091-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "stored_fields": ["String"],
  "contentSources": ["String"],
  "entityTypes": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "enableTopResults": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
