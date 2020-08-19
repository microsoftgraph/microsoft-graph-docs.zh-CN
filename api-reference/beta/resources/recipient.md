---
title: 收件人资源类型
description: '表示事件、邮件或组帖子发送或接收端的用户的相关信息。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: ccd210eeecd84acf8094f7a55b1733e64c4a5437
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810467"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="0a8e7-103">收件人资源类型</span><span class="sxs-lookup"><span data-stu-id="0a8e7-103">recipient resource type</span></span>

<span data-ttu-id="0a8e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a8e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a8e7-105">表示事件、邮件或组帖子发送或接收端的用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="0a8e7-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="0a8e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="0a8e7-106">Properties</span></span>
| <span data-ttu-id="0a8e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="0a8e7-107">Property</span></span>     | <span data-ttu-id="0a8e7-108">类型</span><span class="sxs-lookup"><span data-stu-id="0a8e7-108">Type</span></span>   |<span data-ttu-id="0a8e7-109">说明</span><span class="sxs-lookup"><span data-stu-id="0a8e7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a8e7-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0a8e7-110">emailAddress</span></span>|[<span data-ttu-id="0a8e7-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="0a8e7-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0a8e7-112">收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0a8e7-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a8e7-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a8e7-113">JSON representation</span></span>

<span data-ttu-id="0a8e7-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a8e7-114">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
