---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 124ea40d7d10c3104ef98634c1af4ea40038c211
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461919"
---
# <a name="addin-resource-type"></a><span data-ttu-id="a2a6c-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2a6c-103">addIn resource type</span></span>

<span data-ttu-id="a2a6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a6c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2a6c-105">定义使用服务可用于调用特定上下文中的应用的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="a2a6c-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="a2a6c-106">例如，可以呈现文件流的应用程序[可能会](/onedrive/developer/file-handlers/?view=odsp-graph-online)为其 "FileHandler" 功能配置 addIns。</span><span class="sxs-lookup"><span data-stu-id="a2a6c-106">For example, applications that can render file streams [may configure addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="a2a6c-107">这将使 Office 365 之类的服务在用户正在处理的文档上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="a2a6c-107">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="a2a6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2a6c-108">Properties</span></span>
| <span data-ttu-id="a2a6c-109">属性</span><span class="sxs-lookup"><span data-stu-id="a2a6c-109">Property</span></span>     | <span data-ttu-id="a2a6c-110">类型</span><span class="sxs-lookup"><span data-stu-id="a2a6c-110">Type</span></span>   |<span data-ttu-id="a2a6c-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2a6c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2a6c-112">id</span><span class="sxs-lookup"><span data-stu-id="a2a6c-112">id</span></span>|<span data-ttu-id="a2a6c-113">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="a2a6c-113">guid</span></span>||
|<span data-ttu-id="a2a6c-114">properties</span><span class="sxs-lookup"><span data-stu-id="a2a6c-114">properties</span></span>|<span data-ttu-id="a2a6c-115">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2a6c-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="a2a6c-116">类型</span><span class="sxs-lookup"><span data-stu-id="a2a6c-116">type</span></span>|<span data-ttu-id="a2a6c-117">string</span><span class="sxs-lookup"><span data-stu-id="a2a6c-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="a2a6c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2a6c-118">JSON representation</span></span>

<span data-ttu-id="a2a6c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2a6c-119">Here is a JSON representation of the resource.</span></span>

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
