---
title: emailAddress 资源类型
description: 联系人或邮件收件人的姓名和电子邮件地址。
ms.openlocfilehash: 962b2f36af9e292125edc3da8606cd532b8c2ec0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007957"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="03dea-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="03dea-103">emailAddress resource type</span></span>

<span data-ttu-id="03dea-104">联系人或邮件收件人的姓名和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="03dea-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="03dea-105">属性</span><span class="sxs-lookup"><span data-stu-id="03dea-105">Properties</span></span>
| <span data-ttu-id="03dea-106">属性</span><span class="sxs-lookup"><span data-stu-id="03dea-106">Property</span></span>     | <span data-ttu-id="03dea-107">类型</span><span class="sxs-lookup"><span data-stu-id="03dea-107">Type</span></span>   |<span data-ttu-id="03dea-108">说明</span><span class="sxs-lookup"><span data-stu-id="03dea-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03dea-109">address</span><span class="sxs-lookup"><span data-stu-id="03dea-109">address</span></span>|<span data-ttu-id="03dea-110">String</span><span class="sxs-lookup"><span data-stu-id="03dea-110">String</span></span>|<span data-ttu-id="03dea-111">人员或实体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="03dea-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="03dea-112">name</span><span class="sxs-lookup"><span data-stu-id="03dea-112">name</span></span>|<span data-ttu-id="03dea-113">String</span><span class="sxs-lookup"><span data-stu-id="03dea-113">String</span></span>|<span data-ttu-id="03dea-114">人员或实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="03dea-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03dea-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03dea-115">JSON representation</span></span>

<span data-ttu-id="03dea-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03dea-116">Here is a JSON representation of the resource</span></span>

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
