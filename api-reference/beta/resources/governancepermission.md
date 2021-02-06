---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 具有的访问权限。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f316a863ecba9ed546b9ba4045e57ada87e97ab9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128832"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="e8082-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8082-103">governancePermission resource type</span></span>

<span data-ttu-id="e8082-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8082-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8082-105">表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource 具有的访问权限](../resources/governanceresource.md)。</span><span class="sxs-lookup"><span data-stu-id="e8082-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>


## <a name="properties"></a><span data-ttu-id="e8082-106">属性</span><span class="sxs-lookup"><span data-stu-id="e8082-106">Properties</span></span>
| <span data-ttu-id="e8082-107">属性</span><span class="sxs-lookup"><span data-stu-id="e8082-107">Property</span></span>     | <span data-ttu-id="e8082-108">类型</span><span class="sxs-lookup"><span data-stu-id="e8082-108">Type</span></span>   |<span data-ttu-id="e8082-109">说明</span><span class="sxs-lookup"><span data-stu-id="e8082-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8082-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e8082-110">accessLevel</span></span>|<span data-ttu-id="e8082-111">字符串</span><span class="sxs-lookup"><span data-stu-id="e8082-111">String</span></span>|<span data-ttu-id="e8082-112">访问级别。</span><span class="sxs-lookup"><span data-stu-id="e8082-112">The access level.</span></span> <span data-ttu-id="e8082-113">有效值： ``None`` 、 ``UserRead`` 和 ``AdminRead`` ``AdminReadWrite`` 。</span><span class="sxs-lookup"><span data-stu-id="e8082-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="e8082-114">isActive</span><span class="sxs-lookup"><span data-stu-id="e8082-114">isActive</span></span>|<span data-ttu-id="e8082-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8082-115">Boolean</span></span>|<span data-ttu-id="e8082-116">指示请求程序是否具有访问角色分配活动应用程序。</span><span class="sxs-lookup"><span data-stu-id="e8082-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="e8082-117">isEligible</span><span class="sxs-lookup"><span data-stu-id="e8082-117">isEligible</span></span>|<span data-ttu-id="e8082-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8082-118">Boolean</span></span>|<span data-ttu-id="e8082-119">指示请求者是否具有访问角色分配条件。</span><span class="sxs-lookup"><span data-stu-id="e8082-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8082-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8082-120">JSON representation</span></span>

<span data-ttu-id="e8082-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8082-121">Here is a JSON representation of the resource.</span></span>
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


