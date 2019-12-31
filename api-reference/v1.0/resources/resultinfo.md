---
title: resultInfo 资源类型
description: 这包含成功和失败的特定结果信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 230783192e936d3fb3c2799e6cb98d39492589a3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913406"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="af603-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="af603-103">resultInfo resource type</span></span>

<span data-ttu-id="af603-104">这包含成功和失败的特定结果信息。</span><span class="sxs-lookup"><span data-stu-id="af603-104">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="af603-105">该代码指定结果是否为一般性成功或失败。</span><span class="sxs-lookup"><span data-stu-id="af603-105">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="af603-106">如果代码是2xx，如果它是一个客户端错误，它是成功的，如果是5xx，则表示服务器出错。</span><span class="sxs-lookup"><span data-stu-id="af603-106">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="af603-107">子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）</span><span class="sxs-lookup"><span data-stu-id="af603-107">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="af603-108">属性</span><span class="sxs-lookup"><span data-stu-id="af603-108">Properties</span></span>

| <span data-ttu-id="af603-109">属性</span><span class="sxs-lookup"><span data-stu-id="af603-109">Property</span></span> | <span data-ttu-id="af603-110">类型</span><span class="sxs-lookup"><span data-stu-id="af603-110">Type</span></span>   | <span data-ttu-id="af603-111">说明</span><span class="sxs-lookup"><span data-stu-id="af603-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="af603-112">code</span><span class="sxs-lookup"><span data-stu-id="af603-112">code</span></span>     | <span data-ttu-id="af603-113">Int32</span><span class="sxs-lookup"><span data-stu-id="af603-113">Int32</span></span> | <span data-ttu-id="af603-114">结果代码。</span><span class="sxs-lookup"><span data-stu-id="af603-114">The result code.</span></span>     |
| <span data-ttu-id="af603-115">message</span><span class="sxs-lookup"><span data-stu-id="af603-115">message</span></span>  | <span data-ttu-id="af603-116">String</span><span class="sxs-lookup"><span data-stu-id="af603-116">String</span></span> | <span data-ttu-id="af603-117">邮件。</span><span class="sxs-lookup"><span data-stu-id="af603-117">The message.</span></span>         |
| <span data-ttu-id="af603-118">subcode</span><span class="sxs-lookup"><span data-stu-id="af603-118">subcode</span></span>  | <span data-ttu-id="af603-119">Int32</span><span class="sxs-lookup"><span data-stu-id="af603-119">Int32</span></span> | <span data-ttu-id="af603-120">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="af603-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af603-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af603-121">JSON representation</span></span>

<span data-ttu-id="af603-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af603-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
