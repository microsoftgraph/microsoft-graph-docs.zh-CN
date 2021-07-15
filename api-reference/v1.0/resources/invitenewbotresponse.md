---
title: inviteNewBotResponse 资源类型
description: 包含对请求的响应，请求让参与者加入通知作为传入呼叫通知再次发送到所需位置。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 675b7cd1df35b25e3414f36a4dd04e389e05b192
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430184"
---
# <a name="invitenewbotresponse-resource-type"></a><span data-ttu-id="bd766-103">inviteNewBotResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd766-103">inviteNewBotResponse resource type</span></span>

<span data-ttu-id="bd766-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd766-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd766-105">包含对请求的响应，请求让参与者加入通知作为传入呼叫通知再次发送到所需位置。</span><span class="sxs-lookup"><span data-stu-id="bd766-105">Contains a response to a request to have a participant joining notification sent out again as a incoming call notification to the desired location.</span></span>

## <a name="properties"></a><span data-ttu-id="bd766-106">属性</span><span class="sxs-lookup"><span data-stu-id="bd766-106">Properties</span></span>

| <span data-ttu-id="bd766-107">属性</span><span class="sxs-lookup"><span data-stu-id="bd766-107">Property</span></span>         | <span data-ttu-id="bd766-108">类型</span><span class="sxs-lookup"><span data-stu-id="bd766-108">Type</span></span>                            | <span data-ttu-id="bd766-109">说明</span><span class="sxs-lookup"><span data-stu-id="bd766-109">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bd766-110">inviteUri</span><span class="sxs-lookup"><span data-stu-id="bd766-110">inviteUri</span></span>        | <span data-ttu-id="bd766-111">String</span><span class="sxs-lookup"><span data-stu-id="bd766-111">String</span></span>                          | <span data-ttu-id="bd766-112">接收新传入呼叫通知的 URI。</span><span class="sxs-lookup"><span data-stu-id="bd766-112">URI to receive new incoming call notification.</span></span>                                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="bd766-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd766-113">JSON representation</span></span>

<span data-ttu-id="bd766-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd766-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.inviteNewBotResponse"
}-->
```json
{
  "inviteUri": "uri" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inviteNewBotResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
