---
title: educationIdentityMatchingOptions 资源类型
description: 提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 624e2717387c5cc8994596fd83d5a6856ac6082b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978254"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="a1b3b-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1b3b-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="a1b3b-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1b3b-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1b3b-108">提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="a1b3b-109">Source 属性应存在的源数据中。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-109">The source property should exist in the source data.</span></span> <span data-ttu-id="a1b3b-110">目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="a1b3b-111">属性</span><span class="sxs-lookup"><span data-stu-id="a1b3b-111">Properties</span></span>

| <span data-ttu-id="a1b3b-112">属性</span><span class="sxs-lookup"><span data-stu-id="a1b3b-112">Property</span></span> | <span data-ttu-id="a1b3b-113">类型</span><span class="sxs-lookup"><span data-stu-id="a1b3b-113">Type</span></span> | <span data-ttu-id="a1b3b-114">说明</span><span class="sxs-lookup"><span data-stu-id="a1b3b-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a1b3b-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="a1b3b-115">**appliesTo**</span></span> | <span data-ttu-id="a1b3b-116">string</span><span class="sxs-lookup"><span data-stu-id="a1b3b-116">string</span></span> |  <span data-ttu-id="a1b3b-117">要分配许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-117">The user role type to assign to the license.</span></span> <span data-ttu-id="a1b3b-118">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="a1b3b-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="a1b3b-119">**sourcePropertyName**</span></span> | <span data-ttu-id="a1b3b-120">string</span><span class="sxs-lookup"><span data-stu-id="a1b3b-120">string</span></span> |  <span data-ttu-id="a1b3b-121">Source 属性，应该是源数据中的字段名称的名称。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="a1b3b-122">此属性是区分大小写。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="a1b3b-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="a1b3b-123">**targetPropertyName**</span></span> | <span data-ttu-id="a1b3b-124">string</span><span class="sxs-lookup"><span data-stu-id="a1b3b-124">string</span></span> |  <span data-ttu-id="a1b3b-125">目标属性，应为 Azure AD 中的有效属性名称。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="a1b3b-126">此属性是区分大小写。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="a1b3b-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="a1b3b-127">**targetDomain**</span></span> | <span data-ttu-id="a1b3b-128">string</span><span class="sxs-lookup"><span data-stu-id="a1b3b-128">string</span></span> |  <span data-ttu-id="a1b3b-129">使用 source 属性以匹配目标后缀域。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="a1b3b-130">如果提供为 null，source 属性将用于与目标属性相匹配。</span><span class="sxs-lookup"><span data-stu-id="a1b3b-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="a1b3b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1b3b-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
