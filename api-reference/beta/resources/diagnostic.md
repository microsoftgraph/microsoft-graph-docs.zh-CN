---
title: 诊断资源类型
description: 有关 OneNote 操作的错误或警告的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f0d5e6a938c454ca2efeda0dd7628c15269d6311
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507238"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="b0d08-103">诊断资源类型</span><span class="sxs-lookup"><span data-stu-id="b0d08-103">diagnostic resource type</span></span>

<span data-ttu-id="b0d08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0d08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0d08-105">有关 OneNote 操作的错误或警告的信息。</span><span class="sxs-lookup"><span data-stu-id="b0d08-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0d08-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0d08-106">JSON representation</span></span>

<span data-ttu-id="b0d08-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0d08-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b0d08-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0d08-108">Properties</span></span>
| <span data-ttu-id="b0d08-109">属性</span><span class="sxs-lookup"><span data-stu-id="b0d08-109">Property</span></span>     | <span data-ttu-id="b0d08-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0d08-110">Type</span></span>   |<span data-ttu-id="b0d08-111">描述</span><span class="sxs-lookup"><span data-stu-id="b0d08-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0d08-112">message</span><span class="sxs-lookup"><span data-stu-id="b0d08-112">message</span></span>|<span data-ttu-id="b0d08-113">String</span><span class="sxs-lookup"><span data-stu-id="b0d08-113">String</span></span>|<span data-ttu-id="b0d08-114">描述触发错误或警告的条件的消息。</span><span class="sxs-lookup"><span data-stu-id="b0d08-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="b0d08-115">url</span><span class="sxs-lookup"><span data-stu-id="b0d08-115">url</span></span>|<span data-ttu-id="b0d08-116">String</span><span class="sxs-lookup"><span data-stu-id="b0d08-116">String</span></span>|<span data-ttu-id="b0d08-117">有关此问题的文档的链接。</span><span class="sxs-lookup"><span data-stu-id="b0d08-117">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
