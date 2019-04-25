---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 的访问权限。  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547506"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="51f99-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="51f99-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f99-104">表示[governanceSubject](../resources/governancesubject.md)对特定[governanceResource](../resources/governanceresource.md)的访问权限。</span><span class="sxs-lookup"><span data-stu-id="51f99-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="51f99-105">属性</span><span class="sxs-lookup"><span data-stu-id="51f99-105">Properties</span></span>
| <span data-ttu-id="51f99-106">属性</span><span class="sxs-lookup"><span data-stu-id="51f99-106">Property</span></span>     | <span data-ttu-id="51f99-107">类型</span><span class="sxs-lookup"><span data-stu-id="51f99-107">Type</span></span>   |<span data-ttu-id="51f99-108">说明</span><span class="sxs-lookup"><span data-stu-id="51f99-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51f99-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="51f99-109">accessLevel</span></span>|<span data-ttu-id="51f99-110">String</span><span class="sxs-lookup"><span data-stu-id="51f99-110">String</span></span>|<span data-ttu-id="51f99-111">访问级别。</span><span class="sxs-lookup"><span data-stu-id="51f99-111">The access level.</span></span> <span data-ttu-id="51f99-112">有效值: ``None``、 ``UserRead`` ``AdminRead``、和。 ``AdminReadWrite``</span><span class="sxs-lookup"><span data-stu-id="51f99-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="51f99-113">isActive</span><span class="sxs-lookup"><span data-stu-id="51f99-113">isActive</span></span>|<span data-ttu-id="51f99-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="51f99-114">Boolean</span></span>|<span data-ttu-id="51f99-115">指示请求者是否具有访问级别的任何活动角色分配。</span><span class="sxs-lookup"><span data-stu-id="51f99-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="51f99-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="51f99-116">isEligible</span></span>|<span data-ttu-id="51f99-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="51f99-117">Boolean</span></span>|<span data-ttu-id="51f99-118">指示请求者是否具有访问级别的任何符合条件的角色分配。</span><span class="sxs-lookup"><span data-stu-id="51f99-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51f99-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51f99-119">JSON representation</span></span>

<span data-ttu-id="51f99-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51f99-120">Here is a JSON representation of the resource.</span></span>

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
