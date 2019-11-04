---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 26a224989af3ab87036fbd6bd0964ea811016dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939093"
---
# <a name="addin-resource-type"></a><span data-ttu-id="56e2d-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="56e2d-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e2d-104">定义使用服务可用于调用特定上下文中的应用程序的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="56e2d-104">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="56e2d-105">例如，可以呈现文件流的应用程序[可能会配置](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online)文件处理程序功能的外接程序。</span><span class="sxs-lookup"><span data-stu-id="56e2d-105">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="56e2d-106">这将允许 Office 365 等服务在用户正在使用的文档的上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="56e2d-106">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="56e2d-107">属性</span><span class="sxs-lookup"><span data-stu-id="56e2d-107">Properties</span></span>
| <span data-ttu-id="56e2d-108">属性</span><span class="sxs-lookup"><span data-stu-id="56e2d-108">Property</span></span>     | <span data-ttu-id="56e2d-109">类型</span><span class="sxs-lookup"><span data-stu-id="56e2d-109">Type</span></span>   |<span data-ttu-id="56e2d-110">说明</span><span class="sxs-lookup"><span data-stu-id="56e2d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56e2d-111">id</span><span class="sxs-lookup"><span data-stu-id="56e2d-111">id</span></span>|<span data-ttu-id="56e2d-112">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="56e2d-112">guid</span></span>||
|<span data-ttu-id="56e2d-113">properties</span><span class="sxs-lookup"><span data-stu-id="56e2d-113">properties</span></span>|<span data-ttu-id="56e2d-114">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56e2d-114">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="56e2d-115">类型</span><span class="sxs-lookup"><span data-stu-id="56e2d-115">type</span></span>|<span data-ttu-id="56e2d-116">string</span><span class="sxs-lookup"><span data-stu-id="56e2d-116">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="56e2d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56e2d-117">JSON representation</span></span>

<span data-ttu-id="56e2d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56e2d-118">Here is a JSON representation of the resource.</span></span>

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
