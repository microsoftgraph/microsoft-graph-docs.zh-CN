---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 22efb3e00689daad5c914d770a7cd0d41b3e35b7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939129"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="1e78b-104">searchRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e78b-104">searchRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e78b-105">要发送到查询终结点的搜索请求。</span><span class="sxs-lookup"><span data-stu-id="1e78b-105">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="1e78b-106">它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。</span><span class="sxs-lookup"><span data-stu-id="1e78b-106">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

## <a name="properties"></a><span data-ttu-id="1e78b-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e78b-107">Properties</span></span>

| <span data-ttu-id="1e78b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e78b-108">Property</span></span>     | <span data-ttu-id="1e78b-109">类型</span><span class="sxs-lookup"><span data-stu-id="1e78b-109">Type</span></span>        | <span data-ttu-id="1e78b-110">描述</span><span class="sxs-lookup"><span data-stu-id="1e78b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e78b-111">stored_fields</span><span class="sxs-lookup"><span data-stu-id="1e78b-111">stored_fields</span></span>|<span data-ttu-id="1e78b-112">String collection</span><span class="sxs-lookup"><span data-stu-id="1e78b-112">String collection</span></span> |<span data-ttu-id="1e78b-113">包含要为搜索 _so urces 对象返回的字段。</span><span class="sxs-lookup"><span data-stu-id="1e78b-113">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="1e78b-114">注释仅当在响应中指定了`externalItem` entityType = 时，这才适用。</span><span class="sxs-lookup"><span data-stu-id="1e78b-114">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="1e78b-115">contentSources</span><span class="sxs-lookup"><span data-stu-id="1e78b-115">contentSources</span></span>|<span data-ttu-id="1e78b-116">String collection</span><span class="sxs-lookup"><span data-stu-id="1e78b-116">String collection</span></span>|<span data-ttu-id="1e78b-117">包含要设定的连接。</span><span class="sxs-lookup"><span data-stu-id="1e78b-117">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="1e78b-118">遵循以下格式：在`/external/connections/connectionid`连接器`connectionid`管理中定义 ConnectionId 的位置。</span><span class="sxs-lookup"><span data-stu-id="1e78b-118">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="1e78b-119">注释 contentSource 仅当 entityType =`externalItem`时适用。</span><span class="sxs-lookup"><span data-stu-id="1e78b-119">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="1e78b-120">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="1e78b-120">enableTopResults</span></span>|<span data-ttu-id="1e78b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e78b-121">Boolean</span></span>|<span data-ttu-id="1e78b-122">这将触发邮件的混合排序：前3个邮件最相关</span><span class="sxs-lookup"><span data-stu-id="1e78b-122">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="1e78b-123">这仅适用于 entityType =`message`。</span><span class="sxs-lookup"><span data-stu-id="1e78b-123">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="1e78b-124">entityTypes</span><span class="sxs-lookup"><span data-stu-id="1e78b-124">entityTypes</span></span>|<span data-ttu-id="1e78b-125">`entityType` 集合</span><span class="sxs-lookup"><span data-stu-id="1e78b-125">`entityType` collection</span></span>| <span data-ttu-id="1e78b-126">可取值为：`event`、`message`、`driveItem`、`externalFile`、`externalItem`。</span><span class="sxs-lookup"><span data-stu-id="1e78b-126">Possible values are: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span></span>|
|<span data-ttu-id="1e78b-127">发件人</span><span class="sxs-lookup"><span data-stu-id="1e78b-127">from</span></span>|<span data-ttu-id="1e78b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1e78b-128">Int32</span></span>|<span data-ttu-id="1e78b-129">指定搜索结果的偏移量。</span><span class="sxs-lookup"><span data-stu-id="1e78b-129">Specifies the offset for the search results.</span></span> <span data-ttu-id="1e78b-130">偏移量0返回的第一个结果。</span><span class="sxs-lookup"><span data-stu-id="1e78b-130">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="1e78b-131">查询</span><span class="sxs-lookup"><span data-stu-id="1e78b-131">query</span></span>|[<span data-ttu-id="1e78b-132">searchQuery</span><span class="sxs-lookup"><span data-stu-id="1e78b-132">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="1e78b-133">包含查询词。</span><span class="sxs-lookup"><span data-stu-id="1e78b-133">Contains the query terms.</span></span>|
|<span data-ttu-id="1e78b-134">大小</span><span class="sxs-lookup"><span data-stu-id="1e78b-134">size</span></span>|<span data-ttu-id="1e78b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1e78b-135">Int32</span></span>|<span data-ttu-id="1e78b-136">要检索的页面的大小。</span><span class="sxs-lookup"><span data-stu-id="1e78b-136">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e78b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e78b-137">JSON representation</span></span>

<span data-ttu-id="1e78b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e78b-138">The following is a JSON representation of the resource.</span></span>

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
