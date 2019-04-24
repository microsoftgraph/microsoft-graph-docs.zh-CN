---
title: emailAddress 资源类型
description: 表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc1f00ab09ac71f4f3cd9eb1aff8163a537ce257
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506725"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="bd4e4-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd4e4-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd4e4-104">表示实体实例的名称和 SMTP 地址, 例如, 邮件收件人或日历所有者。</span><span class="sxs-lookup"><span data-stu-id="bd4e4-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="bd4e4-105">属性</span><span class="sxs-lookup"><span data-stu-id="bd4e4-105">Properties</span></span>
| <span data-ttu-id="bd4e4-106">属性</span><span class="sxs-lookup"><span data-stu-id="bd4e4-106">Property</span></span>     | <span data-ttu-id="bd4e4-107">类型</span><span class="sxs-lookup"><span data-stu-id="bd4e4-107">Type</span></span>   |<span data-ttu-id="bd4e4-108">说明</span><span class="sxs-lookup"><span data-stu-id="bd4e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd4e4-109">address</span><span class="sxs-lookup"><span data-stu-id="bd4e4-109">address</span></span>|<span data-ttu-id="bd4e4-110">String</span><span class="sxs-lookup"><span data-stu-id="bd4e4-110">String</span></span>|<span data-ttu-id="bd4e4-111">实体实例的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="bd4e4-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="bd4e4-112">name</span><span class="sxs-lookup"><span data-stu-id="bd4e4-112">name</span></span>|<span data-ttu-id="bd4e4-113">String</span><span class="sxs-lookup"><span data-stu-id="bd4e4-113">String</span></span>|<span data-ttu-id="bd4e4-114">实体实例的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bd4e4-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd4e4-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd4e4-115">JSON representation</span></span>

<span data-ttu-id="bd4e4-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd4e4-116">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/emailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
