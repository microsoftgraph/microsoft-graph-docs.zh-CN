---
title: 收件人资源类型
description: '表示事件、邮件或组帖子发送或接收端的用户的相关信息。 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 600b058124f17f66b30af7430016a2ad274107e6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137499"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="74f93-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="74f93-103">recipient resource type</span></span>

<span data-ttu-id="74f93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74f93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74f93-105">表示事件、邮件或组帖子发送或接收端的用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="74f93-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="74f93-106">属性</span><span class="sxs-lookup"><span data-stu-id="74f93-106">Properties</span></span>
| <span data-ttu-id="74f93-107">属性</span><span class="sxs-lookup"><span data-stu-id="74f93-107">Property</span></span>     | <span data-ttu-id="74f93-108">类型</span><span class="sxs-lookup"><span data-stu-id="74f93-108">Type</span></span>   |<span data-ttu-id="74f93-109">说明</span><span class="sxs-lookup"><span data-stu-id="74f93-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74f93-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="74f93-110">emailAddress</span></span>|[<span data-ttu-id="74f93-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="74f93-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="74f93-112">收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="74f93-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74f93-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74f93-113">JSON representation</span></span>

<span data-ttu-id="74f93-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74f93-114">Here is a JSON representation of the resource</span></span>

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

