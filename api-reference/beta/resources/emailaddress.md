---
title: emailAddress 资源类型
description: 表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8b49e0ff502f6e36e6ca3291d675c839e9ff5e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340303"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="f3f88-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3f88-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3f88-104">表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。</span><span class="sxs-lookup"><span data-stu-id="f3f88-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="f3f88-105">属性</span><span class="sxs-lookup"><span data-stu-id="f3f88-105">Properties</span></span>
| <span data-ttu-id="f3f88-106">属性</span><span class="sxs-lookup"><span data-stu-id="f3f88-106">Property</span></span>     | <span data-ttu-id="f3f88-107">类型</span><span class="sxs-lookup"><span data-stu-id="f3f88-107">Type</span></span>   |<span data-ttu-id="f3f88-108">说明</span><span class="sxs-lookup"><span data-stu-id="f3f88-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3f88-109">address</span><span class="sxs-lookup"><span data-stu-id="f3f88-109">address</span></span>|<span data-ttu-id="f3f88-110">String</span><span class="sxs-lookup"><span data-stu-id="f3f88-110">String</span></span>|<span data-ttu-id="f3f88-111">实体实例的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f3f88-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="f3f88-112">name</span><span class="sxs-lookup"><span data-stu-id="f3f88-112">name</span></span>|<span data-ttu-id="f3f88-113">String</span><span class="sxs-lookup"><span data-stu-id="f3f88-113">String</span></span>|<span data-ttu-id="f3f88-114">实体实例的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f3f88-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3f88-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3f88-115">JSON representation</span></span>

<span data-ttu-id="f3f88-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3f88-116">Here is a JSON representation of the resource</span></span>

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
