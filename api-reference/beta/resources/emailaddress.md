---
title: emailAddress 资源类型
description: 表示实体实例的名称和 SMTP 地址，例如，邮件收件人或日历所有者。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d2a43300922ddf88df908d39d82b6efde2369348
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979488"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="c553a-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="c553a-103">emailAddress resource type</span></span>

<span data-ttu-id="c553a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c553a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c553a-105">表示实体实例的名称和 SMTP 地址，例如，邮件收件人或日历所有者。</span><span class="sxs-lookup"><span data-stu-id="c553a-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="c553a-106">属性</span><span class="sxs-lookup"><span data-stu-id="c553a-106">Properties</span></span>
| <span data-ttu-id="c553a-107">属性</span><span class="sxs-lookup"><span data-stu-id="c553a-107">Property</span></span>     | <span data-ttu-id="c553a-108">类型</span><span class="sxs-lookup"><span data-stu-id="c553a-108">Type</span></span>   |<span data-ttu-id="c553a-109">说明</span><span class="sxs-lookup"><span data-stu-id="c553a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c553a-110">address</span><span class="sxs-lookup"><span data-stu-id="c553a-110">address</span></span>|<span data-ttu-id="c553a-111">String</span><span class="sxs-lookup"><span data-stu-id="c553a-111">String</span></span>|<span data-ttu-id="c553a-112">实体实例的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c553a-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="c553a-113">name</span><span class="sxs-lookup"><span data-stu-id="c553a-113">name</span></span>|<span data-ttu-id="c553a-114">String</span><span class="sxs-lookup"><span data-stu-id="c553a-114">String</span></span>|<span data-ttu-id="c553a-115">实体实例的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c553a-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c553a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c553a-116">JSON representation</span></span>

<span data-ttu-id="c553a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c553a-117">Here is a JSON representation of the resource</span></span>

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


