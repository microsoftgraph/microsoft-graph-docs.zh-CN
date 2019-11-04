---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ad65d0a9a3bed59bcb630082807004a7ca89ba5f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938995"
---
# <a name="addin-resource-type"></a><span data-ttu-id="b70cd-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="b70cd-103">addIn resource type</span></span>

<span data-ttu-id="b70cd-104">定义使用服务可用于调用特定上下文中的应用程序的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="b70cd-104">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="b70cd-105">例如，可以呈现文件流的应用程序[可能会](https://docs.microsoft.com/en-us/onedrive/developer/file-handlers/?view=odsp-graph-online)为其 "FileHandler" 功能配置 addIns。</span><span class="sxs-lookup"><span data-stu-id="b70cd-105">For example, applications that can render file streams [may configure addIns](https://docs.microsoft.com/en-us/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="b70cd-106">这将允许 Office 365 等服务在用户正在使用的文档的上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="b70cd-106">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="b70cd-107">属性</span><span class="sxs-lookup"><span data-stu-id="b70cd-107">Properties</span></span>
| <span data-ttu-id="b70cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="b70cd-108">Property</span></span>     | <span data-ttu-id="b70cd-109">类型</span><span class="sxs-lookup"><span data-stu-id="b70cd-109">Type</span></span>   |<span data-ttu-id="b70cd-110">说明</span><span class="sxs-lookup"><span data-stu-id="b70cd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b70cd-111">id</span><span class="sxs-lookup"><span data-stu-id="b70cd-111">id</span></span>|<span data-ttu-id="b70cd-112">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="b70cd-112">guid</span></span>||
|<span data-ttu-id="b70cd-113">properties</span><span class="sxs-lookup"><span data-stu-id="b70cd-113">properties</span></span>|<span data-ttu-id="b70cd-114">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b70cd-114">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="b70cd-115">类型</span><span class="sxs-lookup"><span data-stu-id="b70cd-115">type</span></span>|<span data-ttu-id="b70cd-116">string</span><span class="sxs-lookup"><span data-stu-id="b70cd-116">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="b70cd-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b70cd-117">JSON representation</span></span>

<span data-ttu-id="b70cd-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b70cd-118">Here is a JSON representation of the resource.</span></span>

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
