---
title: itemFacet 资源类型
description: itemFacet 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ff186b8b78e0070b5f92efa1858ef8d15d51c59f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021432"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="1b918-103">itemFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b918-103">itemFacet resource type</span></span>

<span data-ttu-id="1b918-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b918-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b918-105">表示 [配置文件](profile.md) entityset 中的所有资源类型继承自的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="1b918-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="1b918-106">属性</span><span class="sxs-lookup"><span data-stu-id="1b918-106">Properties</span></span>
|<span data-ttu-id="1b918-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b918-107">Property</span></span>|<span data-ttu-id="1b918-108">类型</span><span class="sxs-lookup"><span data-stu-id="1b918-108">Type</span></span>|<span data-ttu-id="1b918-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b918-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b918-110">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1b918-110">allowedAudiences</span></span>|<span data-ttu-id="1b918-111">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="1b918-111">allowedAudiences</span></span>|<span data-ttu-id="1b918-112">能够查看关联实体内包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="1b918-112">The audiences that are able to see the values contained within the associated entity.</span></span> <span data-ttu-id="1b918-113">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1b918-113">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1b918-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="1b918-114">createdBy</span></span>|[<span data-ttu-id="1b918-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b918-115">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="1b918-116">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="1b918-116">Provides the identifier of the user and/or application that created the entity.</span></span>|
|<span data-ttu-id="1b918-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b918-117">createdDateTime</span></span>|<span data-ttu-id="1b918-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b918-118">DateTimeOffset</span></span>|<span data-ttu-id="1b918-119">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="1b918-119">Provides the dateTimeOffset for when the entity was created.</span></span>|
|<span data-ttu-id="1b918-120">id</span><span class="sxs-lookup"><span data-stu-id="1b918-120">id</span></span>|<span data-ttu-id="1b918-121">String</span><span class="sxs-lookup"><span data-stu-id="1b918-121">String</span></span>|<span data-ttu-id="1b918-122">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="1b918-122">Identifier used for individually addressing an entity.</span></span> <span data-ttu-id="1b918-123">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="1b918-123">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="1b918-124">推导</span><span class="sxs-lookup"><span data-stu-id="1b918-124">inference</span></span>|[<span data-ttu-id="1b918-125">inferenceData</span><span class="sxs-lookup"><span data-stu-id="1b918-125">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1b918-126">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="1b918-126">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span>|
|<span data-ttu-id="1b918-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1b918-127">lastModifiedBy</span></span>|[<span data-ttu-id="1b918-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b918-128">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="1b918-129">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="1b918-129">Provides the identifier of the user and/or application that last modified the entity.</span></span>|
|<span data-ttu-id="1b918-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b918-130">lastModifiedDateTime</span></span>|<span data-ttu-id="1b918-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b918-131">DateTimeOffset</span></span>|<span data-ttu-id="1b918-132">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="1b918-132">Provides the dateTimeOffset for when the entity was created.</span></span>|
|<span data-ttu-id="1b918-133">source</span><span class="sxs-lookup"><span data-stu-id="1b918-133">source</span></span>|[<span data-ttu-id="1b918-134">personDataSource</span><span class="sxs-lookup"><span data-stu-id="1b918-134">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="1b918-135">实体中的值的起源（如果从另一个服务同步）。</span><span class="sxs-lookup"><span data-stu-id="1b918-135">Where the values within an entity originated if synced from another service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b918-136">关系</span><span class="sxs-lookup"><span data-stu-id="1b918-136">Relationships</span></span>
<span data-ttu-id="1b918-137">无。</span><span class="sxs-lookup"><span data-stu-id="1b918-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b918-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b918-138">JSON representation</span></span>
<span data-ttu-id="1b918-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b918-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemFacet",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  }
}
```



