---
title: emailAddress 资源类型
description: 联系人或邮件收件人的姓名和电子邮件地址。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 055f4d426e475156469f3b3cd8ba9eca87102495
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132805"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="6fc46-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fc46-103">emailAddress resource type</span></span>

<span data-ttu-id="6fc46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fc46-105">联系人或邮件收件人的姓名和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6fc46-105">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="6fc46-106">属性</span><span class="sxs-lookup"><span data-stu-id="6fc46-106">Properties</span></span>
| <span data-ttu-id="6fc46-107">属性</span><span class="sxs-lookup"><span data-stu-id="6fc46-107">Property</span></span>     | <span data-ttu-id="6fc46-108">类型</span><span class="sxs-lookup"><span data-stu-id="6fc46-108">Type</span></span>   |<span data-ttu-id="6fc46-109">说明</span><span class="sxs-lookup"><span data-stu-id="6fc46-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fc46-110">address</span><span class="sxs-lookup"><span data-stu-id="6fc46-110">address</span></span>|<span data-ttu-id="6fc46-111">String</span><span class="sxs-lookup"><span data-stu-id="6fc46-111">String</span></span>|<span data-ttu-id="6fc46-112">人员或实体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6fc46-112">The email address of the person or entity.</span></span>|
|<span data-ttu-id="6fc46-113">name</span><span class="sxs-lookup"><span data-stu-id="6fc46-113">name</span></span>|<span data-ttu-id="6fc46-114">String</span><span class="sxs-lookup"><span data-stu-id="6fc46-114">String</span></span>|<span data-ttu-id="6fc46-115">人员或实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6fc46-115">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc46-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fc46-116">JSON representation</span></span>

<span data-ttu-id="6fc46-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc46-117">Here is a JSON representation of the resource</span></span>

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

