---
title: educationOrganization 资源类型
description: 用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562802"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="55be7-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="55be7-103">educationOrganization resource type</span></span>

<span data-ttu-id="55be7-104">用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="55be7-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="55be7-105">属性</span><span class="sxs-lookup"><span data-stu-id="55be7-105">Properties</span></span>
| <span data-ttu-id="55be7-106">属性</span><span class="sxs-lookup"><span data-stu-id="55be7-106">Property</span></span>     | <span data-ttu-id="55be7-107">类型</span><span class="sxs-lookup"><span data-stu-id="55be7-107">Type</span></span>   |<span data-ttu-id="55be7-108">说明</span><span class="sxs-lookup"><span data-stu-id="55be7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55be7-109">说明</span><span class="sxs-lookup"><span data-stu-id="55be7-109">description</span></span>|<span data-ttu-id="55be7-110">String</span><span class="sxs-lookup"><span data-stu-id="55be7-110">String</span></span>| <span data-ttu-id="55be7-111">组织说明。</span><span class="sxs-lookup"><span data-stu-id="55be7-111">Organization description.</span></span>|
|<span data-ttu-id="55be7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="55be7-112">displayName</span></span>|<span data-ttu-id="55be7-113">String</span><span class="sxs-lookup"><span data-stu-id="55be7-113">String</span></span>| <span data-ttu-id="55be7-114">组织显示名称。</span><span class="sxs-lookup"><span data-stu-id="55be7-114">Organization display name.</span></span>|
|<span data-ttu-id="55be7-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="55be7-115">externalSource</span></span>|<span data-ttu-id="55be7-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="55be7-116">educationExternalSource</span></span>| <span data-ttu-id="55be7-117">从中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="55be7-117">Source where this organization was created from.</span></span> <span data-ttu-id="55be7-118">可能的值包括 `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="55be7-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55be7-119">关系</span><span class="sxs-lookup"><span data-stu-id="55be7-119">Relationships</span></span>
<span data-ttu-id="55be7-120">无。</span><span class="sxs-lookup"><span data-stu-id="55be7-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="55be7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55be7-121">JSON representation</span></span>

<span data-ttu-id="55be7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55be7-122">The following is a JSON representation of the resource.</span></span>

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
