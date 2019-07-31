---
title: 诊断资源类型
description: 有关 OneNote 操作的错误或警告的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4ac591640e647a1caa5230bd8e7e8c64ad2314af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973141"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="1ab9e-103">诊断资源类型</span><span class="sxs-lookup"><span data-stu-id="1ab9e-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ab9e-104">有关 OneNote 操作的错误或警告的信息。</span><span class="sxs-lookup"><span data-stu-id="1ab9e-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ab9e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ab9e-105">JSON representation</span></span>

<span data-ttu-id="1ab9e-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ab9e-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1ab9e-107">属性</span><span class="sxs-lookup"><span data-stu-id="1ab9e-107">Properties</span></span>
| <span data-ttu-id="1ab9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ab9e-108">Property</span></span>     | <span data-ttu-id="1ab9e-109">类型</span><span class="sxs-lookup"><span data-stu-id="1ab9e-109">Type</span></span>   |<span data-ttu-id="1ab9e-110">描述</span><span class="sxs-lookup"><span data-stu-id="1ab9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ab9e-111">message</span><span class="sxs-lookup"><span data-stu-id="1ab9e-111">message</span></span>|<span data-ttu-id="1ab9e-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1ab9e-112">String</span></span>|<span data-ttu-id="1ab9e-113">描述触发错误或警告的条件的消息。</span><span class="sxs-lookup"><span data-stu-id="1ab9e-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="1ab9e-114">url</span><span class="sxs-lookup"><span data-stu-id="1ab9e-114">url</span></span>|<span data-ttu-id="1ab9e-115">String</span><span class="sxs-lookup"><span data-stu-id="1ab9e-115">String</span></span>|<span data-ttu-id="1ab9e-116">有关此问题的文档的链接。</span><span class="sxs-lookup"><span data-stu-id="1ab9e-116">The link to the documentation for this issue.</span></span>|

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
