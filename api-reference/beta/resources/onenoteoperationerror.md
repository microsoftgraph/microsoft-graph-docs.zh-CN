---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 6c61ab3808a37d1f90f15dc55ab6331c5bec8c7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522335"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="09c6d-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="09c6d-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="09c6d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09c6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09c6d-105">失败的 OneNote 操作中的错误。</span><span class="sxs-lookup"><span data-stu-id="09c6d-105">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09c6d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09c6d-106">JSON representation</span></span>

<span data-ttu-id="09c6d-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09c6d-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="09c6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="09c6d-108">Properties</span></span>
| <span data-ttu-id="09c6d-109">属性</span><span class="sxs-lookup"><span data-stu-id="09c6d-109">Property</span></span>     | <span data-ttu-id="09c6d-110">类型</span><span class="sxs-lookup"><span data-stu-id="09c6d-110">Type</span></span>   |<span data-ttu-id="09c6d-111">说明</span><span class="sxs-lookup"><span data-stu-id="09c6d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09c6d-112">code</span><span class="sxs-lookup"><span data-stu-id="09c6d-112">code</span></span>|<span data-ttu-id="09c6d-113">string</span><span class="sxs-lookup"><span data-stu-id="09c6d-113">string</span></span>|<span data-ttu-id="09c6d-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="09c6d-114">The error code.</span></span>|
|<span data-ttu-id="09c6d-115">message</span><span class="sxs-lookup"><span data-stu-id="09c6d-115">message</span></span>|<span data-ttu-id="09c6d-116">字符串</span><span class="sxs-lookup"><span data-stu-id="09c6d-116">string</span></span>|<span data-ttu-id="09c6d-117">错误消息。</span><span class="sxs-lookup"><span data-stu-id="09c6d-117">The error message.</span></span>|

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
