---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: f9802b592cb3412fec61b0d8e8dea4e4cf0b7bae
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897923"
---
# <a name="addin-resource-type"></a><span data-ttu-id="68f1b-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="68f1b-103">addIn resource type</span></span>

<span data-ttu-id="68f1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68f1b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68f1b-105">定义使用服务可用于调用特定上下文中的应用的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="68f1b-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="68f1b-106">例如，可以呈现文件流的应用程序[可能会](/onedrive/developer/file-handlers/?view=odsp-graph-online)为其 "FileHandler" 功能配置 addIns。</span><span class="sxs-lookup"><span data-stu-id="68f1b-106">For example, applications that can render file streams [may configure addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="68f1b-107">这将使 Microsoft 365 等服务能够在用户正在使用的文档的上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="68f1b-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="68f1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="68f1b-108">Properties</span></span>
| <span data-ttu-id="68f1b-109">属性</span><span class="sxs-lookup"><span data-stu-id="68f1b-109">Property</span></span>     | <span data-ttu-id="68f1b-110">类型</span><span class="sxs-lookup"><span data-stu-id="68f1b-110">Type</span></span>   |<span data-ttu-id="68f1b-111">说明</span><span class="sxs-lookup"><span data-stu-id="68f1b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68f1b-112">id</span><span class="sxs-lookup"><span data-stu-id="68f1b-112">id</span></span>|<span data-ttu-id="68f1b-113">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="68f1b-113">guid</span></span>||
|<span data-ttu-id="68f1b-114">properties</span><span class="sxs-lookup"><span data-stu-id="68f1b-114">properties</span></span>|<span data-ttu-id="68f1b-115">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68f1b-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="68f1b-116">类型</span><span class="sxs-lookup"><span data-stu-id="68f1b-116">type</span></span>|<span data-ttu-id="68f1b-117">string</span><span class="sxs-lookup"><span data-stu-id="68f1b-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="68f1b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68f1b-118">JSON representation</span></span>

<span data-ttu-id="68f1b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68f1b-119">Here is a JSON representation of the resource.</span></span>

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
