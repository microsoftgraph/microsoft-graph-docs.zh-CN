---
title: organizerMeetingInfo 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 00a7978c44c82ddd6b34802f29188a554e7e0b4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045344"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="a5251-103">organizerMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5251-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="a5251-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5251-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5251-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5251-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="a5251-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5251-106">Properties</span></span>

| <span data-ttu-id="a5251-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5251-107">Property</span></span>                     | <span data-ttu-id="a5251-108">类型</span><span class="sxs-lookup"><span data-stu-id="a5251-108">Type</span></span>                          | <span data-ttu-id="a5251-109">说明</span><span class="sxs-lookup"><span data-stu-id="a5251-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="a5251-110">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="a5251-110">allowConversationWithoutHost</span></span> | <span data-ttu-id="a5251-111">布尔</span><span class="sxs-lookup"><span data-stu-id="a5251-111">Boolean</span></span>                       | <span data-ttu-id="a5251-112">指示是否一旦离开对话的主机，也可以继续对话。</span><span class="sxs-lookup"><span data-stu-id="a5251-112">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="a5251-113">organizer</span><span class="sxs-lookup"><span data-stu-id="a5251-113">organizer</span></span>                    | [<span data-ttu-id="a5251-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="a5251-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="a5251-115">组织者 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="a5251-115">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a5251-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5251-116">JSON representation</span></span>

<span data-ttu-id="a5251-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5251-117">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="a5251-118">示例</span><span class="sxs-lookup"><span data-stu-id="a5251-118">Example</span></span>

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
