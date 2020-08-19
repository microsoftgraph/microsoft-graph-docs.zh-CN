---
title: 诊断资源类型
description: 有关 OneNote 操作的错误或警告的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: b6cad8680b00b935dbaac817d53d930b5046e265
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809108"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="075f1-103">诊断资源类型</span><span class="sxs-lookup"><span data-stu-id="075f1-103">diagnostic resource type</span></span>

<span data-ttu-id="075f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="075f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="075f1-105">有关 OneNote 操作的错误或警告的信息。</span><span class="sxs-lookup"><span data-stu-id="075f1-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="075f1-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="075f1-106">JSON representation</span></span>

<span data-ttu-id="075f1-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="075f1-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="075f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="075f1-108">Properties</span></span>
| <span data-ttu-id="075f1-109">属性</span><span class="sxs-lookup"><span data-stu-id="075f1-109">Property</span></span>     | <span data-ttu-id="075f1-110">类型</span><span class="sxs-lookup"><span data-stu-id="075f1-110">Type</span></span>   |<span data-ttu-id="075f1-111">描述</span><span class="sxs-lookup"><span data-stu-id="075f1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="075f1-112">message</span><span class="sxs-lookup"><span data-stu-id="075f1-112">message</span></span>|<span data-ttu-id="075f1-113">String</span><span class="sxs-lookup"><span data-stu-id="075f1-113">String</span></span>|<span data-ttu-id="075f1-114">描述触发错误或警告的条件的消息。</span><span class="sxs-lookup"><span data-stu-id="075f1-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="075f1-115">url</span><span class="sxs-lookup"><span data-stu-id="075f1-115">url</span></span>|<span data-ttu-id="075f1-116">String</span><span class="sxs-lookup"><span data-stu-id="075f1-116">String</span></span>|<span data-ttu-id="075f1-117">有关此问题的文档的链接。</span><span class="sxs-lookup"><span data-stu-id="075f1-117">The link to the documentation for this issue.</span></span>|

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
