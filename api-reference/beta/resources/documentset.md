---
author: swapnil1993
title: documentSet 资源类型
description: 包含有关文档集设置的元数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 25a2b5e71c76a8a097ff9c490313ae6d319abeb8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446160"
---
# <a name="documentset-resource-type"></a><span data-ttu-id="17eee-103">documentSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="17eee-103">documentSet resource type</span></span>

<span data-ttu-id="17eee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17eee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="17eee-105">包含有关文档集设置的元数据。</span><span class="sxs-lookup"><span data-stu-id="17eee-105">Contains metadata about document set settings.</span></span>

## <a name="properties"></a><span data-ttu-id="17eee-106">属性</span><span class="sxs-lookup"><span data-stu-id="17eee-106">Properties</span></span>

| <span data-ttu-id="17eee-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="17eee-107">Property name</span></span>  | <span data-ttu-id="17eee-108">类型</span><span class="sxs-lookup"><span data-stu-id="17eee-108">Type</span></span>    | <span data-ttu-id="17eee-109">说明</span><span class="sxs-lookup"><span data-stu-id="17eee-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="17eee-110">shouldPrefixNameToFile</span><span class="sxs-lookup"><span data-stu-id="17eee-110">shouldPrefixNameToFile</span></span> | <span data-ttu-id="17eee-111">布尔</span><span class="sxs-lookup"><span data-stu-id="17eee-111">Boolean</span></span>  | <span data-ttu-id="17eee-112">将文档集的名称添加到每个文件名。</span><span class="sxs-lookup"><span data-stu-id="17eee-112">Add the name of the Document Set to each file name.</span></span>
| <span data-ttu-id="17eee-113">allowedContentTypes</span><span class="sxs-lookup"><span data-stu-id="17eee-113">allowedContentTypes</span></span> | <span data-ttu-id="17eee-114">collection (microsoft.graph.contentTypeInfo) </span><span class="sxs-lookup"><span data-stu-id="17eee-114">Collection(microsoft.graph.contentTypeInfo)</span></span> | <span data-ttu-id="17eee-115">文档集允许的内容类型。</span><span class="sxs-lookup"><span data-stu-id="17eee-115">Content types allowed in document set.</span></span>
| <span data-ttu-id="17eee-116">defaultContents</span><span class="sxs-lookup"><span data-stu-id="17eee-116">defaultContents</span></span>     | <span data-ttu-id="17eee-117">集合 (microsoft.graph.documentSetContent) </span><span class="sxs-lookup"><span data-stu-id="17eee-117">Collection(microsoft.graph.documentSetContent)</span></span> | <span data-ttu-id="17eee-118">文档集的默认内容。</span><span class="sxs-lookup"><span data-stu-id="17eee-118">Default contents of document set.</span></span>  
| <span data-ttu-id="17eee-119">propagateWelcomePageChanges</span><span class="sxs-lookup"><span data-stu-id="17eee-119">propagateWelcomePageChanges</span></span> | <span data-ttu-id="17eee-120">布尔</span><span class="sxs-lookup"><span data-stu-id="17eee-120">Boolean</span></span> | <span data-ttu-id="17eee-121">指定是否将欢迎页面更改推送到继承的内容类型。</span><span class="sxs-lookup"><span data-stu-id="17eee-121">Specifies whether to push welcome page changes to inherited content types.</span></span>  
| <span data-ttu-id="17eee-122">sharedColumns</span><span class="sxs-lookup"><span data-stu-id="17eee-122">sharedColumns</span></span>       | <span data-ttu-id="17eee-123">集合 (microsoft.graph.columnDefinition) </span><span class="sxs-lookup"><span data-stu-id="17eee-123">Collection(microsoft.graph.columnDefinition)</span></span> | <span data-ttu-id="17eee-124">在同步到文档集内所有文档的文档集上编辑的列。</span><span class="sxs-lookup"><span data-stu-id="17eee-124">Columns edited on the document set that synchronize to all documents in the set.</span></span> <span data-ttu-id="17eee-125">这些文档本身是只读的。</span><span class="sxs-lookup"><span data-stu-id="17eee-125">These are read-only on the documents themselves.</span></span> 
| <span data-ttu-id="17eee-126">welcomePageColumns</span><span class="sxs-lookup"><span data-stu-id="17eee-126">welcomePageColumns</span></span>  | <span data-ttu-id="17eee-127">集合 (microsoft.graph.columnDefinition) </span><span class="sxs-lookup"><span data-stu-id="17eee-127">Collection(microsoft.graph.columnDefinition)</span></span>  | <span data-ttu-id="17eee-128">指定要显示在文档集的欢迎页上的列。</span><span class="sxs-lookup"><span data-stu-id="17eee-128">Specifies columns to show on the welcome page for the document set.</span></span>  
| <span data-ttu-id="17eee-129">welcomePageUrl</span><span class="sxs-lookup"><span data-stu-id="17eee-129">welcomePageUrl</span></span>      | <span data-ttu-id="17eee-130">string</span><span class="sxs-lookup"><span data-stu-id="17eee-130">string</span></span> | <span data-ttu-id="17eee-131">欢迎页面绝对 URL。</span><span class="sxs-lookup"><span data-stu-id="17eee-131">Welcome page absolute URL.</span></span>  

## <a name="json-representation"></a><span data-ttu-id="17eee-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17eee-132">JSON representation</span></span>

<span data-ttu-id="17eee-133">下面是 **documentSet** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17eee-133">The following is a JSON representation of a **documentSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "sharedColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
