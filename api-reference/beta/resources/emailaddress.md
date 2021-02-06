---
title: emailAddress 资源类型
description: 表示实体实例的名称和 SMTP 地址，例如邮件收件人或日历所有者。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f572058d50672a26b3930f90a7b0492f9aa1eca
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132557"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="b7f4e-103">emailAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7f4e-103">emailAddress resource type</span></span>

<span data-ttu-id="b7f4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7f4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7f4e-105">表示实体实例的名称和 SMTP 地址，例如邮件收件人或日历所有者。</span><span class="sxs-lookup"><span data-stu-id="b7f4e-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="b7f4e-106">属性</span><span class="sxs-lookup"><span data-stu-id="b7f4e-106">Properties</span></span>
| <span data-ttu-id="b7f4e-107">属性</span><span class="sxs-lookup"><span data-stu-id="b7f4e-107">Property</span></span>     | <span data-ttu-id="b7f4e-108">类型</span><span class="sxs-lookup"><span data-stu-id="b7f4e-108">Type</span></span>   |<span data-ttu-id="b7f4e-109">说明</span><span class="sxs-lookup"><span data-stu-id="b7f4e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7f4e-110">address</span><span class="sxs-lookup"><span data-stu-id="b7f4e-110">address</span></span>|<span data-ttu-id="b7f4e-111">String</span><span class="sxs-lookup"><span data-stu-id="b7f4e-111">String</span></span>|<span data-ttu-id="b7f4e-112">实体实例的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b7f4e-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="b7f4e-113">name</span><span class="sxs-lookup"><span data-stu-id="b7f4e-113">name</span></span>|<span data-ttu-id="b7f4e-114">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f4e-114">String</span></span>|<span data-ttu-id="b7f4e-115">实体显示名称实例的一部分。</span><span class="sxs-lookup"><span data-stu-id="b7f4e-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7f4e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7f4e-116">JSON representation</span></span>

<span data-ttu-id="b7f4e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7f4e-117">Here is a JSON representation of the resource</span></span>

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


