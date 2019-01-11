---
title: 收件人资源类型
description: '表示事件、邮件或组帖子发送或接收端的用户的相关信息。 '
localization_priority: Normal
ms.openlocfilehash: b234cac0526ee66a59a19f7059dbebdc8a1bdcb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848375"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="08dcb-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="08dcb-103">recipient resource type</span></span>

> <span data-ttu-id="08dcb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08dcb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08dcb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08dcb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08dcb-106">表示事件、邮件或组帖子发送或接收端的用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="08dcb-106">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="08dcb-107">属性</span><span class="sxs-lookup"><span data-stu-id="08dcb-107">Properties</span></span>
| <span data-ttu-id="08dcb-108">属性</span><span class="sxs-lookup"><span data-stu-id="08dcb-108">Property</span></span>     | <span data-ttu-id="08dcb-109">类型</span><span class="sxs-lookup"><span data-stu-id="08dcb-109">Type</span></span>   |<span data-ttu-id="08dcb-110">说明</span><span class="sxs-lookup"><span data-stu-id="08dcb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08dcb-111">emailAddress</span><span class="sxs-lookup"><span data-stu-id="08dcb-111">emailAddress</span></span>|[<span data-ttu-id="08dcb-112">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="08dcb-112">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="08dcb-113">收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="08dcb-113">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08dcb-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08dcb-114">JSON representation</span></span>

<span data-ttu-id="08dcb-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08dcb-115">Here is a JSON representation of the resource</span></span>

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
