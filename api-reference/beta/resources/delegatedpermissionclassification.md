---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f3d35c11ffe29feafed025b95c8f221e4f9ee4cb
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921730"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="54a13-103">delegatedPermissionClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="54a13-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="54a13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54a13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54a13-105">用于指定委派权限的分类。</span><span class="sxs-lookup"><span data-stu-id="54a13-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="54a13-106">委派权限分类可与用户同意设置结合使用，以选择允许用户同意的权限。</span><span class="sxs-lookup"><span data-stu-id="54a13-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="54a13-107">请参阅 [配置最终用户同意应用程序的方式](/azure/active-directory/manage-apps/configure-user-consent) ，以了解有关权限分类的详细信息。</span><span class="sxs-lookup"><span data-stu-id="54a13-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="54a13-108">属性</span><span class="sxs-lookup"><span data-stu-id="54a13-108">Properties</span></span>

| <span data-ttu-id="54a13-109">属性</span><span class="sxs-lookup"><span data-stu-id="54a13-109">Property</span></span> | <span data-ttu-id="54a13-110">类型</span><span class="sxs-lookup"><span data-stu-id="54a13-110">Type</span></span> | <span data-ttu-id="54a13-111">说明</span><span class="sxs-lookup"><span data-stu-id="54a13-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="54a13-112">id</span><span class="sxs-lookup"><span data-stu-id="54a13-112">id</span></span> | <span data-ttu-id="54a13-113">String</span><span class="sxs-lookup"><span data-stu-id="54a13-113">String</span></span> | <span data-ttu-id="54a13-114">**DelegatedPermissionClassification** 项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="54a13-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="54a13-115">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="54a13-115">Not nullable.</span></span> <span data-ttu-id="54a13-116">只读。</span><span class="sxs-lookup"><span data-stu-id="54a13-116">Read-only.</span></span> |
| <span data-ttu-id="54a13-117">classification</span><span class="sxs-lookup"><span data-stu-id="54a13-117">classification</span></span> | <span data-ttu-id="54a13-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="54a13-118">permissionClassificationType</span></span> | <span data-ttu-id="54a13-119">所提供的分类值。</span><span class="sxs-lookup"><span data-stu-id="54a13-119">The classification value being given.</span></span> <span data-ttu-id="54a13-120">可能的值： `low` 。</span><span class="sxs-lookup"><span data-stu-id="54a13-120">Possible value: `low`.</span></span> <span data-ttu-id="54a13-121">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="54a13-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="54a13-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="54a13-122">permissionId</span></span> | <span data-ttu-id="54a13-123">Guid</span><span class="sxs-lookup"><span data-stu-id="54a13-123">Guid</span></span> | <span data-ttu-id="54a13-124">[ServicePrincipal](servicePrincipal.md)的 **publishedPermissionScopes** 集合中列出的委派权限 ( **id** ) 唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="54a13-124">The unique identifier ( **id** ) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="54a13-125">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="54a13-125">Required on create.</span></span> <span data-ttu-id="54a13-126">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="54a13-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="54a13-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="54a13-127">permissionName</span></span> | <span data-ttu-id="54a13-128">String</span><span class="sxs-lookup"><span data-stu-id="54a13-128">String</span></span> | <span data-ttu-id="54a13-129">对于 [servicePrincipal](servicePrincipal.md)的 **publishedPermissionScopes** 集合中列出的委派权限，声明值 ( **值** ) 。</span><span class="sxs-lookup"><span data-stu-id="54a13-129">The claim value ( **value** ) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="54a13-130">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="54a13-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54a13-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54a13-131">JSON representation</span></span>

<span data-ttu-id="54a13-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54a13-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
}-->

```json
{
  "id": "string (identifier)",
  "classification": "low",
  "permissionId": "string",
  "permissionName": "string"
}
```
