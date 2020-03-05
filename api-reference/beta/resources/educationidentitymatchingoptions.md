---
title: educationIdentityMatchingOptions 资源类型
description: 提供源属性和目标属性之间用于匹配用户帐户的映射。 Source 属性应存在于源数据中。 目标属性应为 Azure Active Directory （Azure AD）中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d722beaac54cbd57c227457a0883b856f6eca4bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501827"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="db001-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="db001-105">educationIdentityMatchingOptions resource type</span></span>

<span data-ttu-id="db001-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="db001-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db001-107">提供源属性和目标属性之间用于匹配用户帐户的映射。</span><span class="sxs-lookup"><span data-stu-id="db001-107">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="db001-108">Source 属性应存在于源数据中。</span><span class="sxs-lookup"><span data-stu-id="db001-108">The source property should exist in the source data.</span></span> <span data-ttu-id="db001-109">目标属性应为 Azure Active Directory （Azure AD）中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="db001-109">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="db001-110">属性</span><span class="sxs-lookup"><span data-stu-id="db001-110">Properties</span></span>

| <span data-ttu-id="db001-111">属性</span><span class="sxs-lookup"><span data-stu-id="db001-111">Property</span></span> | <span data-ttu-id="db001-112">类型</span><span class="sxs-lookup"><span data-stu-id="db001-112">Type</span></span> | <span data-ttu-id="db001-113">说明</span><span class="sxs-lookup"><span data-stu-id="db001-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="db001-114">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="db001-114">**appliesTo**</span></span> | <span data-ttu-id="db001-115">string</span><span class="sxs-lookup"><span data-stu-id="db001-115">string</span></span> |  <span data-ttu-id="db001-116">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="db001-116">The user role type to assign to the license.</span></span> <span data-ttu-id="db001-117">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="db001-117">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="db001-118">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="db001-118">**sourcePropertyName**</span></span> | <span data-ttu-id="db001-119">string</span><span class="sxs-lookup"><span data-stu-id="db001-119">string</span></span> |  <span data-ttu-id="db001-120">Source 属性的名称，该名称应为源数据中的字段名称。</span><span class="sxs-lookup"><span data-stu-id="db001-120">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="db001-121">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="db001-121">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="db001-122">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="db001-122">**targetPropertyName**</span></span> | <span data-ttu-id="db001-123">string</span><span class="sxs-lookup"><span data-stu-id="db001-123">string</span></span> |  <span data-ttu-id="db001-124">目标属性的名称，该名称应为 Azure AD 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="db001-124">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="db001-125">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="db001-125">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="db001-126">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="db001-126">**targetDomain**</span></span> | <span data-ttu-id="db001-127">string</span><span class="sxs-lookup"><span data-stu-id="db001-127">string</span></span> |  <span data-ttu-id="db001-128">要与要在目标中匹配的 source 属性后缀的域。</span><span class="sxs-lookup"><span data-stu-id="db001-128">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="db001-129">如果提供为 null，则 source 属性将用于与目标属性匹配。</span><span class="sxs-lookup"><span data-stu-id="db001-129">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="db001-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db001-130">JSON representation</span></span>
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
