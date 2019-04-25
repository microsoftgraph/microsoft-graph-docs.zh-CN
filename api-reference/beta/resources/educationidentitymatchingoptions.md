---
title: educationIdentityMatchingOptions 资源类型
description: 提供源属性和目标属性之间用于匹配用户帐户的映射。 source 属性应存在于源数据中。 目标属性应为 azure Active Directory (azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543237"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="451da-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="451da-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="451da-106">提供源属性和目标属性之间用于匹配用户帐户的映射。</span><span class="sxs-lookup"><span data-stu-id="451da-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="451da-107">source 属性应存在于源数据中。</span><span class="sxs-lookup"><span data-stu-id="451da-107">The source property should exist in the source data.</span></span> <span data-ttu-id="451da-108">目标属性应为 azure Active Directory (azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="451da-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="451da-109">属性</span><span class="sxs-lookup"><span data-stu-id="451da-109">Properties</span></span>

| <span data-ttu-id="451da-110">属性</span><span class="sxs-lookup"><span data-stu-id="451da-110">Property</span></span> | <span data-ttu-id="451da-111">类型</span><span class="sxs-lookup"><span data-stu-id="451da-111">Type</span></span> | <span data-ttu-id="451da-112">说明</span><span class="sxs-lookup"><span data-stu-id="451da-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="451da-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="451da-113">**appliesTo**</span></span> | <span data-ttu-id="451da-114">string</span><span class="sxs-lookup"><span data-stu-id="451da-114">string</span></span> |  <span data-ttu-id="451da-115">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="451da-115">The user role type to assign to the license.</span></span> <span data-ttu-id="451da-116">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="451da-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="451da-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="451da-117">**sourcePropertyName**</span></span> | <span data-ttu-id="451da-118">string</span><span class="sxs-lookup"><span data-stu-id="451da-118">string</span></span> |  <span data-ttu-id="451da-119">source 属性的名称, 该名称应为源数据中的字段名称。</span><span class="sxs-lookup"><span data-stu-id="451da-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="451da-120">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="451da-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="451da-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="451da-121">**targetPropertyName**</span></span> | <span data-ttu-id="451da-122">string</span><span class="sxs-lookup"><span data-stu-id="451da-122">string</span></span> |  <span data-ttu-id="451da-123">目标属性的名称, 该名称应为 Azure AD 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="451da-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="451da-124">此属性区分大小写。</span><span class="sxs-lookup"><span data-stu-id="451da-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="451da-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="451da-125">**targetDomain**</span></span> | <span data-ttu-id="451da-126">string</span><span class="sxs-lookup"><span data-stu-id="451da-126">string</span></span> |  <span data-ttu-id="451da-127">要与要在目标中匹配的 source 属性后缀的域。</span><span class="sxs-lookup"><span data-stu-id="451da-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="451da-128">如果提供为 null, 则 source 属性将用于与目标属性匹配。</span><span class="sxs-lookup"><span data-stu-id="451da-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="451da-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="451da-129">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
