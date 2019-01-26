---
title: governancePermission 资源类型
description: '表示对特定 governanceResource governanceSubject 具有访问权限。  '
localization_priority: Normal
ms.openlocfilehash: 9b6e920d92d7010fb325be05cf0b645f9b8d81cd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570720"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="a5c71-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5c71-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5c71-104">表示对特定[governanceResource](../resources/governanceresource.md) [governanceSubject](../resources/governancesubject.md)具有访问权限。</span><span class="sxs-lookup"><span data-stu-id="a5c71-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="a5c71-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5c71-105">Properties</span></span>
| <span data-ttu-id="a5c71-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5c71-106">Property</span></span>     | <span data-ttu-id="a5c71-107">类型</span><span class="sxs-lookup"><span data-stu-id="a5c71-107">Type</span></span>   |<span data-ttu-id="a5c71-108">说明</span><span class="sxs-lookup"><span data-stu-id="a5c71-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5c71-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="a5c71-109">accessLevel</span></span>|<span data-ttu-id="a5c71-110">String</span><span class="sxs-lookup"><span data-stu-id="a5c71-110">String</span></span>|<span data-ttu-id="a5c71-111">访问级别。</span><span class="sxs-lookup"><span data-stu-id="a5c71-111">The access level.</span></span> <span data-ttu-id="a5c71-112">有效值： ``None``， ``UserRead``， ``AdminRead``，和``AdminReadWrite``。</span><span class="sxs-lookup"><span data-stu-id="a5c71-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="a5c71-113">isActive</span><span class="sxs-lookup"><span data-stu-id="a5c71-113">isActive</span></span>|<span data-ttu-id="a5c71-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="a5c71-114">Boolean</span></span>|<span data-ttu-id="a5c71-115">指示如果请求者有任何主动角色分配访问级别。</span><span class="sxs-lookup"><span data-stu-id="a5c71-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="a5c71-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="a5c71-116">isEligible</span></span>|<span data-ttu-id="a5c71-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="a5c71-117">Boolean</span></span>|<span data-ttu-id="a5c71-118">指示请求者是否具有任何访问级别的合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="a5c71-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5c71-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5c71-119">JSON representation</span></span>

<span data-ttu-id="a5c71-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5c71-120">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
