---
author: nilakhan
description: 表示打印文档上载的信息
title: printDocumentUploadProperties 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: universal-print
ms.openlocfilehash: 1249eaae4d62cffe14935587c655ba402237b0ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727967"
---
# <a name="printdocumentuploadproperties-resource-type"></a><span data-ttu-id="83784-103">printDocumentUploadProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="83784-103">printDocumentUploadProperties resource type</span></span>

<span data-ttu-id="83784-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83784-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83784-105">描述要上载的文档</span><span class="sxs-lookup"><span data-stu-id="83784-105">Describes the document that is being uploaded</span></span>

## <a name="json-representation"></a><span data-ttu-id="83784-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83784-106">JSON representation</span></span>

<span data-ttu-id="83784-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83784-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.printDocumentUploadProperties",
  "baseType": null
}-->

```json
{
  "contentType": "String",
  "documentName": "String",
  "size": "Int64",
}
```

## <a name="properties"></a><span data-ttu-id="83784-108">属性</span><span class="sxs-lookup"><span data-stu-id="83784-108">Properties</span></span>


| <span data-ttu-id="83784-109">属性</span><span class="sxs-lookup"><span data-stu-id="83784-109">Property</span></span>       | <span data-ttu-id="83784-110">类型</span><span class="sxs-lookup"><span data-stu-id="83784-110">Type</span></span>              |<span data-ttu-id="83784-111">说明</span><span class="sxs-lookup"><span data-stu-id="83784-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="83784-112">contentType</span><span class="sxs-lookup"><span data-stu-id="83784-112">contentType</span></span> | <span data-ttu-id="83784-113">String</span><span class="sxs-lookup"><span data-stu-id="83784-113">String</span></span>    | <span data-ttu-id="83784-114">文档的内容 (MIME) 类型。</span><span class="sxs-lookup"><span data-stu-id="83784-114">The document's content (MIME) type.</span></span>
| <span data-ttu-id="83784-115">documentName</span><span class="sxs-lookup"><span data-stu-id="83784-115">documentName</span></span> | <span data-ttu-id="83784-116">String</span><span class="sxs-lookup"><span data-stu-id="83784-116">String</span></span> | <span data-ttu-id="83784-117">文档的名称。</span><span class="sxs-lookup"><span data-stu-id="83784-117">The document's name.</span></span>
| <span data-ttu-id="83784-118">size</span><span class="sxs-lookup"><span data-stu-id="83784-118">size</span></span>          | <span data-ttu-id="83784-119">Int64</span><span class="sxs-lookup"><span data-stu-id="83784-119">Int64</span></span>            | <span data-ttu-id="83784-120">文档的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="83784-120">The document's size in bytes.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "printDocumentUploadProperties",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
