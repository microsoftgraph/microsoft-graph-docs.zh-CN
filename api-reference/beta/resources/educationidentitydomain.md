---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 628fbdea770c685eca0194fb95a314e2e542d2fc
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750155"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="546e9-104">educationIdentityDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="546e9-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="546e9-105">表示教育用户类型与用户帐户所属域之间的映射。</span><span class="sxs-lookup"><span data-stu-id="546e9-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="546e9-106">域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="546e9-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="546e9-107">属性</span><span class="sxs-lookup"><span data-stu-id="546e9-107">Properties</span></span>

| <span data-ttu-id="546e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="546e9-108">Property</span></span> | <span data-ttu-id="546e9-109">类型</span><span class="sxs-lookup"><span data-stu-id="546e9-109">Type</span></span> | <span data-ttu-id="546e9-110">说明</span><span class="sxs-lookup"><span data-stu-id="546e9-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="546e9-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="546e9-111">**appliesTo**</span></span> | <span data-ttu-id="546e9-112">string</span><span class="sxs-lookup"><span data-stu-id="546e9-112">string</span></span> |  <span data-ttu-id="546e9-113">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="546e9-113">The user role type to assign to the license.</span></span> <span data-ttu-id="546e9-114">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="546e9-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="546e9-115">**name**</span><span class="sxs-lookup"><span data-stu-id="546e9-115">**name**</span></span> | <span data-ttu-id="546e9-116">string</span><span class="sxs-lookup"><span data-stu-id="546e9-116">string</span></span> |  <span data-ttu-id="546e9-117">代表用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="546e9-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="546e9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="546e9-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
