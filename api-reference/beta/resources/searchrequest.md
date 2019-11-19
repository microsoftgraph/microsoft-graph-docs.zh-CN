---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f19b9a14e1f6f4016e53a4a0ff1f62ae27e1cfd
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703754"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="a97e7-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="a97e7-104">searchRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a97e7-105">要发送到查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="a97e7-105">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="a97e7-106">它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="a97e7-106">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="a97e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="a97e7-107">Properties</span></span>

| <span data-ttu-id="a97e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="a97e7-108">Property</span></span>     | <span data-ttu-id="a97e7-109">类型</span><span class="sxs-lookup"><span data-stu-id="a97e7-109">Type</span></span>        | <span data-ttu-id="a97e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="a97e7-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a97e7-111">stored_fields</span><span class="sxs-lookup"><span data-stu-id="a97e7-111">stored_fields</span></span>|<span data-ttu-id="a97e7-112">String collection</span><span class="sxs-lookup"><span data-stu-id="a97e7-112">String collection</span></span> |<span data-ttu-id="a97e7-113">包含要为搜索 _so urces 对象返回的字段。</span><span class="sxs-lookup"><span data-stu-id="a97e7-113">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="a97e7-114">注释仅当在响应中指定了`externalItem` entityType = 时，这才适用。</span><span class="sxs-lookup"><span data-stu-id="a97e7-114">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="a97e7-115">contentSources</span><span class="sxs-lookup"><span data-stu-id="a97e7-115">contentSources</span></span>|<span data-ttu-id="a97e7-116">String collection</span><span class="sxs-lookup"><span data-stu-id="a97e7-116">String collection</span></span>|<span data-ttu-id="a97e7-117">包含要设定的连接。</span><span class="sxs-lookup"><span data-stu-id="a97e7-117">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="a97e7-118">遵循以下格式：在`/external/connections/connectionid`连接器`connectionid`管理中定义 ConnectionId 的位置。</span><span class="sxs-lookup"><span data-stu-id="a97e7-118">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="a97e7-119">注释 contentSource 仅当 entityType =`externalItem`时适用。</span><span class="sxs-lookup"><span data-stu-id="a97e7-119">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="a97e7-120">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="a97e7-120">enableTopResults</span></span>|<span data-ttu-id="a97e7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="a97e7-121">Boolean</span></span>|<span data-ttu-id="a97e7-122">这将触发邮件的混合排序：前3个邮件最相关</span><span class="sxs-lookup"><span data-stu-id="a97e7-122">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="a97e7-123">这仅适用于 entityType =`message`。</span><span class="sxs-lookup"><span data-stu-id="a97e7-123">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="a97e7-124">entityTypes</span><span class="sxs-lookup"><span data-stu-id="a97e7-124">entityTypes</span></span>|<span data-ttu-id="a97e7-125">`entityType` 集合</span><span class="sxs-lookup"><span data-stu-id="a97e7-125">`entityType` collection</span></span>| <span data-ttu-id="a97e7-126">可取值为：`event`、`message`、`driveItem`、`externalFile`、`externalItem`。</span><span class="sxs-lookup"><span data-stu-id="a97e7-126">Possible values are: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span></span>|
|<span data-ttu-id="a97e7-127">起始数量</span><span class="sxs-lookup"><span data-stu-id="a97e7-127">from</span></span>|<span data-ttu-id="a97e7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a97e7-128">Int32</span></span>|<span data-ttu-id="a97e7-129">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="a97e7-129">Specifies the offset for the search results.</span></span> <span data-ttu-id="a97e7-130">偏移量0返回的第一个结果。</span><span class="sxs-lookup"><span data-stu-id="a97e7-130">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="a97e7-131">查询</span><span class="sxs-lookup"><span data-stu-id="a97e7-131">query</span></span>|[<span data-ttu-id="a97e7-132">searchQuery</span><span class="sxs-lookup"><span data-stu-id="a97e7-132">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="a97e7-133">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="a97e7-133">Contains the query terms.</span></span>|
|<span data-ttu-id="a97e7-134">大小</span><span class="sxs-lookup"><span data-stu-id="a97e7-134">size</span></span>|<span data-ttu-id="a97e7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a97e7-135">Int32</span></span>|<span data-ttu-id="a97e7-136">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="a97e7-136">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a97e7-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a97e7-137">JSON representation</span></span>

<span data-ttu-id="a97e7-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a97e7-138">The following is a JSON representation of the resource.</span></span>

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
