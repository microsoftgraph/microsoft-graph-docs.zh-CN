---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时, 资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507094"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="60349-104">educationSynchronizationLicenseAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="60349-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60349-105">表示要分配给用户帐户的许可证信息。</span><span class="sxs-lookup"><span data-stu-id="60349-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="60349-106">创建新用户帐户时, 资源将用于设置许可证分配。</span><span class="sxs-lookup"><span data-stu-id="60349-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="60349-107">属性</span><span class="sxs-lookup"><span data-stu-id="60349-107">Properties</span></span>

| <span data-ttu-id="60349-108">属性</span><span class="sxs-lookup"><span data-stu-id="60349-108">Property</span></span> | <span data-ttu-id="60349-109">类型</span><span class="sxs-lookup"><span data-stu-id="60349-109">Type</span></span> | <span data-ttu-id="60349-110">说明</span><span class="sxs-lookup"><span data-stu-id="60349-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="60349-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="60349-111">**appliesTo**</span></span> | <span data-ttu-id="60349-112">字符串</span><span class="sxs-lookup"><span data-stu-id="60349-112">string</span></span> | <span data-ttu-id="60349-113">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="60349-113">The user role type to assign to license.</span></span> <span data-ttu-id="60349-114">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="60349-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="60349-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="60349-115">**skuIds**</span></span> | <span data-ttu-id="60349-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="60349-116">collection of strings</span></span> |  <span data-ttu-id="60349-117">表示要分配的许可证的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="60349-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="60349-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60349-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
