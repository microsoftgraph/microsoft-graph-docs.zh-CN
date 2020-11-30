---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7d5926bff0d7096080aa22fae49d0ed15c7d1fcd
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377238"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="bdf9d-103">delegatedPermissionClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdf9d-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="bdf9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf9d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bdf9d-105">用于指定委派权限的分类。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="bdf9d-106">委派权限分类可与用户同意设置结合使用，以选择允许用户同意的权限。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="bdf9d-107">请参阅 [配置最终用户同意应用程序的方式](/azure/active-directory/manage-apps/configure-user-consent) ，以了解有关权限分类的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="bdf9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdf9d-108">Properties</span></span>

| <span data-ttu-id="bdf9d-109">属性</span><span class="sxs-lookup"><span data-stu-id="bdf9d-109">Property</span></span> | <span data-ttu-id="bdf9d-110">类型</span><span class="sxs-lookup"><span data-stu-id="bdf9d-110">Type</span></span> | <span data-ttu-id="bdf9d-111">说明</span><span class="sxs-lookup"><span data-stu-id="bdf9d-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="bdf9d-112">id</span><span class="sxs-lookup"><span data-stu-id="bdf9d-112">id</span></span> | <span data-ttu-id="bdf9d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="bdf9d-113">String</span></span> | <span data-ttu-id="bdf9d-114">**DelegatedPermissionClassification** 项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="bdf9d-115">不可为空。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-115">Not nullable.</span></span> <span data-ttu-id="bdf9d-116">只读。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-116">Read-only.</span></span> |
| <span data-ttu-id="bdf9d-117">classification</span><span class="sxs-lookup"><span data-stu-id="bdf9d-117">classification</span></span> | <span data-ttu-id="bdf9d-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="bdf9d-118">permissionClassificationType</span></span> | <span data-ttu-id="bdf9d-119">所提供的分类值。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-119">The classification value being given.</span></span> <span data-ttu-id="bdf9d-120">可能的值： `low` 。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-120">Possible value: `low`.</span></span> <span data-ttu-id="bdf9d-121">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="bdf9d-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="bdf9d-122">permissionId</span></span> | <span data-ttu-id="bdf9d-123">Guid</span><span class="sxs-lookup"><span data-stu-id="bdf9d-123">Guid</span></span> | <span data-ttu-id="bdf9d-124">[ServicePrincipal](servicePrincipal.md)的 **oauth2PermissionScopes** 集合中列出的委派权限 (**id**) 唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-124">The unique identifier (**id**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="bdf9d-125">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-125">Required on create.</span></span> <span data-ttu-id="bdf9d-126">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="bdf9d-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="bdf9d-127">permissionName</span></span> | <span data-ttu-id="bdf9d-128">字符串</span><span class="sxs-lookup"><span data-stu-id="bdf9d-128">String</span></span> | <span data-ttu-id="bdf9d-129">对于 [servicePrincipal](servicePrincipal.md)的 **oauth2PermissionScopes** 集合中列出的委派权限，声明值 (**值**) 。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-129">The claim value (**value**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="bdf9d-130">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdf9d-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdf9d-131">JSON representation</span></span>

<span data-ttu-id="bdf9d-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdf9d-132">The following is a JSON representation of the resource.</span></span>

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
