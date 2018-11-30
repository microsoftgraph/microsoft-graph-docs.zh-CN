---
title: meetingParticipantInfo 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 1d9c22924f8f05255b5e01bad4bbcd6ae5957ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045140"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="fa910-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa910-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="fa910-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa910-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa910-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa910-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="fa910-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa910-106">Properties</span></span>

| <span data-ttu-id="fa910-107">属性</span><span class="sxs-lookup"><span data-stu-id="fa910-107">Property</span></span>       | <span data-ttu-id="fa910-108">类型</span><span class="sxs-lookup"><span data-stu-id="fa910-108">Type</span></span>                          | <span data-ttu-id="fa910-109">说明</span><span class="sxs-lookup"><span data-stu-id="fa910-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="fa910-110">标识</span><span class="sxs-lookup"><span data-stu-id="fa910-110">identity</span></span>       | [<span data-ttu-id="fa910-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa910-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="fa910-112">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="fa910-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="fa910-113">upn</span><span class="sxs-lookup"><span data-stu-id="fa910-113">upn</span></span>            | <span data-ttu-id="fa910-114">字符串</span><span class="sxs-lookup"><span data-stu-id="fa910-114">String</span></span>                        | <span data-ttu-id="fa910-115">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="fa910-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="fa910-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa910-116">JSON representation</span></span>

<span data-ttu-id="fa910-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa910-117">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
