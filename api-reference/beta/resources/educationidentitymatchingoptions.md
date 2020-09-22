---
title: educationIdentityMatchingOptions 资源类型
description: 提供源属性和目标属性之间用于匹配用户帐户的映射。 Source 属性应存在于源数据中。 Target 属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 73c97b0e9c23c455b3e15ed656060eca7f8a3e4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095371"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="435ae-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="435ae-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="435ae-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="435ae-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="435ae-107">提供源属性和目标属性之间用于匹配用户帐户的映射。</span><span class="sxs-lookup"><span data-stu-id="435ae-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="435ae-108">Source 属性应存在于源数据中。</span><span class="sxs-lookup"><span data-stu-id="435ae-108">The source property should exist in the source data.</span></span> <span data-ttu-id="435ae-109">Target 属性应为 Azure Active Directory (Azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="435ae-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="435ae-110">属性</span><span class="sxs-lookup"><span data-stu-id="435ae-110">Properties</span></span>

| <span data-ttu-id="435ae-111">属性</span><span class="sxs-lookup"><span data-stu-id="435ae-111">Property</span></span>           | <span data-ttu-id="435ae-112">类型</span><span class="sxs-lookup"><span data-stu-id="435ae-112">Type</span></span>   | <span data-ttu-id="435ae-113">说明</span><span class="sxs-lookup"><span data-stu-id="435ae-113">Description</span></span>                                                                                                                                                    |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="435ae-114">appliesTo</span><span class="sxs-lookup"><span data-stu-id="435ae-114">appliesTo</span></span>          | <span data-ttu-id="435ae-115">String</span><span class="sxs-lookup"><span data-stu-id="435ae-115">String</span></span> | <span data-ttu-id="435ae-116">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="435ae-116">The user role type to assign to the license.</span></span> <span data-ttu-id="435ae-117">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="435ae-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>                                                             |
| <span data-ttu-id="435ae-118">sourcePropertyName</span><span class="sxs-lookup"><span data-stu-id="435ae-118">sourcePropertyName</span></span> | <span data-ttu-id="435ae-119">字符串</span><span class="sxs-lookup"><span data-stu-id="435ae-119">String</span></span> | <span data-ttu-id="435ae-120">Source 属性的名称，该名称应为源数据中的字段名称。</span><span class="sxs-lookup"><span data-stu-id="435ae-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="435ae-121">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="435ae-121">This property is case-sensitive.</span></span>                                             |
| <span data-ttu-id="435ae-122">targetPropertyName</span><span class="sxs-lookup"><span data-stu-id="435ae-122">targetPropertyName</span></span> | <span data-ttu-id="435ae-123">字符串</span><span class="sxs-lookup"><span data-stu-id="435ae-123">String</span></span> | <span data-ttu-id="435ae-124">目标属性的名称，该名称应为 Azure AD 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="435ae-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="435ae-125">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="435ae-125">This property is case-sensitive.</span></span>                                                |
| <span data-ttu-id="435ae-126">targetDomain</span><span class="sxs-lookup"><span data-stu-id="435ae-126">targetDomain</span></span>       | <span data-ttu-id="435ae-127">字符串</span><span class="sxs-lookup"><span data-stu-id="435ae-127">String</span></span> | <span data-ttu-id="435ae-128">要与要在目标中匹配的 source 属性后缀的域。</span><span class="sxs-lookup"><span data-stu-id="435ae-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="435ae-129">如果提供为 null，则 source 属性将用于与目标属性匹配。</span><span class="sxs-lookup"><span data-stu-id="435ae-129">If provided as null, the source property will be used to match with the target property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="435ae-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="435ae-130">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "sourcePropertyName": "String",
  "targetPropertyName": "String",
  "targetDomain": "String"
}
```


