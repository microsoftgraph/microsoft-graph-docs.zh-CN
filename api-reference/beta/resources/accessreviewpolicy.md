---
title: accessReviewPolicy 资源类型
description: 访问评审策略是使组织能够管理目录级别访问评审策略的单一单位。
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 02940987682d84aa3fc3dbb076c998abfe24bf8e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067873"
---
# <a name="accessreviewpolicy-resource-type"></a><span data-ttu-id="ed22e-103">accessReviewPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed22e-103">accessReviewPolicy resource type</span></span>

<span data-ttu-id="ed22e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed22e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed22e-105">访问评审策略是使管理员能够管理目录级别访问评审策略的单一文件。</span><span class="sxs-lookup"><span data-stu-id="ed22e-105">Access review policy is a singleton that enables administrators to manage directory-level access review policies.</span></span> <span data-ttu-id="ed22e-106">例如，管理员可以使用访问评审策略启用和禁用组所有者在自己拥有的组上创建访问评审的能力。</span><span class="sxs-lookup"><span data-stu-id="ed22e-106">For example, administrators can use the access review policy to enable and disable the ability of group owners to create access reviews on groups that they own.</span></span>


<span data-ttu-id="ed22e-107">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="ed22e-107">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ed22e-108">方法</span><span class="sxs-lookup"><span data-stu-id="ed22e-108">Methods</span></span>
|<span data-ttu-id="ed22e-109">方法</span><span class="sxs-lookup"><span data-stu-id="ed22e-109">Method</span></span>|<span data-ttu-id="ed22e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed22e-110">Return type</span></span>|<span data-ttu-id="ed22e-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed22e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed22e-112">获取 accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="ed22e-112">Get accessReviewPolicy</span></span>](../api/accessreviewpolicy-get.md)|[<span data-ttu-id="ed22e-113">accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="ed22e-113">accessReviewPolicy</span></span>](../resources/accessreviewpolicy.md)|<span data-ttu-id="ed22e-114">读取 [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed22e-114">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>|
|[<span data-ttu-id="ed22e-115">更新 accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="ed22e-115">Update accessReviewPolicy</span></span>](../api/accessreviewpolicy-update.md)|[<span data-ttu-id="ed22e-116">accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="ed22e-116">accessReviewPolicy</span></span>](../resources/accessreviewpolicy.md)|<span data-ttu-id="ed22e-117">更新 [accessReviewPolicy 对象](../resources/accessreviewpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ed22e-117">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed22e-118">属性</span><span class="sxs-lookup"><span data-stu-id="ed22e-118">Properties</span></span>
|<span data-ttu-id="ed22e-119">属性</span><span class="sxs-lookup"><span data-stu-id="ed22e-119">Property</span></span>|<span data-ttu-id="ed22e-120">类型</span><span class="sxs-lookup"><span data-stu-id="ed22e-120">Type</span></span>|<span data-ttu-id="ed22e-121">说明</span><span class="sxs-lookup"><span data-stu-id="ed22e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed22e-122">说明</span><span class="sxs-lookup"><span data-stu-id="ed22e-122">description</span></span>|<span data-ttu-id="ed22e-123">String</span><span class="sxs-lookup"><span data-stu-id="ed22e-123">String</span></span>|<span data-ttu-id="ed22e-124">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="ed22e-124">Description for this policy.</span></span> <span data-ttu-id="ed22e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="ed22e-125">Read-only.</span></span>|
|<span data-ttu-id="ed22e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="ed22e-126">displayName</span></span>|<span data-ttu-id="ed22e-127">String</span><span class="sxs-lookup"><span data-stu-id="ed22e-127">String</span></span>|<span data-ttu-id="ed22e-128">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ed22e-128">Display name for this policy.</span></span> <span data-ttu-id="ed22e-129">只读。</span><span class="sxs-lookup"><span data-stu-id="ed22e-129">Read-only.</span></span>|
|<span data-ttu-id="ed22e-130">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="ed22e-130">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="ed22e-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="ed22e-131">Boolean</span></span>|<span data-ttu-id="ed22e-132">如果 `true` 为 ，组所有者可以在他们拥有的组上创建和管理访问评审。</span><span class="sxs-lookup"><span data-stu-id="ed22e-132">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed22e-133">关系</span><span class="sxs-lookup"><span data-stu-id="ed22e-133">Relationships</span></span>
<span data-ttu-id="ed22e-134">无。</span><span class="sxs-lookup"><span data-stu-id="ed22e-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed22e-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed22e-135">JSON representation</span></span>
<span data-ttu-id="ed22e-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed22e-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewPolicy",
  "displayName": "Access Review Policy",
  "description": "Policy contains directory-level access review settings.",
  "isGroupOwnerManagementEnabled": false
}
```
