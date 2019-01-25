---
title: organizerMeetingInfo 资源类型
description: 包含会议的组织者的会议信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3b7d21a313d8744f18c8b96549bc9470b587361c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512239"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="a3fec-103">organizerMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3fec-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3fec-104">包含会议的组织者的会议信息。</span><span class="sxs-lookup"><span data-stu-id="a3fec-104">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="a3fec-105">属性</span><span class="sxs-lookup"><span data-stu-id="a3fec-105">Properties</span></span>

| <span data-ttu-id="a3fec-106">属性</span><span class="sxs-lookup"><span data-stu-id="a3fec-106">Property</span></span>                     | <span data-ttu-id="a3fec-107">类型</span><span class="sxs-lookup"><span data-stu-id="a3fec-107">Type</span></span>                          | <span data-ttu-id="a3fec-108">说明</span><span class="sxs-lookup"><span data-stu-id="a3fec-108">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="a3fec-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="a3fec-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="a3fec-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3fec-110">Boolean</span></span>                       | <span data-ttu-id="a3fec-111">指示是否一旦离开对话的主机，也可以继续对话。</span><span class="sxs-lookup"><span data-stu-id="a3fec-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="a3fec-112">organizer</span><span class="sxs-lookup"><span data-stu-id="a3fec-112">organizer</span></span>                    | [<span data-ttu-id="a3fec-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="a3fec-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="a3fec-114">组织者 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="a3fec-114">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a3fec-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3fec-115">JSON representation</span></span>

<span data-ttu-id="a3fec-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3fec-116">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="a3fec-117">示例</span><span class="sxs-lookup"><span data-stu-id="a3fec-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/organizermeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
