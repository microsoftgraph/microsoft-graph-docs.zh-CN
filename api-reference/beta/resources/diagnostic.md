---
title: 诊断资源类型
description: 有关错误或警告 OneNote 操作的信息。
ms.openlocfilehash: 29e30d44a9fde91b79778042be19461b880216ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047282"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="8ced9-103">诊断资源类型</span><span class="sxs-lookup"><span data-stu-id="8ced9-103">diagnostic resource type</span></span>

> <span data-ttu-id="8ced9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8ced9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ced9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8ced9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ced9-106">有关错误或警告 OneNote 操作的信息。</span><span class="sxs-lookup"><span data-stu-id="8ced9-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ced9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ced9-107">JSON representation</span></span>

<span data-ttu-id="8ced9-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ced9-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8ced9-109">属性</span><span class="sxs-lookup"><span data-stu-id="8ced9-109">Properties</span></span>
| <span data-ttu-id="8ced9-110">属性</span><span class="sxs-lookup"><span data-stu-id="8ced9-110">Property</span></span>     | <span data-ttu-id="8ced9-111">类型</span><span class="sxs-lookup"><span data-stu-id="8ced9-111">Type</span></span>   |<span data-ttu-id="8ced9-112">说明</span><span class="sxs-lookup"><span data-stu-id="8ced9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ced9-113">message</span><span class="sxs-lookup"><span data-stu-id="8ced9-113">message</span></span>|<span data-ttu-id="8ced9-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8ced9-114">String</span></span>|<span data-ttu-id="8ced9-115">描述触发错误或警告的条件的消息。</span><span class="sxs-lookup"><span data-stu-id="8ced9-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="8ced9-116">url</span><span class="sxs-lookup"><span data-stu-id="8ced9-116">url</span></span>|<span data-ttu-id="8ced9-117">String</span><span class="sxs-lookup"><span data-stu-id="8ced9-117">String</span></span>|<span data-ttu-id="8ced9-118">指向此问题的文档的链接。</span><span class="sxs-lookup"><span data-stu-id="8ced9-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->