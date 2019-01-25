---
title: educationIdentityMatchingOptions 资源类型
description: 提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513702"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="9cb26-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cb26-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb26-106">提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。</span><span class="sxs-lookup"><span data-stu-id="9cb26-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="9cb26-107">Source 属性应存在的源数据中。</span><span class="sxs-lookup"><span data-stu-id="9cb26-107">The source property should exist in the source data.</span></span> <span data-ttu-id="9cb26-108">目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="9cb26-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="9cb26-109">属性</span><span class="sxs-lookup"><span data-stu-id="9cb26-109">Properties</span></span>

| <span data-ttu-id="9cb26-110">属性</span><span class="sxs-lookup"><span data-stu-id="9cb26-110">Property</span></span> | <span data-ttu-id="9cb26-111">类型</span><span class="sxs-lookup"><span data-stu-id="9cb26-111">Type</span></span> | <span data-ttu-id="9cb26-112">说明</span><span class="sxs-lookup"><span data-stu-id="9cb26-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9cb26-113">appliesTo</span><span class="sxs-lookup"><span data-stu-id="9cb26-113">**appliesTo**</span></span> | <span data-ttu-id="9cb26-114">string</span><span class="sxs-lookup"><span data-stu-id="9cb26-114">string</span></span> |  <span data-ttu-id="9cb26-115">要分配许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="9cb26-115">The user role type to assign to the license.</span></span> <span data-ttu-id="9cb26-116">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="9cb26-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="9cb26-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="9cb26-117">**sourcePropertyName**</span></span> | <span data-ttu-id="9cb26-118">string</span><span class="sxs-lookup"><span data-stu-id="9cb26-118">string</span></span> |  <span data-ttu-id="9cb26-119">Source 属性，应该是源数据中的字段名称的名称。</span><span class="sxs-lookup"><span data-stu-id="9cb26-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="9cb26-120">此属性是区分大小写。</span><span class="sxs-lookup"><span data-stu-id="9cb26-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="9cb26-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="9cb26-121">**targetPropertyName**</span></span> | <span data-ttu-id="9cb26-122">string</span><span class="sxs-lookup"><span data-stu-id="9cb26-122">string</span></span> |  <span data-ttu-id="9cb26-123">目标属性，应为 Azure AD 中的有效属性名称。</span><span class="sxs-lookup"><span data-stu-id="9cb26-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="9cb26-124">此属性是区分大小写。</span><span class="sxs-lookup"><span data-stu-id="9cb26-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="9cb26-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="9cb26-125">**targetDomain**</span></span> | <span data-ttu-id="9cb26-126">string</span><span class="sxs-lookup"><span data-stu-id="9cb26-126">string</span></span> |  <span data-ttu-id="9cb26-127">使用 source 属性以匹配目标后缀域。</span><span class="sxs-lookup"><span data-stu-id="9cb26-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="9cb26-128">如果提供为 null，source 属性将用于与目标属性相匹配。</span><span class="sxs-lookup"><span data-stu-id="9cb26-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="9cb26-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cb26-129">JSON representation</span></span>
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
