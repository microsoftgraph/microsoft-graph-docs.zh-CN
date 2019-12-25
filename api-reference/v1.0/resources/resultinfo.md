---
title: resultInfo 资源类型
description: 这包含成功和失败的特定结果信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 39027ecf949860d9ffa757a95839ae7fd8184a27
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865766"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="97564-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="97564-103">resultInfo resource type</span></span>

<span data-ttu-id="97564-104">这包含成功和失败的特定结果信息。</span><span class="sxs-lookup"><span data-stu-id="97564-104">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="97564-105">该代码指定结果是否为一般性成功或失败。</span><span class="sxs-lookup"><span data-stu-id="97564-105">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="97564-106">如果代码是2xx，如果它是一个客户端错误，它是成功的，如果是5xx，则表示服务器出错。</span><span class="sxs-lookup"><span data-stu-id="97564-106">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="97564-107">子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）</span><span class="sxs-lookup"><span data-stu-id="97564-107">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="97564-108">属性</span><span class="sxs-lookup"><span data-stu-id="97564-108">Properties</span></span>

| <span data-ttu-id="97564-109">属性</span><span class="sxs-lookup"><span data-stu-id="97564-109">Property</span></span> | <span data-ttu-id="97564-110">类型</span><span class="sxs-lookup"><span data-stu-id="97564-110">Type</span></span>   | <span data-ttu-id="97564-111">说明</span><span class="sxs-lookup"><span data-stu-id="97564-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="97564-112">code</span><span class="sxs-lookup"><span data-stu-id="97564-112">code</span></span>     | <span data-ttu-id="97564-113">Int32</span><span class="sxs-lookup"><span data-stu-id="97564-113">Int32</span></span> | <span data-ttu-id="97564-114">结果代码。</span><span class="sxs-lookup"><span data-stu-id="97564-114">The result code.</span></span>     |
| <span data-ttu-id="97564-115">message</span><span class="sxs-lookup"><span data-stu-id="97564-115">message</span></span>  | <span data-ttu-id="97564-116">String</span><span class="sxs-lookup"><span data-stu-id="97564-116">String</span></span> | <span data-ttu-id="97564-117">邮件。</span><span class="sxs-lookup"><span data-stu-id="97564-117">The message.</span></span>         |
| <span data-ttu-id="97564-118">subcode</span><span class="sxs-lookup"><span data-stu-id="97564-118">subcode</span></span>  | <span data-ttu-id="97564-119">Int32</span><span class="sxs-lookup"><span data-stu-id="97564-119">Int32</span></span> | <span data-ttu-id="97564-120">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="97564-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97564-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97564-121">JSON representation</span></span>

<span data-ttu-id="97564-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97564-122">The following is a JSON representation of the resource.</span></span>

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
