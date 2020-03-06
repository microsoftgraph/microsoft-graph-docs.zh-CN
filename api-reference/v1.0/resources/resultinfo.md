---
title: resultInfo 资源类型
description: 这包含成功和失败的特定结果信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42b636b09e8cfeb2ed41578e06fc57b5aa976fd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533822"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="7b842-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b842-103">resultInfo resource type</span></span>

<span data-ttu-id="7b842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b842-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b842-105">这包含成功和失败的特定结果信息。</span><span class="sxs-lookup"><span data-stu-id="7b842-105">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="7b842-106">该代码指定结果是否为一般性成功或失败。</span><span class="sxs-lookup"><span data-stu-id="7b842-106">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="7b842-107">如果代码是2xx，如果它是一个客户端错误，它是成功的，如果是5xx，则表示服务器出错。</span><span class="sxs-lookup"><span data-stu-id="7b842-107">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="7b842-108">子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）</span><span class="sxs-lookup"><span data-stu-id="7b842-108">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="7b842-109">属性</span><span class="sxs-lookup"><span data-stu-id="7b842-109">Properties</span></span>

| <span data-ttu-id="7b842-110">属性</span><span class="sxs-lookup"><span data-stu-id="7b842-110">Property</span></span> | <span data-ttu-id="7b842-111">类型</span><span class="sxs-lookup"><span data-stu-id="7b842-111">Type</span></span>   | <span data-ttu-id="7b842-112">说明</span><span class="sxs-lookup"><span data-stu-id="7b842-112">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="7b842-113">code</span><span class="sxs-lookup"><span data-stu-id="7b842-113">code</span></span>     | <span data-ttu-id="7b842-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7b842-114">Int32</span></span> | <span data-ttu-id="7b842-115">结果代码。</span><span class="sxs-lookup"><span data-stu-id="7b842-115">The result code.</span></span>     |
| <span data-ttu-id="7b842-116">message</span><span class="sxs-lookup"><span data-stu-id="7b842-116">message</span></span>  | <span data-ttu-id="7b842-117">String</span><span class="sxs-lookup"><span data-stu-id="7b842-117">String</span></span> | <span data-ttu-id="7b842-118">邮件。</span><span class="sxs-lookup"><span data-stu-id="7b842-118">The message.</span></span>         |
| <span data-ttu-id="7b842-119">subcode</span><span class="sxs-lookup"><span data-stu-id="7b842-119">subcode</span></span>  | <span data-ttu-id="7b842-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7b842-120">Int32</span></span> | <span data-ttu-id="7b842-121">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="7b842-121">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b842-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b842-122">JSON representation</span></span>

<span data-ttu-id="7b842-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b842-123">The following is a JSON representation of the resource.</span></span>

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
