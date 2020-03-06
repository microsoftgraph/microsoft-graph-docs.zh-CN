---
title: recordOperation 资源类型
description: 此资源类型包含与音频录音相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9424055d5669b9279dede18b6eb3773da47d9b19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533885"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="4361a-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4361a-103">recordOperation resource type</span></span>

<span data-ttu-id="4361a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4361a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4361a-105">此资源类型包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="4361a-105">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="4361a-106">属性</span><span class="sxs-lookup"><span data-stu-id="4361a-106">Properties</span></span>

| <span data-ttu-id="4361a-107">属性</span><span class="sxs-lookup"><span data-stu-id="4361a-107">Property</span></span>                       | <span data-ttu-id="4361a-108">类型</span><span class="sxs-lookup"><span data-stu-id="4361a-108">Type</span></span>                        | <span data-ttu-id="4361a-109">说明</span><span class="sxs-lookup"><span data-stu-id="4361a-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4361a-110">适用</span><span class="sxs-lookup"><span data-stu-id="4361a-110">clientContext</span></span>                  | <span data-ttu-id="4361a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="4361a-111">String</span></span>                      | <span data-ttu-id="4361a-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="4361a-112">Unique Client Context string.</span></span> <span data-ttu-id="4361a-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="4361a-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="4361a-114">id</span><span class="sxs-lookup"><span data-stu-id="4361a-114">id</span></span>                             | <span data-ttu-id="4361a-115">String</span><span class="sxs-lookup"><span data-stu-id="4361a-115">String</span></span>                      | <span data-ttu-id="4361a-116">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="4361a-116">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="4361a-117">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="4361a-117">recordingAccessToken</span></span>           | <span data-ttu-id="4361a-118">字符串</span><span class="sxs-lookup"><span data-stu-id="4361a-118">String</span></span>                      | <span data-ttu-id="4361a-119">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="4361a-119">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="4361a-120">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="4361a-120">recordingLocation</span></span>              | <span data-ttu-id="4361a-121">字符串</span><span class="sxs-lookup"><span data-stu-id="4361a-121">String</span></span>                      | <span data-ttu-id="4361a-122">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="4361a-122">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="4361a-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4361a-123">resultInfo</span></span>                     | [<span data-ttu-id="4361a-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4361a-124">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4361a-125">结果信息。</span><span class="sxs-lookup"><span data-stu-id="4361a-125">The result information.</span></span>  <span data-ttu-id="4361a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="4361a-126">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="4361a-127">状态</span><span class="sxs-lookup"><span data-stu-id="4361a-127">status</span></span>                         | <span data-ttu-id="4361a-128">String</span><span class="sxs-lookup"><span data-stu-id="4361a-128">String</span></span>                      | <span data-ttu-id="4361a-129">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="4361a-129">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4361a-130">只读。</span><span class="sxs-lookup"><span data-stu-id="4361a-130">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="4361a-131">关系</span><span class="sxs-lookup"><span data-stu-id="4361a-131">Relationships</span></span>
<span data-ttu-id="4361a-132">无</span><span class="sxs-lookup"><span data-stu-id="4361a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4361a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4361a-133">JSON representation</span></span>

<span data-ttu-id="4361a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4361a-134">The following is a JSON representation of the resource.</span></span>

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
