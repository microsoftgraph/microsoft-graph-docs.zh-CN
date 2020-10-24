---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a642532579d127fdeb48b4c69524975b293ff959
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741997"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="ed41b-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed41b-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="ed41b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed41b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed41b-105">会议参与者的相关信息。</span><span class="sxs-lookup"><span data-stu-id="ed41b-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="ed41b-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed41b-106">Properties</span></span>

| <span data-ttu-id="ed41b-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed41b-107">Property</span></span> | <span data-ttu-id="ed41b-108">类型</span><span class="sxs-lookup"><span data-stu-id="ed41b-108">Type</span></span>                          | <span data-ttu-id="ed41b-109">说明</span><span class="sxs-lookup"><span data-stu-id="ed41b-109">Description</span></span>                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="ed41b-110">窃取</span><span class="sxs-lookup"><span data-stu-id="ed41b-110">identity</span></span> | [<span data-ttu-id="ed41b-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="ed41b-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="ed41b-112">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="ed41b-112">Identity information of the participant.</span></span>                                            |
| <span data-ttu-id="ed41b-113">upn</span><span class="sxs-lookup"><span data-stu-id="ed41b-113">upn</span></span>      | <span data-ttu-id="ed41b-114">String</span><span class="sxs-lookup"><span data-stu-id="ed41b-114">String</span></span>                        | <span data-ttu-id="ed41b-115">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="ed41b-115">User principal name of the participant.</span></span>                                             |
| <span data-ttu-id="ed41b-116">role</span><span class="sxs-lookup"><span data-stu-id="ed41b-116">role</span></span>     | <span data-ttu-id="ed41b-117">onlineMeetingRole</span><span class="sxs-lookup"><span data-stu-id="ed41b-117">onlineMeetingRole</span></span>             | <span data-ttu-id="ed41b-118">指定参与者在会议中的角色。</span><span class="sxs-lookup"><span data-stu-id="ed41b-118">Specifies the participant's role in the meeting.</span></span>  <span data-ttu-id="ed41b-119">下表中列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="ed41b-119">Possible values are listed in the following table.</span></span> |

### <a name="onlinemeetingrole-values"></a><span data-ttu-id="ed41b-120">onlineMeetingRole 值</span><span class="sxs-lookup"><span data-stu-id="ed41b-120">onlineMeetingRole values</span></span>

| <span data-ttu-id="ed41b-121">值</span><span class="sxs-lookup"><span data-stu-id="ed41b-121">Value</span></span>              | <span data-ttu-id="ed41b-122">说明</span><span class="sxs-lookup"><span data-stu-id="ed41b-122">Description</span></span>                     |
| ------------------ | ------------------------------- |
| <span data-ttu-id="ed41b-123">attendee</span><span class="sxs-lookup"><span data-stu-id="ed41b-123">attendee</span></span>           | <span data-ttu-id="ed41b-124">参与者是与会者。</span><span class="sxs-lookup"><span data-stu-id="ed41b-124">The participant is an attendee.</span></span> |
| <span data-ttu-id="ed41b-125">演示者</span><span class="sxs-lookup"><span data-stu-id="ed41b-125">presenter</span></span>          | <span data-ttu-id="ed41b-126">参与者是演示者。</span><span class="sxs-lookup"><span data-stu-id="ed41b-126">The participant is a presenter.</span></span> |
| <span data-ttu-id="ed41b-127">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="ed41b-127">unknownFutureValue</span></span> | <span data-ttu-id="ed41b-128">未知的未来值。</span><span class="sxs-lookup"><span data-stu-id="ed41b-128">Unknown future value.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="ed41b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed41b-129">JSON representation</span></span>

<span data-ttu-id="ed41b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed41b-130">The following is a JSON representation of the resource.</span></span>

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

