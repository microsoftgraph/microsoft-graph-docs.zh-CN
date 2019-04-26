---
title: tokenMeetingInfo 资源类型
description: tokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 38a5aae17cf4364a1cfd58680c2e7b9437cf0e40
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345498"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="0e2ca-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e2ca-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e2ca-104">tokenMeetingInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="0e2ca-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="0e2ca-105">属性</span><span class="sxs-lookup"><span data-stu-id="0e2ca-105">Properties</span></span>

| <span data-ttu-id="0e2ca-106">属性</span><span class="sxs-lookup"><span data-stu-id="0e2ca-106">Property</span></span>                     | <span data-ttu-id="0e2ca-107">类型</span><span class="sxs-lookup"><span data-stu-id="0e2ca-107">Type</span></span>    | <span data-ttu-id="0e2ca-108">说明</span><span class="sxs-lookup"><span data-stu-id="0e2ca-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="0e2ca-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="0e2ca-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="0e2ca-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e2ca-110">Boolean</span></span> | <span data-ttu-id="0e2ca-111">指示会话离开的主机后是否可以继续会话。</span><span class="sxs-lookup"><span data-stu-id="0e2ca-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="0e2ca-112">token</span><span class="sxs-lookup"><span data-stu-id="0e2ca-112">token</span></span>                        | <span data-ttu-id="0e2ca-113">String</span><span class="sxs-lookup"><span data-stu-id="0e2ca-113">String</span></span>  | <span data-ttu-id="0e2ca-114">要加入/激活会议的令牌。</span><span class="sxs-lookup"><span data-stu-id="0e2ca-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="0e2ca-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e2ca-115">JSON representation</span></span>

<span data-ttu-id="0e2ca-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e2ca-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType": "microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="0e2ca-117">示例</span><span class="sxs-lookup"><span data-stu-id="0e2ca-117">Example</span></span>

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
