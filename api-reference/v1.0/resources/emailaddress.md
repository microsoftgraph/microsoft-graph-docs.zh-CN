---
title: emailAddress 资源类型
description: 联系人或邮件收件人的姓名和电子邮件地址。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7af23418132c4d1c20097899f870c7d25be119bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555907"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="321ca-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="321ca-103">emailAddress resource type</span></span>

<span data-ttu-id="321ca-104">联系人或邮件收件人的姓名和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="321ca-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="321ca-105">属性</span><span class="sxs-lookup"><span data-stu-id="321ca-105">Properties</span></span>
| <span data-ttu-id="321ca-106">属性</span><span class="sxs-lookup"><span data-stu-id="321ca-106">Property</span></span>     | <span data-ttu-id="321ca-107">类型</span><span class="sxs-lookup"><span data-stu-id="321ca-107">Type</span></span>   |<span data-ttu-id="321ca-108">说明</span><span class="sxs-lookup"><span data-stu-id="321ca-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="321ca-109">address</span><span class="sxs-lookup"><span data-stu-id="321ca-109">address</span></span>|<span data-ttu-id="321ca-110">String</span><span class="sxs-lookup"><span data-stu-id="321ca-110">String</span></span>|<span data-ttu-id="321ca-111">人员或实体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="321ca-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="321ca-112">name</span><span class="sxs-lookup"><span data-stu-id="321ca-112">name</span></span>|<span data-ttu-id="321ca-113">String</span><span class="sxs-lookup"><span data-stu-id="321ca-113">String</span></span>|<span data-ttu-id="321ca-114">人员或实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="321ca-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="321ca-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="321ca-115">JSON representation</span></span>

<span data-ttu-id="321ca-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="321ca-116">Here is a JSON representation of the resource</span></span>

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
