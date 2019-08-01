---
title: emailAddress 资源类型
description: 联系人或邮件收件人的姓名和电子邮件地址。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3b6bddb5436408fa38c931cd7e1e1f5503979e5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032590"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="288f6-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="288f6-103">emailAddress resource type</span></span>

<span data-ttu-id="288f6-104">联系人或邮件收件人的姓名和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="288f6-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="288f6-105">属性</span><span class="sxs-lookup"><span data-stu-id="288f6-105">Properties</span></span>
| <span data-ttu-id="288f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="288f6-106">Property</span></span>     | <span data-ttu-id="288f6-107">类型</span><span class="sxs-lookup"><span data-stu-id="288f6-107">Type</span></span>   |<span data-ttu-id="288f6-108">说明</span><span class="sxs-lookup"><span data-stu-id="288f6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="288f6-109">address</span><span class="sxs-lookup"><span data-stu-id="288f6-109">address</span></span>|<span data-ttu-id="288f6-110">String</span><span class="sxs-lookup"><span data-stu-id="288f6-110">String</span></span>|<span data-ttu-id="288f6-111">人员或实体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="288f6-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="288f6-112">name</span><span class="sxs-lookup"><span data-stu-id="288f6-112">name</span></span>|<span data-ttu-id="288f6-113">String</span><span class="sxs-lookup"><span data-stu-id="288f6-113">String</span></span>|<span data-ttu-id="288f6-114">人员或实体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="288f6-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="288f6-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="288f6-115">JSON representation</span></span>

<span data-ttu-id="288f6-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="288f6-116">Here is a JSON representation of the resource</span></span>

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
