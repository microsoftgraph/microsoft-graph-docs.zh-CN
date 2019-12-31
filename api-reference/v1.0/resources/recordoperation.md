---
title: recordOperation 资源类型
description: 此资源类型包含与音频录音相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 03cdf594b04c75cd14b31dfbaef5894e8aacd19d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913665"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="b6121-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6121-103">recordOperation resource type</span></span>

<span data-ttu-id="b6121-104">此资源类型包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="b6121-104">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="b6121-105">属性</span><span class="sxs-lookup"><span data-stu-id="b6121-105">Properties</span></span>

| <span data-ttu-id="b6121-106">属性</span><span class="sxs-lookup"><span data-stu-id="b6121-106">Property</span></span>                       | <span data-ttu-id="b6121-107">类型</span><span class="sxs-lookup"><span data-stu-id="b6121-107">Type</span></span>                        | <span data-ttu-id="b6121-108">说明</span><span class="sxs-lookup"><span data-stu-id="b6121-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b6121-109">适用</span><span class="sxs-lookup"><span data-stu-id="b6121-109">clientContext</span></span>                  | <span data-ttu-id="b6121-110">String</span><span class="sxs-lookup"><span data-stu-id="b6121-110">String</span></span>                      | <span data-ttu-id="b6121-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="b6121-111">Unique Client Context string.</span></span> <span data-ttu-id="b6121-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="b6121-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="b6121-113">id</span><span class="sxs-lookup"><span data-stu-id="b6121-113">id</span></span>                             | <span data-ttu-id="b6121-114">String</span><span class="sxs-lookup"><span data-stu-id="b6121-114">String</span></span>                      | <span data-ttu-id="b6121-115">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="b6121-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="b6121-116">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="b6121-116">recordingAccessToken</span></span>           | <span data-ttu-id="b6121-117">String</span><span class="sxs-lookup"><span data-stu-id="b6121-117">String</span></span>                      | <span data-ttu-id="b6121-118">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b6121-118">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="b6121-119">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="b6121-119">recordingLocation</span></span>              | <span data-ttu-id="b6121-120">String</span><span class="sxs-lookup"><span data-stu-id="b6121-120">String</span></span>                      | <span data-ttu-id="b6121-121">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="b6121-121">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="b6121-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b6121-122">resultInfo</span></span>                     | [<span data-ttu-id="b6121-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b6121-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b6121-124">结果信息。</span><span class="sxs-lookup"><span data-stu-id="b6121-124">The result information.</span></span>  <span data-ttu-id="b6121-125">只读。</span><span class="sxs-lookup"><span data-stu-id="b6121-125">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="b6121-126">状态</span><span class="sxs-lookup"><span data-stu-id="b6121-126">status</span></span>                         | <span data-ttu-id="b6121-127">String</span><span class="sxs-lookup"><span data-stu-id="b6121-127">String</span></span>                      | <span data-ttu-id="b6121-128">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b6121-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b6121-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b6121-129">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="b6121-130">关系</span><span class="sxs-lookup"><span data-stu-id="b6121-130">Relationships</span></span>
<span data-ttu-id="b6121-131">无</span><span class="sxs-lookup"><span data-stu-id="b6121-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6121-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6121-132">JSON representation</span></span>

<span data-ttu-id="b6121-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6121-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
