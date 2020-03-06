---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cdd0bb125fd8b84177b1370bca633f6d9ae5bb87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534263"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="9a679-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a679-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="9a679-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a679-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a679-105">会议参与者的相关信息。</span><span class="sxs-lookup"><span data-stu-id="9a679-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9a679-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a679-106">Properties</span></span>

| <span data-ttu-id="9a679-107">属性</span><span class="sxs-lookup"><span data-stu-id="9a679-107">Property</span></span>       | <span data-ttu-id="9a679-108">类型</span><span class="sxs-lookup"><span data-stu-id="9a679-108">Type</span></span>                          | <span data-ttu-id="9a679-109">说明</span><span class="sxs-lookup"><span data-stu-id="9a679-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="9a679-110">窃取</span><span class="sxs-lookup"><span data-stu-id="9a679-110">identity</span></span>       | [<span data-ttu-id="9a679-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a679-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="9a679-112">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="9a679-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="9a679-113">upn</span><span class="sxs-lookup"><span data-stu-id="9a679-113">upn</span></span>            | <span data-ttu-id="9a679-114">字符串</span><span class="sxs-lookup"><span data-stu-id="9a679-114">String</span></span>                        | <span data-ttu-id="9a679-115">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="9a679-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9a679-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a679-116">JSON representation</span></span>

<span data-ttu-id="9a679-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a679-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
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
