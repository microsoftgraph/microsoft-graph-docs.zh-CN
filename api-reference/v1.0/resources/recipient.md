---
title: 收件人资源类型
description: '表示事件、邮件或组帖子发送或接收端的用户的相关信息。 '
localization_priority: Normal
ms.openlocfilehash: 89d1ae7703d5b8b0e2a94027e74fbd4c4ebf9ed8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875290"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="72c4f-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="72c4f-103">recipient resource type</span></span>

<span data-ttu-id="72c4f-104">表示事件、邮件或组帖子发送或接收端的用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="72c4f-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="72c4f-105">属性</span><span class="sxs-lookup"><span data-stu-id="72c4f-105">Properties</span></span>
| <span data-ttu-id="72c4f-106">属性</span><span class="sxs-lookup"><span data-stu-id="72c4f-106">Property</span></span>     | <span data-ttu-id="72c4f-107">类型</span><span class="sxs-lookup"><span data-stu-id="72c4f-107">Type</span></span>   |<span data-ttu-id="72c4f-108">说明</span><span class="sxs-lookup"><span data-stu-id="72c4f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72c4f-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="72c4f-109">emailAddress</span></span>|[<span data-ttu-id="72c4f-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="72c4f-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="72c4f-111">收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="72c4f-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72c4f-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72c4f-112">JSON representation</span></span>

<span data-ttu-id="72c4f-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72c4f-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
