---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时, 资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b00550c1a4d2d02efc983ab345fbc429b443a5bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972395"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="fb53f-104">educationSynchronizationLicenseAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb53f-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb53f-105">表示要分配给用户帐户的许可证信息。</span><span class="sxs-lookup"><span data-stu-id="fb53f-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="fb53f-106">创建新用户帐户时, 资源将用于设置许可证分配。</span><span class="sxs-lookup"><span data-stu-id="fb53f-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="fb53f-107">属性</span><span class="sxs-lookup"><span data-stu-id="fb53f-107">Properties</span></span>

| <span data-ttu-id="fb53f-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb53f-108">Property</span></span> | <span data-ttu-id="fb53f-109">类型</span><span class="sxs-lookup"><span data-stu-id="fb53f-109">Type</span></span> | <span data-ttu-id="fb53f-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb53f-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fb53f-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="fb53f-111">**appliesTo**</span></span> | <span data-ttu-id="fb53f-112">string</span><span class="sxs-lookup"><span data-stu-id="fb53f-112">string</span></span> | <span data-ttu-id="fb53f-113">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="fb53f-113">The user role type to assign to license.</span></span> <span data-ttu-id="fb53f-114">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="fb53f-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="fb53f-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="fb53f-115">**skuIds**</span></span> | <span data-ttu-id="fb53f-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="fb53f-116">collection of strings</span></span> |  <span data-ttu-id="fb53f-117">表示要分配的许可证的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="fb53f-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="fb53f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb53f-118">JSON representation</span></span>
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
