---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 的访问权限。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8bf32b855ed77ccdf712b1a739ef913d0a3dade0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971940"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="4089f-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="4089f-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4089f-104">表示[governanceSubject](../resources/governancesubject.md)对特定[governanceResource](../resources/governanceresource.md)的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4089f-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="4089f-105">属性</span><span class="sxs-lookup"><span data-stu-id="4089f-105">Properties</span></span>
| <span data-ttu-id="4089f-106">属性</span><span class="sxs-lookup"><span data-stu-id="4089f-106">Property</span></span>     | <span data-ttu-id="4089f-107">类型</span><span class="sxs-lookup"><span data-stu-id="4089f-107">Type</span></span>   |<span data-ttu-id="4089f-108">说明</span><span class="sxs-lookup"><span data-stu-id="4089f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4089f-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="4089f-109">accessLevel</span></span>|<span data-ttu-id="4089f-110">String</span><span class="sxs-lookup"><span data-stu-id="4089f-110">String</span></span>|<span data-ttu-id="4089f-111">访问级别。</span><span class="sxs-lookup"><span data-stu-id="4089f-111">The access level.</span></span> <span data-ttu-id="4089f-112">有效值: ``None``、 ``UserRead`` ``AdminRead``、和。 ``AdminReadWrite``</span><span class="sxs-lookup"><span data-stu-id="4089f-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="4089f-113">isActive</span><span class="sxs-lookup"><span data-stu-id="4089f-113">isActive</span></span>|<span data-ttu-id="4089f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4089f-114">Boolean</span></span>|<span data-ttu-id="4089f-115">指示请求者是否具有访问级别的任何活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="4089f-115">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="4089f-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="4089f-116">isEligible</span></span>|<span data-ttu-id="4089f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4089f-117">Boolean</span></span>|<span data-ttu-id="4089f-118">指示请求者是否具有访问级别的任何符合条件的角色分配。</span><span class="sxs-lookup"><span data-stu-id="4089f-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4089f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4089f-119">JSON representation</span></span>

<span data-ttu-id="4089f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4089f-120">Here is a JSON representation of the resource.</span></span>
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
