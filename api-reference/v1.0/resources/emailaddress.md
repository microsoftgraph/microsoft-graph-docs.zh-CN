---
title: emailAddress 资源类型
description: 联系人或邮件收件人的姓名和电子邮件地址。
localization_priority: Normal
ms.openlocfilehash: 5ea1919e5c5f389c9b7fece508e8339f722b725a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826880"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="90179-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="90179-103">emailAddress resource type</span></span>

<span data-ttu-id="90179-104">联系人或邮件收件人的姓名和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="90179-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="90179-105">属性</span><span class="sxs-lookup"><span data-stu-id="90179-105">Properties</span></span>
| <span data-ttu-id="90179-106">属性</span><span class="sxs-lookup"><span data-stu-id="90179-106">Property</span></span>     | <span data-ttu-id="90179-107">类型</span><span class="sxs-lookup"><span data-stu-id="90179-107">Type</span></span>   |<span data-ttu-id="90179-108">说明</span><span class="sxs-lookup"><span data-stu-id="90179-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90179-109">address</span><span class="sxs-lookup"><span data-stu-id="90179-109">address</span></span>|<span data-ttu-id="90179-110">String</span><span class="sxs-lookup"><span data-stu-id="90179-110">String</span></span>|<span data-ttu-id="90179-111">人员或实体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="90179-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="90179-112">name</span><span class="sxs-lookup"><span data-stu-id="90179-112">name</span></span>|<span data-ttu-id="90179-113">String</span><span class="sxs-lookup"><span data-stu-id="90179-113">String</span></span>|<span data-ttu-id="90179-114">人员或实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="90179-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90179-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90179-115">JSON representation</span></span>

<span data-ttu-id="90179-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90179-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
