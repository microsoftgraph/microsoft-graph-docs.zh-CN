---
title: educationOrganization 资源类型
description: '用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 49afe12f4897df80ce78ba28a024883cefeb0a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340476"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="9b26b-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b26b-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b26b-104">用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="9b26b-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="9b26b-105">属性</span><span class="sxs-lookup"><span data-stu-id="9b26b-105">Properties</span></span>
| <span data-ttu-id="9b26b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9b26b-106">Property</span></span>     | <span data-ttu-id="9b26b-107">类型</span><span class="sxs-lookup"><span data-stu-id="9b26b-107">Type</span></span>   |<span data-ttu-id="9b26b-108">说明</span><span class="sxs-lookup"><span data-stu-id="9b26b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b26b-109">说明</span><span class="sxs-lookup"><span data-stu-id="9b26b-109">description</span></span>|<span data-ttu-id="9b26b-110">String</span><span class="sxs-lookup"><span data-stu-id="9b26b-110">String</span></span>| <span data-ttu-id="9b26b-111">组织说明。</span><span class="sxs-lookup"><span data-stu-id="9b26b-111">Organization description.</span></span>|
|<span data-ttu-id="9b26b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9b26b-112">displayName</span></span>|<span data-ttu-id="9b26b-113">String</span><span class="sxs-lookup"><span data-stu-id="9b26b-113">String</span></span>| <span data-ttu-id="9b26b-114">组织显示名称。</span><span class="sxs-lookup"><span data-stu-id="9b26b-114">Organization display name.</span></span>|
|<span data-ttu-id="9b26b-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="9b26b-115">externalSource</span></span>|<span data-ttu-id="9b26b-116">string</span><span class="sxs-lookup"><span data-stu-id="9b26b-116">string</span></span>| <span data-ttu-id="9b26b-117">从中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="9b26b-117">Source where this organization was created from.</span></span> <span data-ttu-id="9b26b-118">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b26b-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b26b-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="9b26b-119">Relationships</span></span>
<span data-ttu-id="9b26b-120">无。</span><span class="sxs-lookup"><span data-stu-id="9b26b-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b26b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b26b-121">JSON representation</span></span>

<span data-ttu-id="9b26b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b26b-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
