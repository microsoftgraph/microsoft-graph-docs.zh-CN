---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 的访问权限。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 113f25cd276cf01ce46e3c410ca4b5b409417d98
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809514"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="d61df-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="d61df-103">governancePermission resource type</span></span>

<span data-ttu-id="d61df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d61df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61df-105">表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource](../resources/governanceresource.md)的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d61df-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>


## <a name="properties"></a><span data-ttu-id="d61df-106">属性</span><span class="sxs-lookup"><span data-stu-id="d61df-106">Properties</span></span>
| <span data-ttu-id="d61df-107">属性</span><span class="sxs-lookup"><span data-stu-id="d61df-107">Property</span></span>     | <span data-ttu-id="d61df-108">类型</span><span class="sxs-lookup"><span data-stu-id="d61df-108">Type</span></span>   |<span data-ttu-id="d61df-109">说明</span><span class="sxs-lookup"><span data-stu-id="d61df-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d61df-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="d61df-110">accessLevel</span></span>|<span data-ttu-id="d61df-111">String</span><span class="sxs-lookup"><span data-stu-id="d61df-111">String</span></span>|<span data-ttu-id="d61df-112">访问级别。</span><span class="sxs-lookup"><span data-stu-id="d61df-112">The access level.</span></span> <span data-ttu-id="d61df-113">有效值： ``None`` 、、 ``UserRead`` ``AdminRead`` 和 ``AdminReadWrite`` 。</span><span class="sxs-lookup"><span data-stu-id="d61df-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="d61df-114">isActive</span><span class="sxs-lookup"><span data-stu-id="d61df-114">isActive</span></span>|<span data-ttu-id="d61df-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="d61df-115">Boolean</span></span>|<span data-ttu-id="d61df-116">指示请求者是否具有访问级别的任何活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="d61df-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="d61df-117">isEligible</span><span class="sxs-lookup"><span data-stu-id="d61df-117">isEligible</span></span>|<span data-ttu-id="d61df-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="d61df-118">Boolean</span></span>|<span data-ttu-id="d61df-119">指示请求者是否具有访问级别的任何符合条件的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d61df-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d61df-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d61df-120">JSON representation</span></span>

<span data-ttu-id="d61df-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d61df-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
