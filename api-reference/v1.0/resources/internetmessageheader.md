---
title: internetMessageHeader 资源类型
description: '表示 Internet 邮件头 (由 RFC5322 定义) 的键/值对, 可提供 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 14d4cb88c79651bbba381206df7d5ff9b26db0bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030196"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="c64de-103">internetMessageHeader 资源类型</span><span class="sxs-lookup"><span data-stu-id="c64de-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="c64de-104">一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c64de-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="c64de-105">有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。</span><span class="sxs-lookup"><span data-stu-id="c64de-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="c64de-106">属性</span><span class="sxs-lookup"><span data-stu-id="c64de-106">Properties</span></span>
| <span data-ttu-id="c64de-107">属性</span><span class="sxs-lookup"><span data-stu-id="c64de-107">Property</span></span>     | <span data-ttu-id="c64de-108">类型</span><span class="sxs-lookup"><span data-stu-id="c64de-108">Type</span></span>   |<span data-ttu-id="c64de-109">说明</span><span class="sxs-lookup"><span data-stu-id="c64de-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c64de-110">name</span><span class="sxs-lookup"><span data-stu-id="c64de-110">name</span></span>|<span data-ttu-id="c64de-111">string</span><span class="sxs-lookup"><span data-stu-id="c64de-111">string</span></span>|<span data-ttu-id="c64de-112">表示键值对中的键。</span><span class="sxs-lookup"><span data-stu-id="c64de-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="c64de-113">value</span><span class="sxs-lookup"><span data-stu-id="c64de-113">value</span></span>|<span data-ttu-id="c64de-114">string</span><span class="sxs-lookup"><span data-stu-id="c64de-114">string</span></span>|<span data-ttu-id="c64de-115">键值对中的值。</span><span class="sxs-lookup"><span data-stu-id="c64de-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c64de-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c64de-116">JSON representation</span></span>

<span data-ttu-id="c64de-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c64de-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
