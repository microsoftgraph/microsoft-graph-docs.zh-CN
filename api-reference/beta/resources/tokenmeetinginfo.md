---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0df9a7a66420f20ff62677f54e617d64e9db0273
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007541"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="88fb4-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="88fb4-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88fb4-104">TokenMeetingInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="88fb4-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="88fb4-105">属性</span><span class="sxs-lookup"><span data-stu-id="88fb4-105">Properties</span></span>

| <span data-ttu-id="88fb4-106">属性</span><span class="sxs-lookup"><span data-stu-id="88fb4-106">Property</span></span>                     | <span data-ttu-id="88fb4-107">类型</span><span class="sxs-lookup"><span data-stu-id="88fb4-107">Type</span></span>    | <span data-ttu-id="88fb4-108">说明</span><span class="sxs-lookup"><span data-stu-id="88fb4-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="88fb4-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="88fb4-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="88fb4-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="88fb4-110">Boolean</span></span> | <span data-ttu-id="88fb4-111">指示会话离开的主机后是否可以继续会话。</span><span class="sxs-lookup"><span data-stu-id="88fb4-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="88fb4-112">token</span><span class="sxs-lookup"><span data-stu-id="88fb4-112">token</span></span>                        | <span data-ttu-id="88fb4-113">String</span><span class="sxs-lookup"><span data-stu-id="88fb4-113">String</span></span>  | <span data-ttu-id="88fb4-114">要加入/激活会议的令牌。</span><span class="sxs-lookup"><span data-stu-id="88fb4-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="88fb4-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88fb4-115">JSON representation</span></span>

<span data-ttu-id="88fb4-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88fb4-116">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="88fb4-117">示例</span><span class="sxs-lookup"><span data-stu-id="88fb4-117">Example</span></span>

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
