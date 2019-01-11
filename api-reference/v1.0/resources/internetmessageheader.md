---
title: internetMessageHeader 资源类型
description: '表示由 RFC5322，提供定义 Internet 邮件头，键 / 值对 '
localization_priority: Normal
ms.openlocfilehash: 2a8dd616ffe8417a5064c0a98976d512b1279704
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892349"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="98c5c-103">internetMessageHeader 资源类型</span><span class="sxs-lookup"><span data-stu-id="98c5c-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="98c5c-104">一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。</span><span class="sxs-lookup"><span data-stu-id="98c5c-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="98c5c-105">有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。</span><span class="sxs-lookup"><span data-stu-id="98c5c-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="98c5c-106">属性</span><span class="sxs-lookup"><span data-stu-id="98c5c-106">Properties</span></span>
| <span data-ttu-id="98c5c-107">属性</span><span class="sxs-lookup"><span data-stu-id="98c5c-107">Property</span></span>     | <span data-ttu-id="98c5c-108">类型</span><span class="sxs-lookup"><span data-stu-id="98c5c-108">Type</span></span>   |<span data-ttu-id="98c5c-109">说明</span><span class="sxs-lookup"><span data-stu-id="98c5c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98c5c-110">name</span><span class="sxs-lookup"><span data-stu-id="98c5c-110">name</span></span>|<span data-ttu-id="98c5c-111">string</span><span class="sxs-lookup"><span data-stu-id="98c5c-111">string</span></span>|<span data-ttu-id="98c5c-112">表示键值对中的键。</span><span class="sxs-lookup"><span data-stu-id="98c5c-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="98c5c-113">value</span><span class="sxs-lookup"><span data-stu-id="98c5c-113">value</span></span>|<span data-ttu-id="98c5c-114">string</span><span class="sxs-lookup"><span data-stu-id="98c5c-114">string</span></span>|<span data-ttu-id="98c5c-115">键值对中的值。</span><span class="sxs-lookup"><span data-stu-id="98c5c-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98c5c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98c5c-116">JSON representation</span></span>

<span data-ttu-id="98c5c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98c5c-117">Here is a JSON representation of the resource.</span></span>

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
