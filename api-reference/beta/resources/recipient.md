---
title: 收件人资源类型
description: '表示事件、邮件或组帖子发送或接收端的用户的相关信息。 '
localization_priority: Normal
ms.openlocfilehash: 9718d7e6ce09a42e742303aaed484fa6335f3cbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563194"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="ee847-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="ee847-103">recipient resource type</span></span>

<span data-ttu-id="ee847-104">表示事件、邮件或组帖子发送或接收端的用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="ee847-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="ee847-105">属性</span><span class="sxs-lookup"><span data-stu-id="ee847-105">Properties</span></span>
| <span data-ttu-id="ee847-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee847-106">Property</span></span>     | <span data-ttu-id="ee847-107">类型</span><span class="sxs-lookup"><span data-stu-id="ee847-107">Type</span></span>   |<span data-ttu-id="ee847-108">说明</span><span class="sxs-lookup"><span data-stu-id="ee847-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee847-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ee847-109">emailAddress</span></span>|[<span data-ttu-id="ee847-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="ee847-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ee847-111">收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ee847-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee847-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee847-112">JSON representation</span></span>

<span data-ttu-id="ee847-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee847-113">Here is a JSON representation of the resource</span></span>

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
