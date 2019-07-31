---
title: educationIdentityMatchingOptions 资源类型
description: 提供源属性和目标属性之间用于匹配用户帐户的映射。 Source 属性应存在于源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88a22ff446aaa4fd1e7093ec507372c03afcc42b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972689"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="ef72f-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef72f-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef72f-106">提供源属性和目标属性之间用于匹配用户帐户的映射。</span><span class="sxs-lookup"><span data-stu-id="ef72f-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="ef72f-107">Source 属性应存在于源数据中。</span><span class="sxs-lookup"><span data-stu-id="ef72f-107">The source property should exist in the source data.</span></span> <span data-ttu-id="ef72f-108">目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="ef72f-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="ef72f-109">属性</span><span class="sxs-lookup"><span data-stu-id="ef72f-109">Properties</span></span>

| <span data-ttu-id="ef72f-110">属性</span><span class="sxs-lookup"><span data-stu-id="ef72f-110">Property</span></span> | <span data-ttu-id="ef72f-111">类型</span><span class="sxs-lookup"><span data-stu-id="ef72f-111">Type</span></span> | <span data-ttu-id="ef72f-112">说明</span><span class="sxs-lookup"><span data-stu-id="ef72f-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ef72f-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="ef72f-113">**appliesTo**</span></span> | <span data-ttu-id="ef72f-114">string</span><span class="sxs-lookup"><span data-stu-id="ef72f-114">string</span></span> |  <span data-ttu-id="ef72f-115">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="ef72f-115">The user role type to assign to the license.</span></span> <span data-ttu-id="ef72f-116">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="ef72f-116">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="ef72f-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="ef72f-117">**sourcePropertyName**</span></span> | <span data-ttu-id="ef72f-118">string</span><span class="sxs-lookup"><span data-stu-id="ef72f-118">string</span></span> |  <span data-ttu-id="ef72f-119">Source 属性的名称, 该名称应为源数据中的字段名称。</span><span class="sxs-lookup"><span data-stu-id="ef72f-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="ef72f-120">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ef72f-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="ef72f-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="ef72f-121">**targetPropertyName**</span></span> | <span data-ttu-id="ef72f-122">string</span><span class="sxs-lookup"><span data-stu-id="ef72f-122">string</span></span> |  <span data-ttu-id="ef72f-123">目标属性的名称, 该名称应为 Azure AD 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="ef72f-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="ef72f-124">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ef72f-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="ef72f-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="ef72f-125">**targetDomain**</span></span> | <span data-ttu-id="ef72f-126">string</span><span class="sxs-lookup"><span data-stu-id="ef72f-126">string</span></span> |  <span data-ttu-id="ef72f-127">要与要在目标中匹配的 source 属性后缀的域。</span><span class="sxs-lookup"><span data-stu-id="ef72f-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="ef72f-128">如果提供为 null, 则 source 属性将用于与目标属性匹配。</span><span class="sxs-lookup"><span data-stu-id="ef72f-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="ef72f-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef72f-129">JSON representation</span></span>
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
