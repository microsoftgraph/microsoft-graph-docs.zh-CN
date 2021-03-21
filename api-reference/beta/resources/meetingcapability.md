---
title: meetingCapability 资源类型
description: 包含会议功能
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d8e1d3985f95ecc28bd986218d7ff668f65b1db8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960402"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="d29b4-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="d29b4-103">meetingCapability resource type</span></span>

<span data-ttu-id="d29b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d29b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d29b4-105">包含会议功能</span><span class="sxs-lookup"><span data-stu-id="d29b4-105">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="d29b4-106">属性</span><span class="sxs-lookup"><span data-stu-id="d29b4-106">Properties</span></span>

| <span data-ttu-id="d29b4-107">属性</span><span class="sxs-lookup"><span data-stu-id="d29b4-107">Property</span></span>                          | <span data-ttu-id="d29b4-108">类型</span><span class="sxs-lookup"><span data-stu-id="d29b4-108">Type</span></span>    | <span data-ttu-id="d29b4-109">说明</span><span class="sxs-lookup"><span data-stu-id="d29b4-109">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="d29b4-110">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="d29b4-110">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="d29b4-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d29b4-111">Boolean</span></span> | <span data-ttu-id="d29b4-112">指示是否允许在会议中匿名用户拨出。</span><span class="sxs-lookup"><span data-stu-id="d29b4-112">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="d29b4-113">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="d29b4-113">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="d29b4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d29b4-114">Boolean</span></span> | <span data-ttu-id="d29b4-115">指示是否允许匿名用户启动会议。</span><span class="sxs-lookup"><span data-stu-id="d29b4-115">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="d29b4-116">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="d29b4-116">autoAdmittedUsers</span></span>                 | <span data-ttu-id="d29b4-117">autoAdmittedUsersType</span><span class="sxs-lookup"><span data-stu-id="d29b4-117">autoAdmittedUsersType</span></span>  | <span data-ttu-id="d29b4-118">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="d29b4-118">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="d29b4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d29b4-119">JSON representation</span></span>

<span data-ttu-id="d29b4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d29b4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


