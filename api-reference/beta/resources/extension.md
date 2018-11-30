---
title: 扩展资源类型
description: 用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。
ms.openlocfilehash: b67c347e44c875ca550465be46eecdff3f845eef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042517"
---
# <a name="extension-resource-type"></a><span data-ttu-id="04e0d-103">扩展资源类型</span><span class="sxs-lookup"><span data-stu-id="04e0d-103">extension resource type</span></span>

> <span data-ttu-id="04e0d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04e0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04e0d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04e0d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04e0d-106">用以支持 OData v4 开放类型 [openTypeExtension](opentypeextension.md) 的抽象类型。</span><span class="sxs-lookup"><span data-stu-id="04e0d-106">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="04e0d-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04e0d-107">JSON representation</span></span>

<span data-ttu-id="04e0d-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04e0d-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="04e0d-109">属性</span><span class="sxs-lookup"><span data-stu-id="04e0d-109">Properties</span></span>
| <span data-ttu-id="04e0d-110">属性</span><span class="sxs-lookup"><span data-stu-id="04e0d-110">Property</span></span>     | <span data-ttu-id="04e0d-111">类型</span><span class="sxs-lookup"><span data-stu-id="04e0d-111">Type</span></span>   |<span data-ttu-id="04e0d-112">说明</span><span class="sxs-lookup"><span data-stu-id="04e0d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04e0d-113">id</span><span class="sxs-lookup"><span data-stu-id="04e0d-113">id</span></span>|<span data-ttu-id="04e0d-114">String</span><span class="sxs-lookup"><span data-stu-id="04e0d-114">String</span></span>| <span data-ttu-id="04e0d-115">只读。</span><span class="sxs-lookup"><span data-stu-id="04e0d-115">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04e0d-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="04e0d-116">Relationships</span></span>
<span data-ttu-id="04e0d-117">无</span><span class="sxs-lookup"><span data-stu-id="04e0d-117">None</span></span>


## <a name="methods"></a><span data-ttu-id="04e0d-118">方法</span><span class="sxs-lookup"><span data-stu-id="04e0d-118">Methods</span></span>

<span data-ttu-id="04e0d-119">请参阅派生类型 [openTypeExtension](opentypeextension.md) 的方法以了解实际支持的方法。</span><span class="sxs-lookup"><span data-stu-id="04e0d-119">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->