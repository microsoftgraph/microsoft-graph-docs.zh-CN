---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d9f5df716d62f2ae33e9a6c90d5803413b8c69b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461829"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="8fe7f-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fe7f-103">mailTipsError resource type</span></span>

<span data-ttu-id="8fe7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fe7f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fe7f-105">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="8fe7f-105">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="8fe7f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8fe7f-106">Properties</span></span>
| <span data-ttu-id="8fe7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8fe7f-107">Property</span></span>     | <span data-ttu-id="8fe7f-108">类型</span><span class="sxs-lookup"><span data-stu-id="8fe7f-108">Type</span></span>   |<span data-ttu-id="8fe7f-109">描述</span><span class="sxs-lookup"><span data-stu-id="8fe7f-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="8fe7f-110">message</span><span class="sxs-lookup"><span data-stu-id="8fe7f-110">message</span></span> | <span data-ttu-id="8fe7f-111">String</span><span class="sxs-lookup"><span data-stu-id="8fe7f-111">String</span></span> | <span data-ttu-id="8fe7f-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="8fe7f-112">The error message.</span></span> |
| <span data-ttu-id="8fe7f-113">code</span><span class="sxs-lookup"><span data-stu-id="8fe7f-113">code</span></span> | <span data-ttu-id="8fe7f-114">String</span><span class="sxs-lookup"><span data-stu-id="8fe7f-114">String</span></span> | <span data-ttu-id="8fe7f-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="8fe7f-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8fe7f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fe7f-116">JSON representation</span></span>

<span data-ttu-id="8fe7f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fe7f-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
