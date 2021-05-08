---
title: educationOrganization 资源类型
description: 抽象实体，用于对教育部门内不同组织类型之间的通用性进行建模。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24313b6b6061449faea0ecb4880a421a2333099
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231862"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="c58ee-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="c58ee-103">educationOrganization resource type</span></span>

<span data-ttu-id="c58ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c58ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c58ee-105">抽象实体，用于对教育部门内不同组织类型之间的通用性进行建模。</span><span class="sxs-lookup"><span data-stu-id="c58ee-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

<span data-ttu-id="c58ee-106">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="c58ee-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c58ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="c58ee-107">Properties</span></span>

| <span data-ttu-id="c58ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="c58ee-108">Property</span></span>             | <span data-ttu-id="c58ee-109">类型</span><span class="sxs-lookup"><span data-stu-id="c58ee-109">Type</span></span>                    | <span data-ttu-id="c58ee-110">说明</span><span class="sxs-lookup"><span data-stu-id="c58ee-110">Description</span></span>                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="c58ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="c58ee-111">description</span></span>          | <span data-ttu-id="c58ee-112">String</span><span class="sxs-lookup"><span data-stu-id="c58ee-112">String</span></span>                  | <span data-ttu-id="c58ee-113">组织说明。</span><span class="sxs-lookup"><span data-stu-id="c58ee-113">Organization description.</span></span>                                                              |
| <span data-ttu-id="c58ee-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c58ee-114">displayName</span></span>          | <span data-ttu-id="c58ee-115">String</span><span class="sxs-lookup"><span data-stu-id="c58ee-115">String</span></span>                  | <span data-ttu-id="c58ee-116">组织显示名称。</span><span class="sxs-lookup"><span data-stu-id="c58ee-116">Organization display name.</span></span>                                                             |
| <span data-ttu-id="c58ee-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="c58ee-117">externalSource</span></span>       | <span data-ttu-id="c58ee-118">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="c58ee-118">educationExternalSource</span></span> | <span data-ttu-id="c58ee-119">创建组织的来源。</span><span class="sxs-lookup"><span data-stu-id="c58ee-119">Source where this organization was created from.</span></span> <span data-ttu-id="c58ee-120">可取值为：`sis`、`manual`。</span><span class="sxs-lookup"><span data-stu-id="c58ee-120">Possible values are: `sis`, `manual`.</span></span> |
| <span data-ttu-id="c58ee-121">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="c58ee-121">externalSourceDetail</span></span> | <span data-ttu-id="c58ee-122">String</span><span class="sxs-lookup"><span data-stu-id="c58ee-122">String</span></span>                  | <span data-ttu-id="c58ee-123">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="c58ee-123">The name of the external source this resources was generated from.</span></span>                     |
| <span data-ttu-id="c58ee-124">id</span><span class="sxs-lookup"><span data-stu-id="c58ee-124">id</span></span>                   | <span data-ttu-id="c58ee-125">String</span><span class="sxs-lookup"><span data-stu-id="c58ee-125">String</span></span>                  | <span data-ttu-id="c58ee-126">对象标识符。</span><span class="sxs-lookup"><span data-stu-id="c58ee-126">Object identifier.</span></span> <span data-ttu-id="c58ee-127">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="c58ee-127">Inherited from [entity](../resources/entity.md)</span></span>                     |

## <a name="relationships"></a><span data-ttu-id="c58ee-128">关系</span><span class="sxs-lookup"><span data-stu-id="c58ee-128">Relationships</span></span>

<span data-ttu-id="c58ee-129">无。</span><span class="sxs-lookup"><span data-stu-id="c58ee-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c58ee-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c58ee-130">JSON representation</span></span>

<span data-ttu-id="c58ee-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c58ee-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String"
}
```
