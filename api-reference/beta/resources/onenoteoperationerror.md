---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8b2912ee02ab22631224b892a09a8c4dd7840dd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341414"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="04811-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="04811-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04811-104">失败的 OneNote 操作中的错误。</span><span class="sxs-lookup"><span data-stu-id="04811-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04811-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04811-105">JSON representation</span></span>

<span data-ttu-id="04811-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04811-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="04811-107">属性</span><span class="sxs-lookup"><span data-stu-id="04811-107">Properties</span></span>
| <span data-ttu-id="04811-108">属性</span><span class="sxs-lookup"><span data-stu-id="04811-108">Property</span></span>     | <span data-ttu-id="04811-109">类型</span><span class="sxs-lookup"><span data-stu-id="04811-109">Type</span></span>   |<span data-ttu-id="04811-110">说明</span><span class="sxs-lookup"><span data-stu-id="04811-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04811-111">code</span><span class="sxs-lookup"><span data-stu-id="04811-111">code</span></span>|<span data-ttu-id="04811-112">string</span><span class="sxs-lookup"><span data-stu-id="04811-112">string</span></span>|<span data-ttu-id="04811-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="04811-113">The error code.</span></span>|
|<span data-ttu-id="04811-114">message</span><span class="sxs-lookup"><span data-stu-id="04811-114">message</span></span>|<span data-ttu-id="04811-115">字符串</span><span class="sxs-lookup"><span data-stu-id="04811-115">string</span></span>|<span data-ttu-id="04811-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="04811-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
