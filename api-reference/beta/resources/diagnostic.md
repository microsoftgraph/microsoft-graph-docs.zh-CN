---
title: 诊断资源类型
description: 有关错误或警告 OneNote 操作的信息。
localization_priority: Normal
ms.openlocfilehash: 28cdd1c07bab0494a69cfb7ce6a5284238e1ff19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845988"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="67663-103">诊断资源类型</span><span class="sxs-lookup"><span data-stu-id="67663-103">diagnostic resource type</span></span>

> <span data-ttu-id="67663-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="67663-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67663-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67663-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67663-106">有关错误或警告 OneNote 操作的信息。</span><span class="sxs-lookup"><span data-stu-id="67663-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67663-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67663-107">JSON representation</span></span>

<span data-ttu-id="67663-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67663-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="67663-109">属性</span><span class="sxs-lookup"><span data-stu-id="67663-109">Properties</span></span>
| <span data-ttu-id="67663-110">属性</span><span class="sxs-lookup"><span data-stu-id="67663-110">Property</span></span>     | <span data-ttu-id="67663-111">类型</span><span class="sxs-lookup"><span data-stu-id="67663-111">Type</span></span>   |<span data-ttu-id="67663-112">Description</span><span class="sxs-lookup"><span data-stu-id="67663-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67663-113">message</span><span class="sxs-lookup"><span data-stu-id="67663-113">message</span></span>|<span data-ttu-id="67663-114">字符串</span><span class="sxs-lookup"><span data-stu-id="67663-114">String</span></span>|<span data-ttu-id="67663-115">描述触发错误或警告的条件的消息。</span><span class="sxs-lookup"><span data-stu-id="67663-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="67663-116">url</span><span class="sxs-lookup"><span data-stu-id="67663-116">url</span></span>|<span data-ttu-id="67663-117">String</span><span class="sxs-lookup"><span data-stu-id="67663-117">String</span></span>|<span data-ttu-id="67663-118">指向此问题的文档的链接。</span><span class="sxs-lookup"><span data-stu-id="67663-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
