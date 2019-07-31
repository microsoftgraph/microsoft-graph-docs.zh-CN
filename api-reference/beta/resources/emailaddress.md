---
title: emailAddress 资源类型
description: 表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4f0b36d84ffba5c5a8e39bd7603f92c815cda008
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972213"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="1170f-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="1170f-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1170f-104">表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。</span><span class="sxs-lookup"><span data-stu-id="1170f-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="1170f-105">属性</span><span class="sxs-lookup"><span data-stu-id="1170f-105">Properties</span></span>
| <span data-ttu-id="1170f-106">属性</span><span class="sxs-lookup"><span data-stu-id="1170f-106">Property</span></span>     | <span data-ttu-id="1170f-107">类型</span><span class="sxs-lookup"><span data-stu-id="1170f-107">Type</span></span>   |<span data-ttu-id="1170f-108">说明</span><span class="sxs-lookup"><span data-stu-id="1170f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1170f-109">address</span><span class="sxs-lookup"><span data-stu-id="1170f-109">address</span></span>|<span data-ttu-id="1170f-110">String</span><span class="sxs-lookup"><span data-stu-id="1170f-110">String</span></span>|<span data-ttu-id="1170f-111">实体实例的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1170f-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="1170f-112">name</span><span class="sxs-lookup"><span data-stu-id="1170f-112">name</span></span>|<span data-ttu-id="1170f-113">String</span><span class="sxs-lookup"><span data-stu-id="1170f-113">String</span></span>|<span data-ttu-id="1170f-114">实体实例的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1170f-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1170f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1170f-115">JSON representation</span></span>

<span data-ttu-id="1170f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1170f-116">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
