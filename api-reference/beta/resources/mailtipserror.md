---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1c456073ab1a32eb6bc236cb7047641ed967cdcf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129833"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="a7170-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7170-103">mailTipsError resource type</span></span>

<span data-ttu-id="a7170-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7170-105">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="a7170-105">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="a7170-106">属性</span><span class="sxs-lookup"><span data-stu-id="a7170-106">Properties</span></span>
| <span data-ttu-id="a7170-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7170-107">Property</span></span>     | <span data-ttu-id="a7170-108">类型</span><span class="sxs-lookup"><span data-stu-id="a7170-108">Type</span></span>   |<span data-ttu-id="a7170-109">描述</span><span class="sxs-lookup"><span data-stu-id="a7170-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="a7170-110">message</span><span class="sxs-lookup"><span data-stu-id="a7170-110">message</span></span> | <span data-ttu-id="a7170-111">String</span><span class="sxs-lookup"><span data-stu-id="a7170-111">String</span></span> | <span data-ttu-id="a7170-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="a7170-112">The error message.</span></span> |
| <span data-ttu-id="a7170-113">code</span><span class="sxs-lookup"><span data-stu-id="a7170-113">code</span></span> | <span data-ttu-id="a7170-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a7170-114">String</span></span> | <span data-ttu-id="a7170-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="a7170-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a7170-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7170-116">JSON representation</span></span>

<span data-ttu-id="a7170-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7170-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


