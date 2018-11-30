---
title: internetMessageHeader 资源类型
description: '表示由 RFC5322，提供定义 Internet 邮件头，键 / 值对 '
ms.openlocfilehash: 420d39b6a139563e3f5f277f032f0f7a29252337
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044576"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="18ca4-103">internetMessageHeader 资源类型</span><span class="sxs-lookup"><span data-stu-id="18ca4-103">internetMessageHeader resource type</span></span>

> <span data-ttu-id="18ca4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="18ca4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18ca4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="18ca4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18ca4-106">一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。</span><span class="sxs-lookup"><span data-stu-id="18ca4-106">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="18ca4-107">有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。</span><span class="sxs-lookup"><span data-stu-id="18ca4-107">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="18ca4-108">属性</span><span class="sxs-lookup"><span data-stu-id="18ca4-108">Properties</span></span>
| <span data-ttu-id="18ca4-109">属性</span><span class="sxs-lookup"><span data-stu-id="18ca4-109">Property</span></span>     | <span data-ttu-id="18ca4-110">类型</span><span class="sxs-lookup"><span data-stu-id="18ca4-110">Type</span></span>   |<span data-ttu-id="18ca4-111">说明</span><span class="sxs-lookup"><span data-stu-id="18ca4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18ca4-112">name</span><span class="sxs-lookup"><span data-stu-id="18ca4-112">name</span></span>|<span data-ttu-id="18ca4-113">string</span><span class="sxs-lookup"><span data-stu-id="18ca4-113">string</span></span>|<span data-ttu-id="18ca4-114">表示键值对中的键。</span><span class="sxs-lookup"><span data-stu-id="18ca4-114">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="18ca4-115">value</span><span class="sxs-lookup"><span data-stu-id="18ca4-115">value</span></span>|<span data-ttu-id="18ca4-116">string</span><span class="sxs-lookup"><span data-stu-id="18ca4-116">string</span></span>|<span data-ttu-id="18ca4-117">键值对中的值。</span><span class="sxs-lookup"><span data-stu-id="18ca4-117">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18ca4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18ca4-118">JSON representation</span></span>

<span data-ttu-id="18ca4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18ca4-119">Here is a JSON representation of the resource.</span></span>

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