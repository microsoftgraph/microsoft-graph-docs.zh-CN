---
title: meetingParticipantInfo 资源类型
description: 有关会议参与者的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40209354f1621839bd51a20fcbafa4cd58b4fd8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962453"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="a601b-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a601b-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="a601b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a601b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a601b-105">有关会议参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="a601b-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="a601b-106">属性</span><span class="sxs-lookup"><span data-stu-id="a601b-106">Properties</span></span>

| <span data-ttu-id="a601b-107">属性</span><span class="sxs-lookup"><span data-stu-id="a601b-107">Property</span></span> | <span data-ttu-id="a601b-108">类型</span><span class="sxs-lookup"><span data-stu-id="a601b-108">Type</span></span>                          | <span data-ttu-id="a601b-109">说明</span><span class="sxs-lookup"><span data-stu-id="a601b-109">Description</span></span>                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="a601b-110">identity</span><span class="sxs-lookup"><span data-stu-id="a601b-110">identity</span></span> | [<span data-ttu-id="a601b-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="a601b-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="a601b-112">参与者的身份信息。</span><span class="sxs-lookup"><span data-stu-id="a601b-112">Identity information of the participant.</span></span>                                            |
| <span data-ttu-id="a601b-113">upn</span><span class="sxs-lookup"><span data-stu-id="a601b-113">upn</span></span>      | <span data-ttu-id="a601b-114">String</span><span class="sxs-lookup"><span data-stu-id="a601b-114">String</span></span>                        | <span data-ttu-id="a601b-115">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a601b-115">User principal name of the participant.</span></span>                                             |
| <span data-ttu-id="a601b-116">role</span><span class="sxs-lookup"><span data-stu-id="a601b-116">role</span></span>     | <span data-ttu-id="a601b-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="a601b-117">onlineMeetingRole</span></span>             | <span data-ttu-id="a601b-118">指定会议参与者的角色。</span><span class="sxs-lookup"><span data-stu-id="a601b-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="a601b-119">可取值为：`attendee`、`presenter` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a601b-119">Possible values are `attendee`, `presenter`, and `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a601b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a601b-120">JSON representation</span></span>

<span data-ttu-id="a601b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a601b-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

