---
title: educationIdentityMatchingOptions 资源类型
description: 提供源属性和目标属性之间用于匹配用户帐户的映射。 Source 属性应存在于源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 37ebb55fdd5457841ca0083c18518babca7565c4
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750148"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="4bc58-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bc58-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bc58-106">提供源属性和目标属性之间用于匹配用户帐户的映射。</span><span class="sxs-lookup"><span data-stu-id="4bc58-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="4bc58-107">Source 属性应存在于源数据中。</span><span class="sxs-lookup"><span data-stu-id="4bc58-107">The source property should exist in the source data.</span></span> <span data-ttu-id="4bc58-108">目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="4bc58-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="4bc58-109">属性</span><span class="sxs-lookup"><span data-stu-id="4bc58-109">Properties</span></span>

| <span data-ttu-id="4bc58-110">属性</span><span class="sxs-lookup"><span data-stu-id="4bc58-110">Property</span></span> | <span data-ttu-id="4bc58-111">类型</span><span class="sxs-lookup"><span data-stu-id="4bc58-111">Type</span></span> | <span data-ttu-id="4bc58-112">说明</span><span class="sxs-lookup"><span data-stu-id="4bc58-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4bc58-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="4bc58-113">**appliesTo**</span></span> | <span data-ttu-id="4bc58-114">string</span><span class="sxs-lookup"><span data-stu-id="4bc58-114">string</span></span> |  <span data-ttu-id="4bc58-115">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="4bc58-115">The user role type to assign to the license.</span></span> <span data-ttu-id="4bc58-116">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="4bc58-116">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="4bc58-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="4bc58-117">**sourcePropertyName**</span></span> | <span data-ttu-id="4bc58-118">string</span><span class="sxs-lookup"><span data-stu-id="4bc58-118">string</span></span> |  <span data-ttu-id="4bc58-119">Source 属性的名称, 该名称应为源数据中的字段名称。</span><span class="sxs-lookup"><span data-stu-id="4bc58-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="4bc58-120">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4bc58-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="4bc58-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="4bc58-121">**targetPropertyName**</span></span> | <span data-ttu-id="4bc58-122">string</span><span class="sxs-lookup"><span data-stu-id="4bc58-122">string</span></span> |  <span data-ttu-id="4bc58-123">目标属性的名称, 该名称应为 Azure AD 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="4bc58-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="4bc58-124">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4bc58-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="4bc58-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="4bc58-125">**targetDomain**</span></span> | <span data-ttu-id="4bc58-126">string</span><span class="sxs-lookup"><span data-stu-id="4bc58-126">string</span></span> |  <span data-ttu-id="4bc58-127">要与要在目标中匹配的 source 属性后缀的域。</span><span class="sxs-lookup"><span data-stu-id="4bc58-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="4bc58-128">如果提供为 null, 则 source 属性将用于与目标属性匹配。</span><span class="sxs-lookup"><span data-stu-id="4bc58-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="4bc58-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bc58-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
