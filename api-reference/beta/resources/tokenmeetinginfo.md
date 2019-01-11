---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9a618906df450ce58f7428a76367e896b315591a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806977"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="22c0b-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="22c0b-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="22c0b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22c0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22c0b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22c0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22c0b-106">TokenMeetingInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="22c0b-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="22c0b-107">属性</span><span class="sxs-lookup"><span data-stu-id="22c0b-107">Properties</span></span>

| <span data-ttu-id="22c0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="22c0b-108">Property</span></span>                     | <span data-ttu-id="22c0b-109">类型</span><span class="sxs-lookup"><span data-stu-id="22c0b-109">Type</span></span>    | <span data-ttu-id="22c0b-110">Description</span><span class="sxs-lookup"><span data-stu-id="22c0b-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="22c0b-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="22c0b-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="22c0b-112">布尔</span><span class="sxs-lookup"><span data-stu-id="22c0b-112">Boolean</span></span> | <span data-ttu-id="22c0b-113">指示是否一旦离开对话的主机，也可以继续对话。</span><span class="sxs-lookup"><span data-stu-id="22c0b-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="22c0b-114">token</span><span class="sxs-lookup"><span data-stu-id="22c0b-114">token</span></span>                        | <span data-ttu-id="22c0b-115">String</span><span class="sxs-lookup"><span data-stu-id="22c0b-115">String</span></span>  | <span data-ttu-id="22c0b-116">要加入/激活会议的标记。</span><span class="sxs-lookup"><span data-stu-id="22c0b-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="22c0b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22c0b-117">JSON representation</span></span>

<span data-ttu-id="22c0b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22c0b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="22c0b-119">示例</span><span class="sxs-lookup"><span data-stu-id="22c0b-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
