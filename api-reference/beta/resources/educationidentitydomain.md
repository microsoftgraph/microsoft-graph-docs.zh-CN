---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b25f935ae404a243826a14c310a17ad80c598380
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095385"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="141f9-104">educationIdentityDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="141f9-104">educationIdentityDomain resource type</span></span>

<span data-ttu-id="141f9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="141f9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="141f9-106">表示教育用户类型与用户帐户所属域之间的映射。</span><span class="sxs-lookup"><span data-stu-id="141f9-106">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="141f9-107">域资源是 [标识创建配置](educationidentitycreationconfiguration.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="141f9-107">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="141f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="141f9-108">Properties</span></span>

| <span data-ttu-id="141f9-109">属性</span><span class="sxs-lookup"><span data-stu-id="141f9-109">Property</span></span>  | <span data-ttu-id="141f9-110">类型</span><span class="sxs-lookup"><span data-stu-id="141f9-110">Type</span></span>   | <span data-ttu-id="141f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="141f9-111">Description</span></span>                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="141f9-112">appliesTo</span><span class="sxs-lookup"><span data-stu-id="141f9-112">appliesTo</span></span> | <span data-ttu-id="141f9-113">String</span><span class="sxs-lookup"><span data-stu-id="141f9-113">String</span></span> | <span data-ttu-id="141f9-114">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="141f9-114">The user role type to assign to the license.</span></span> <span data-ttu-id="141f9-115">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="141f9-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="141f9-116">名称</span><span class="sxs-lookup"><span data-stu-id="141f9-116">name</span></span>      | <span data-ttu-id="141f9-117">字符串</span><span class="sxs-lookup"><span data-stu-id="141f9-117">String</span></span> | <span data-ttu-id="141f9-118">代表用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="141f9-118">Represents the domain for the user account.</span></span>                                                        |

## <a name="json-representation"></a><span data-ttu-id="141f9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="141f9-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "name": "String"
}
```


