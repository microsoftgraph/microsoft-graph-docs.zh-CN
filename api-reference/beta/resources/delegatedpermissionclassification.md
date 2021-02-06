---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4a567696d2adf0cd2a53cc2eb4d193ec1e1c2855
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133635"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="88f3e-103">delegatedPermissionClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="88f3e-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="88f3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88f3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88f3e-105">用于指定委派权限的分类。</span><span class="sxs-lookup"><span data-stu-id="88f3e-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="88f3e-106">委派权限分类可以与用户同意设置结合使用，以选择允许用户同意的权限。</span><span class="sxs-lookup"><span data-stu-id="88f3e-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="88f3e-107">请参阅 ["配置最终用户如何同意应用程序以](/azure/active-directory/manage-apps/configure-user-consent) 了解有关权限分类更多信息"。</span><span class="sxs-lookup"><span data-stu-id="88f3e-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="88f3e-108">属性</span><span class="sxs-lookup"><span data-stu-id="88f3e-108">Properties</span></span>

| <span data-ttu-id="88f3e-109">属性</span><span class="sxs-lookup"><span data-stu-id="88f3e-109">Property</span></span> | <span data-ttu-id="88f3e-110">类型</span><span class="sxs-lookup"><span data-stu-id="88f3e-110">Type</span></span> | <span data-ttu-id="88f3e-111">说明</span><span class="sxs-lookup"><span data-stu-id="88f3e-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="88f3e-112">id</span><span class="sxs-lookup"><span data-stu-id="88f3e-112">id</span></span> | <span data-ttu-id="88f3e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="88f3e-113">String</span></span> | <span data-ttu-id="88f3e-114">**delegatedPermissionClassification 项的唯一** 标识符。</span><span class="sxs-lookup"><span data-stu-id="88f3e-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="88f3e-115">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="88f3e-115">Not nullable.</span></span> <span data-ttu-id="88f3e-116">只读。</span><span class="sxs-lookup"><span data-stu-id="88f3e-116">Read-only.</span></span> |
| <span data-ttu-id="88f3e-117">classification</span><span class="sxs-lookup"><span data-stu-id="88f3e-117">classification</span></span> | <span data-ttu-id="88f3e-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="88f3e-118">permissionClassificationType</span></span> | <span data-ttu-id="88f3e-119">给定的分类值。</span><span class="sxs-lookup"><span data-stu-id="88f3e-119">The classification value being given.</span></span> <span data-ttu-id="88f3e-120">可能的值： `low` .</span><span class="sxs-lookup"><span data-stu-id="88f3e-120">Possible value: `low`.</span></span> <span data-ttu-id="88f3e-121">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="88f3e-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="88f3e-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="88f3e-122">permissionId</span></span> | <span data-ttu-id="88f3e-123">Guid</span><span class="sxs-lookup"><span data-stu-id="88f3e-123">Guid</span></span> | <span data-ttu-id="88f3e-124">[servicePrincipal](servicePrincipal.md) **() 的 publishedPermissionScopes** 集合中列出的委派权限的唯一标识符 id。 </span><span class="sxs-lookup"><span data-stu-id="88f3e-124">The unique identifier (**id**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="88f3e-125">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="88f3e-125">Required on create.</span></span> <span data-ttu-id="88f3e-126">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="88f3e-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="88f3e-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="88f3e-127">permissionName</span></span> | <span data-ttu-id="88f3e-128">字符串</span><span class="sxs-lookup"><span data-stu-id="88f3e-128">String</span></span> | <span data-ttu-id="88f3e-129">the claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="88f3e-129">The claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="88f3e-130">不支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="88f3e-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88f3e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88f3e-131">JSON representation</span></span>

<span data-ttu-id="88f3e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88f3e-132">The following is a JSON representation of the resource.</span></span>

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

