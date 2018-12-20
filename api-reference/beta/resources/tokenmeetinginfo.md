---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: VinodRavichandran
ms.openlocfilehash: 6fa66fef6f401db848a9ed3e92c5a1003a5294b6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380546"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="d6fe1-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6fe1-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="d6fe1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6fe1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6fe1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6fe1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6fe1-106">TokenMeetingInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="d6fe1-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="d6fe1-107">属性</span><span class="sxs-lookup"><span data-stu-id="d6fe1-107">Properties</span></span>

| <span data-ttu-id="d6fe1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6fe1-108">Property</span></span>                     | <span data-ttu-id="d6fe1-109">类型</span><span class="sxs-lookup"><span data-stu-id="d6fe1-109">Type</span></span>    | <span data-ttu-id="d6fe1-110">说明</span><span class="sxs-lookup"><span data-stu-id="d6fe1-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="d6fe1-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="d6fe1-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="d6fe1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6fe1-112">Boolean</span></span> | <span data-ttu-id="d6fe1-113">指示是否一旦离开对话的主机，也可以继续对话。</span><span class="sxs-lookup"><span data-stu-id="d6fe1-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="d6fe1-114">token</span><span class="sxs-lookup"><span data-stu-id="d6fe1-114">token</span></span>                        | <span data-ttu-id="d6fe1-115">String</span><span class="sxs-lookup"><span data-stu-id="d6fe1-115">String</span></span>  | <span data-ttu-id="d6fe1-116">要加入/激活会议的标记。</span><span class="sxs-lookup"><span data-stu-id="d6fe1-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="d6fe1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6fe1-117">JSON representation</span></span>

<span data-ttu-id="d6fe1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6fe1-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="d6fe1-119">示例</span><span class="sxs-lookup"><span data-stu-id="d6fe1-119">Example</span></span>

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
