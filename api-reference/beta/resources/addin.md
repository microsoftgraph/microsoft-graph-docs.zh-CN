---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80c9e3c31a3bcc0d7b74e24373e5d1bb6947840f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134055"
---
# <a name="addin-resource-type"></a><span data-ttu-id="44926-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="44926-103">addIn resource type</span></span>

<span data-ttu-id="44926-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44926-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44926-105">定义使用服务可用于调用特定上下文中的应用的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="44926-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="44926-106">例如，可以呈现文件 [流的应用程序可能会](/onedrive/developer/file-handlers/?view=odsp-graph-online) 为文件处理程序功能配置外接程序。</span><span class="sxs-lookup"><span data-stu-id="44926-106">For example, applications that can render file streams [might configure add-ins](/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="44926-107">这将使 Microsoft 365 之类的服务在用户正在处理的文档上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="44926-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="44926-108">属性</span><span class="sxs-lookup"><span data-stu-id="44926-108">Properties</span></span>
| <span data-ttu-id="44926-109">属性</span><span class="sxs-lookup"><span data-stu-id="44926-109">Property</span></span>     | <span data-ttu-id="44926-110">类型</span><span class="sxs-lookup"><span data-stu-id="44926-110">Type</span></span>   |<span data-ttu-id="44926-111">说明</span><span class="sxs-lookup"><span data-stu-id="44926-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44926-112">id</span><span class="sxs-lookup"><span data-stu-id="44926-112">id</span></span>|<span data-ttu-id="44926-113">guid</span><span class="sxs-lookup"><span data-stu-id="44926-113">guid</span></span>||
|<span data-ttu-id="44926-114">properties</span><span class="sxs-lookup"><span data-stu-id="44926-114">properties</span></span>|<span data-ttu-id="44926-115">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="44926-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="44926-116">类型</span><span class="sxs-lookup"><span data-stu-id="44926-116">type</span></span>|<span data-ttu-id="44926-117">string</span><span class="sxs-lookup"><span data-stu-id="44926-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="44926-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44926-118">JSON representation</span></span>

<span data-ttu-id="44926-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44926-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
