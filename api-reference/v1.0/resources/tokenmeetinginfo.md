---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 786b3d1429d2f081207fa2d81b5f178d3cb5e08d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533440"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="635f3-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="635f3-103">tokenMeetingInfo resource type</span></span>

<span data-ttu-id="635f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="635f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="635f3-105">这是允许你加入现有会议的令牌信息。</span><span class="sxs-lookup"><span data-stu-id="635f3-105">This is the token information that allows you to join an existing meeting.</span></span> <span data-ttu-id="635f3-106">这是作为传入呼叫通知的一部分获取的。</span><span class="sxs-lookup"><span data-stu-id="635f3-106">This is obtained as part of the incoming call notification.</span></span> 

<span data-ttu-id="635f3-107">在断开呼叫的情况下，此信息可以帮助您重新加入该呼叫。</span><span class="sxs-lookup"><span data-stu-id="635f3-107">In the event that a call is disconnected, this information can help you rejoin that call.</span></span>

## <a name="properties"></a><span data-ttu-id="635f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="635f3-108">Properties</span></span>

| <span data-ttu-id="635f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="635f3-109">Property</span></span>                     | <span data-ttu-id="635f3-110">类型</span><span class="sxs-lookup"><span data-stu-id="635f3-110">Type</span></span>    | <span data-ttu-id="635f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="635f3-111">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="635f3-112">令牌</span><span class="sxs-lookup"><span data-stu-id="635f3-112">token</span></span>                        | <span data-ttu-id="635f3-113">String</span><span class="sxs-lookup"><span data-stu-id="635f3-113">String</span></span>  | <span data-ttu-id="635f3-114">用于加入呼叫的令牌。</span><span class="sxs-lookup"><span data-stu-id="635f3-114">The token used to join the call.</span></span>                                                 |

## <a name="json-representation"></a><span data-ttu-id="635f3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="635f3-115">JSON representation</span></span>

<span data-ttu-id="635f3-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="635f3-116">The following is a JSON representation of the resource.</span></span>

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
