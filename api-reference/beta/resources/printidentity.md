---
title: printIdentity 资源类型
description: 表示通用打印服务中的标识。 映射到 Azure AD 组。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 45a69cbad25d2f9c3c99c9e01aa47982fe5c62b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048765"
---
# <a name="printidentity-resource-type"></a><span data-ttu-id="b5cc8-104">printIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5cc8-104">printIdentity resource type</span></span>

<span data-ttu-id="b5cc8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5cc8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5cc8-106">表示通用打印服务中的标识。</span><span class="sxs-lookup"><span data-stu-id="b5cc8-106">Represents an identity within the Universal Print service.</span></span> <span data-ttu-id="b5cc8-107">映射到 [Azure Active Directory (AZURE AD) 组](group.md)。</span><span class="sxs-lookup"><span data-stu-id="b5cc8-107">Maps to an [Azure Active Directory (Azure AD) group](group.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b5cc8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5cc8-108">Properties</span></span>
| <span data-ttu-id="b5cc8-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5cc8-109">Property</span></span>     | <span data-ttu-id="b5cc8-110">类型</span><span class="sxs-lookup"><span data-stu-id="b5cc8-110">Type</span></span>        | <span data-ttu-id="b5cc8-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5cc8-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5cc8-112">id</span><span class="sxs-lookup"><span data-stu-id="b5cc8-112">id</span></span>|<span data-ttu-id="b5cc8-113">String</span><span class="sxs-lookup"><span data-stu-id="b5cc8-113">String</span></span>|<span data-ttu-id="b5cc8-114">PrintIdentity 的标识符。</span><span class="sxs-lookup"><span data-stu-id="b5cc8-114">The printIdentity's identifier.</span></span> <span data-ttu-id="b5cc8-115">只读。</span><span class="sxs-lookup"><span data-stu-id="b5cc8-115">Read-only.</span></span>|
|<span data-ttu-id="b5cc8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="b5cc8-116">displayName</span></span>|<span data-ttu-id="b5cc8-117">String</span><span class="sxs-lookup"><span data-stu-id="b5cc8-117">String</span></span>|<span data-ttu-id="b5cc8-118">PrintIdentity 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b5cc8-118">The printIdentity's display name.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5cc8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5cc8-119">JSON representation</span></span>

<span data-ttu-id="b5cc8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5cc8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


