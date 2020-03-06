---
title: educationOrganization 资源类型
description: 用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a6e32f7bf9c635423ca1aace92aea160f6cc2706
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531525"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="6b5e7-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b5e7-103">educationOrganization resource type</span></span>

<span data-ttu-id="6b5e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b5e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b5e7-105">用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="6b5e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b5e7-106">Properties</span></span>
| <span data-ttu-id="6b5e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b5e7-107">Property</span></span>     | <span data-ttu-id="6b5e7-108">类型</span><span class="sxs-lookup"><span data-stu-id="6b5e7-108">Type</span></span>   |<span data-ttu-id="6b5e7-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b5e7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b5e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="6b5e7-110">description</span></span>|<span data-ttu-id="6b5e7-111">字符串</span><span class="sxs-lookup"><span data-stu-id="6b5e7-111">String</span></span>| <span data-ttu-id="6b5e7-112">组织说明。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-112">Organization description.</span></span>|
|<span data-ttu-id="6b5e7-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6b5e7-113">displayName</span></span>|<span data-ttu-id="6b5e7-114">String</span><span class="sxs-lookup"><span data-stu-id="6b5e7-114">String</span></span>| <span data-ttu-id="6b5e7-115">组织显示名称。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-115">Organization display name.</span></span>|
|<span data-ttu-id="6b5e7-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="6b5e7-116">externalSource</span></span>|<span data-ttu-id="6b5e7-117">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="6b5e7-117">educationExternalSource</span></span>| <span data-ttu-id="6b5e7-118">从中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-118">Source where this organization was created from.</span></span> <span data-ttu-id="6b5e7-119">可能的值包括 `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-119">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b5e7-120">关系</span><span class="sxs-lookup"><span data-stu-id="6b5e7-120">Relationships</span></span>
<span data-ttu-id="6b5e7-121">无。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-121">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b5e7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b5e7-122">JSON representation</span></span>

<span data-ttu-id="6b5e7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b5e7-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
