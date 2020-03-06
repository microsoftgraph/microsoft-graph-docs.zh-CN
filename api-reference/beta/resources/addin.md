---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a5f0d078bf73603ccedf905c2cd496223fbd426e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508413"
---
# <a name="addin-resource-type"></a><span data-ttu-id="fb390-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb390-103">addIn resource type</span></span>

<span data-ttu-id="fb390-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb390-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb390-105">定义使用服务可用于调用特定上下文中的应用的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="fb390-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="fb390-106">例如，可以呈现文件流的应用程序[可能会配置](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online)文件处理程序功能的外接程序。</span><span class="sxs-lookup"><span data-stu-id="fb390-106">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="fb390-107">这将使 Office 365 之类的服务在用户正在处理的文档上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="fb390-107">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="fb390-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb390-108">Properties</span></span>
| <span data-ttu-id="fb390-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb390-109">Property</span></span>     | <span data-ttu-id="fb390-110">类型</span><span class="sxs-lookup"><span data-stu-id="fb390-110">Type</span></span>   |<span data-ttu-id="fb390-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb390-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb390-112">id</span><span class="sxs-lookup"><span data-stu-id="fb390-112">id</span></span>|<span data-ttu-id="fb390-113">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="fb390-113">guid</span></span>||
|<span data-ttu-id="fb390-114">properties</span><span class="sxs-lookup"><span data-stu-id="fb390-114">properties</span></span>|<span data-ttu-id="fb390-115">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb390-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="fb390-116">类型</span><span class="sxs-lookup"><span data-stu-id="fb390-116">type</span></span>|<span data-ttu-id="fb390-117">string</span><span class="sxs-lookup"><span data-stu-id="fb390-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="fb390-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb390-118">JSON representation</span></span>

<span data-ttu-id="fb390-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb390-119">Here is a JSON representation of the resource.</span></span>

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
