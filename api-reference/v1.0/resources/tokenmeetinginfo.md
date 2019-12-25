---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e34a10b9cd0fb09ff29c2d3373ad51a92109dcea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865757"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="28c2f-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="28c2f-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="28c2f-104">这是允许你加入现有会议的令牌信息。</span><span class="sxs-lookup"><span data-stu-id="28c2f-104">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="28c2f-105">这是作为传入呼叫通知的一部分获取的。</span><span class="sxs-lookup"><span data-stu-id="28c2f-105">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="28c2f-106">在断开呼叫的情况下，此信息可以帮助您重新加入该呼叫。</span><span class="sxs-lookup"><span data-stu-id="28c2f-106">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="28c2f-107">属性</span><span class="sxs-lookup"><span data-stu-id="28c2f-107">Properties</span></span>

| <span data-ttu-id="28c2f-108">属性</span><span class="sxs-lookup"><span data-stu-id="28c2f-108">Property</span></span>                     | <span data-ttu-id="28c2f-109">类型</span><span class="sxs-lookup"><span data-stu-id="28c2f-109">Type</span></span>    | <span data-ttu-id="28c2f-110">说明</span><span class="sxs-lookup"><span data-stu-id="28c2f-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="28c2f-111">令牌</span><span class="sxs-lookup"><span data-stu-id="28c2f-111">token</span></span>                        | <span data-ttu-id="28c2f-112">String</span><span class="sxs-lookup"><span data-stu-id="28c2f-112">String</span></span>  | <span data-ttu-id="28c2f-113">用于加入呼叫的令牌。</span><span class="sxs-lookup"><span data-stu-id="28c2f-113">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="28c2f-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28c2f-114">JSON representation</span></span>

<span data-ttu-id="28c2f-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28c2f-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
    "token": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
