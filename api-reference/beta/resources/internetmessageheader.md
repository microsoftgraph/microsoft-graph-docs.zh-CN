---
title: internetMessageHeader 资源类型
description: '表示 Internet 邮件头（由 RFC5322 定义）的键/值对，可提供 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 29fbef55b1c1e7e8c948c85a283cf27a1f74ffc6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808779"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="481e0-103">internetMessageHeader 资源类型</span><span class="sxs-lookup"><span data-stu-id="481e0-103">internetMessageHeader resource type</span></span>

<span data-ttu-id="481e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="481e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="481e0-105">一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。</span><span class="sxs-lookup"><span data-stu-id="481e0-105">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span>

<span data-ttu-id="481e0-106">有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。</span><span class="sxs-lookup"><span data-stu-id="481e0-106">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="481e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="481e0-107">Properties</span></span>
| <span data-ttu-id="481e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="481e0-108">Property</span></span>     | <span data-ttu-id="481e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="481e0-109">Type</span></span>   |<span data-ttu-id="481e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="481e0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="481e0-111">name</span><span class="sxs-lookup"><span data-stu-id="481e0-111">name</span></span>|<span data-ttu-id="481e0-112">string</span><span class="sxs-lookup"><span data-stu-id="481e0-112">string</span></span>|<span data-ttu-id="481e0-113">表示键值对中的键。</span><span class="sxs-lookup"><span data-stu-id="481e0-113">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="481e0-114">value</span><span class="sxs-lookup"><span data-stu-id="481e0-114">value</span></span>|<span data-ttu-id="481e0-115">string</span><span class="sxs-lookup"><span data-stu-id="481e0-115">string</span></span>|<span data-ttu-id="481e0-116">键值对中的值。</span><span class="sxs-lookup"><span data-stu-id="481e0-116">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="481e0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="481e0-117">JSON representation</span></span>

<span data-ttu-id="481e0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="481e0-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
