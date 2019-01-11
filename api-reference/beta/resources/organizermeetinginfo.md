---
title: organizerMeetingInfo 资源类型
description: 包含会议的组织者的会议信息。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: fd096a55762892ca9b2fd72c883a544e503c5f90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870727"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="59621-103">organizerMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="59621-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="59621-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="59621-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59621-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59621-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59621-106">包含会议的组织者的会议信息。</span><span class="sxs-lookup"><span data-stu-id="59621-106">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="59621-107">属性</span><span class="sxs-lookup"><span data-stu-id="59621-107">Properties</span></span>

| <span data-ttu-id="59621-108">属性</span><span class="sxs-lookup"><span data-stu-id="59621-108">Property</span></span>                     | <span data-ttu-id="59621-109">类型</span><span class="sxs-lookup"><span data-stu-id="59621-109">Type</span></span>                          | <span data-ttu-id="59621-110">Description</span><span class="sxs-lookup"><span data-stu-id="59621-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="59621-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="59621-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="59621-112">布尔</span><span class="sxs-lookup"><span data-stu-id="59621-112">Boolean</span></span>                       | <span data-ttu-id="59621-113">指示是否一旦离开对话的主机，也可以继续对话。</span><span class="sxs-lookup"><span data-stu-id="59621-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="59621-114">organizer</span><span class="sxs-lookup"><span data-stu-id="59621-114">organizer</span></span>                    | [<span data-ttu-id="59621-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="59621-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="59621-116">组织者 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="59621-116">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="59621-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59621-117">JSON representation</span></span>

<span data-ttu-id="59621-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59621-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="59621-119">示例</span><span class="sxs-lookup"><span data-stu-id="59621-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
