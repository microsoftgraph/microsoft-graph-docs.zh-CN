---
author: swapnil1993
title: documentSetContent 资源类型
description: documentSetContent 资源包含有关存在于内容的默认内容位置中的文件的元数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8597dfb8a762d2166a9253fb4e806b9c2fcf5223
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446161"
---
# <a name="documentsetcontent-resource-type"></a><span data-ttu-id="1a79b-103">documentSetContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a79b-103">documentSetContent resource type</span></span>

<span data-ttu-id="1a79b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a79b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="1a79b-105">包含有关存在于内容类型的默认内容位置中的文件的元数据。</span><span class="sxs-lookup"><span data-stu-id="1a79b-105">Contains metadata about a file present in default content location of a content type.</span></span>

## <a name="properties"></a><span data-ttu-id="1a79b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a79b-106">Properties</span></span>

| <span data-ttu-id="1a79b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="1a79b-107">Property name</span></span>  | <span data-ttu-id="1a79b-108">类型</span><span class="sxs-lookup"><span data-stu-id="1a79b-108">Type</span></span>    | <span data-ttu-id="1a79b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1a79b-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="1a79b-110">contentType</span><span class="sxs-lookup"><span data-stu-id="1a79b-110">contentType</span></span>    | <span data-ttu-id="1a79b-111">microsoft.graph.contentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="1a79b-111">microsoft.graph.contentTypeInfo</span></span> | <span data-ttu-id="1a79b-112">文件的内容类型信息。</span><span class="sxs-lookup"><span data-stu-id="1a79b-112">Content type information of the file.</span></span> 
| <span data-ttu-id="1a79b-113">fileName</span><span class="sxs-lookup"><span data-stu-id="1a79b-113">fileName</span></span>      | <span data-ttu-id="1a79b-114">string</span><span class="sxs-lookup"><span data-stu-id="1a79b-114">string</span></span>  | <span data-ttu-id="1a79b-115">资源文件夹中应添加为默认内容或文档集模板的文件的名称</span><span class="sxs-lookup"><span data-stu-id="1a79b-115">Name of the file in resource folder that should be added as a default content or a template in the document set</span></span>  
| <span data-ttu-id="1a79b-116">folderName</span><span class="sxs-lookup"><span data-stu-id="1a79b-116">folderName</span></span>         | <span data-ttu-id="1a79b-117">string</span><span class="sxs-lookup"><span data-stu-id="1a79b-117">string</span></span>  | <span data-ttu-id="1a79b-118">在库中新建文档集时将放置文件的文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="1a79b-118">Folder name in which the file will be placed when a new document set is created in the library.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a79b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a79b-119">JSON representation</span></span>

<span data-ttu-id="1a79b-120">下面是 **documentSetContent** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a79b-120">Here is a JSON representation of a **documentSetContent** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```