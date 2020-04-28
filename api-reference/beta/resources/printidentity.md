---
title: printIdentity 资源类型
description: 表示通用打印服务中的标识。 映射到 Azure AD 组。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4ac0695357aba0ba6c44fef4654d2edaefca6cb
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917599"
---
# <a name="printidentity-resource-type"></a><span data-ttu-id="eaf8b-104">printIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="eaf8b-104">printIdentity resource type</span></span>

<span data-ttu-id="eaf8b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaf8b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaf8b-106">表示通用打印服务中的标识。</span><span class="sxs-lookup"><span data-stu-id="eaf8b-106">Represents an identity within the Universal Print service.</span></span> <span data-ttu-id="eaf8b-107">映射到[Azure Active Directory （AZURE AD）组](group.md)。</span><span class="sxs-lookup"><span data-stu-id="eaf8b-107">Maps to an [Azure Active Directory (Azure AD) group](group.md).</span></span>

## <a name="properties"></a><span data-ttu-id="eaf8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="eaf8b-108">Properties</span></span>
| <span data-ttu-id="eaf8b-109">属性</span><span class="sxs-lookup"><span data-stu-id="eaf8b-109">Property</span></span>     | <span data-ttu-id="eaf8b-110">类型</span><span class="sxs-lookup"><span data-stu-id="eaf8b-110">Type</span></span>        | <span data-ttu-id="eaf8b-111">说明</span><span class="sxs-lookup"><span data-stu-id="eaf8b-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eaf8b-112">id</span><span class="sxs-lookup"><span data-stu-id="eaf8b-112">id</span></span>|<span data-ttu-id="eaf8b-113">String</span><span class="sxs-lookup"><span data-stu-id="eaf8b-113">String</span></span>|<span data-ttu-id="eaf8b-114">PrintIdentity 的标识符。</span><span class="sxs-lookup"><span data-stu-id="eaf8b-114">The printIdentity's identifier.</span></span> <span data-ttu-id="eaf8b-115">只读。</span><span class="sxs-lookup"><span data-stu-id="eaf8b-115">Read-only.</span></span>|
|<span data-ttu-id="eaf8b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="eaf8b-116">displayName</span></span>|<span data-ttu-id="eaf8b-117">String</span><span class="sxs-lookup"><span data-stu-id="eaf8b-117">String</span></span>|<span data-ttu-id="eaf8b-118">PrintIdentity 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eaf8b-118">The printIdentity's display name.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eaf8b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eaf8b-119">JSON representation</span></span>

<span data-ttu-id="eaf8b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaf8b-120">The following is a JSON representation of the resource.</span></span>

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
