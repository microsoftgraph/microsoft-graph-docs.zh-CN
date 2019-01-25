---
title: governancePermission 资源类型
description: '表示对特定 governanceResource governanceSubject 具有访问权限。  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529836"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="f6fa4-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6fa4-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6fa4-104">表示对特定[governanceResource](../resources/governanceresource.md) [governanceSubject](../resources/governancesubject.md)具有访问权限。</span><span class="sxs-lookup"><span data-stu-id="f6fa4-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="f6fa4-105">属性</span><span class="sxs-lookup"><span data-stu-id="f6fa4-105">Properties</span></span>
| <span data-ttu-id="f6fa4-106">属性</span><span class="sxs-lookup"><span data-stu-id="f6fa4-106">Property</span></span>     | <span data-ttu-id="f6fa4-107">类型</span><span class="sxs-lookup"><span data-stu-id="f6fa4-107">Type</span></span>   |<span data-ttu-id="f6fa4-108">说明</span><span class="sxs-lookup"><span data-stu-id="f6fa4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6fa4-109">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="f6fa4-109">accessLevel</span></span>|<span data-ttu-id="f6fa4-110">String</span><span class="sxs-lookup"><span data-stu-id="f6fa4-110">String</span></span>|<span data-ttu-id="f6fa4-111">访问级别。</span><span class="sxs-lookup"><span data-stu-id="f6fa4-111">The access level.</span></span> <span data-ttu-id="f6fa4-112">有效值： ``None``， ``UserRead``， ``AdminRead``，和``AdminReadWrite``。</span><span class="sxs-lookup"><span data-stu-id="f6fa4-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="f6fa4-113">isActive</span><span class="sxs-lookup"><span data-stu-id="f6fa4-113">isActive</span></span>|<span data-ttu-id="f6fa4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6fa4-114">Boolean</span></span>|<span data-ttu-id="f6fa4-115">指示如果请求者有任何主动角色分配访问级别。</span><span class="sxs-lookup"><span data-stu-id="f6fa4-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="f6fa4-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="f6fa4-116">isEligible</span></span>|<span data-ttu-id="f6fa4-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6fa4-117">Boolean</span></span>|<span data-ttu-id="f6fa4-118">指示请求者是否具有任何访问级别的合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="f6fa4-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6fa4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6fa4-119">JSON representation</span></span>

<span data-ttu-id="f6fa4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6fa4-120">Here is a JSON representation of the resource.</span></span>

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
