---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e77322dee3f8d94fe8eaee226dce029133a578d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635192"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="c6678-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6678-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="c6678-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6678-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6678-105">包含有关会议参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="c6678-105">Contains information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="c6678-106">属性</span><span class="sxs-lookup"><span data-stu-id="c6678-106">Properties</span></span>

| <span data-ttu-id="c6678-107">属性</span><span class="sxs-lookup"><span data-stu-id="c6678-107">Property</span></span> | <span data-ttu-id="c6678-108">类型</span><span class="sxs-lookup"><span data-stu-id="c6678-108">Type</span></span>                          | <span data-ttu-id="c6678-109">说明</span><span class="sxs-lookup"><span data-stu-id="c6678-109">Description</span></span>                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="c6678-110">窃取</span><span class="sxs-lookup"><span data-stu-id="c6678-110">identity</span></span> | [<span data-ttu-id="c6678-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="c6678-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="c6678-112">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="c6678-112">Identity information of the participant.</span></span>                                           |
| <span data-ttu-id="c6678-113">upn</span><span class="sxs-lookup"><span data-stu-id="c6678-113">upn</span></span>      | <span data-ttu-id="c6678-114">String</span><span class="sxs-lookup"><span data-stu-id="c6678-114">String</span></span>                        | <span data-ttu-id="c6678-115">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c6678-115">User principal name of the participant.</span></span>                                            |
| <span data-ttu-id="c6678-116">role</span><span class="sxs-lookup"><span data-stu-id="c6678-116">role</span></span>     | <span data-ttu-id="c6678-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="c6678-117">onlineMeetingRole</span></span>             | <span data-ttu-id="c6678-118">指定参与者在会议中的角色。</span><span class="sxs-lookup"><span data-stu-id="c6678-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="c6678-119">可取值为：`attendee`、`presenter` 和 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c6678-119">Possible values are `attendee`, `presenter`, and `unknownFutureValue`.</span></span>|

### <a name="onlinemeetingrole-values"></a><span data-ttu-id="c6678-120">onlineMeetingRole 值</span><span class="sxs-lookup"><span data-stu-id="c6678-120">onlineMeetingRole values</span></span>

| <span data-ttu-id="c6678-121">值</span><span class="sxs-lookup"><span data-stu-id="c6678-121">Value</span></span>              | <span data-ttu-id="c6678-122">说明</span><span class="sxs-lookup"><span data-stu-id="c6678-122">Description</span></span>                     |
| ------------------ | ------------------------------- |
| <span data-ttu-id="c6678-123">attendee</span><span class="sxs-lookup"><span data-stu-id="c6678-123">attendee</span></span>           | <span data-ttu-id="c6678-124">参与者是与会者。</span><span class="sxs-lookup"><span data-stu-id="c6678-124">The participant is an attendee.</span></span> |
| <span data-ttu-id="c6678-125">演示者</span><span class="sxs-lookup"><span data-stu-id="c6678-125">presenter</span></span>          | <span data-ttu-id="c6678-126">参与者是演示者。</span><span class="sxs-lookup"><span data-stu-id="c6678-126">The participant is a presenter.</span></span> |
| <span data-ttu-id="c6678-127">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="c6678-127">unknownFutureValue</span></span> | <span data-ttu-id="c6678-128">未知的未来值。</span><span class="sxs-lookup"><span data-stu-id="c6678-128">Unknown future value.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="c6678-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6678-129">JSON representation</span></span>

<span data-ttu-id="c6678-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6678-130">The following is a JSON representation of the resource.</span></span>

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


