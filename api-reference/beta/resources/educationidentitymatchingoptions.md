---
title: educationIdentityMatchingOptions 资源类型
description: 提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c2b092d5589cdccccfe73a7e71afcafa7b555a90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425790"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="c9ddb-105">educationIdentityMatchingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9ddb-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="c9ddb-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9ddb-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9ddb-108">提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="c9ddb-109">Source 属性应存在的源数据中。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-109">The source property should exist in the source data.</span></span> <span data-ttu-id="c9ddb-110">目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="c9ddb-111">属性</span><span class="sxs-lookup"><span data-stu-id="c9ddb-111">Properties</span></span>

| <span data-ttu-id="c9ddb-112">属性</span><span class="sxs-lookup"><span data-stu-id="c9ddb-112">Property</span></span> | <span data-ttu-id="c9ddb-113">类型</span><span class="sxs-lookup"><span data-stu-id="c9ddb-113">Type</span></span> | <span data-ttu-id="c9ddb-114">说明</span><span class="sxs-lookup"><span data-stu-id="c9ddb-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c9ddb-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="c9ddb-115">**appliesTo**</span></span> | <span data-ttu-id="c9ddb-116">string</span><span class="sxs-lookup"><span data-stu-id="c9ddb-116">string</span></span> |  <span data-ttu-id="c9ddb-117">要分配许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-117">The user role type to assign to the license.</span></span> <span data-ttu-id="c9ddb-118">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="c9ddb-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="c9ddb-119">**sourcePropertyName**</span></span> | <span data-ttu-id="c9ddb-120">string</span><span class="sxs-lookup"><span data-stu-id="c9ddb-120">string</span></span> |  <span data-ttu-id="c9ddb-121">Source 属性，应该是源数据中的字段名称的名称。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="c9ddb-122">此属性是区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="c9ddb-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="c9ddb-123">**targetPropertyName**</span></span> | <span data-ttu-id="c9ddb-124">string</span><span class="sxs-lookup"><span data-stu-id="c9ddb-124">string</span></span> |  <span data-ttu-id="c9ddb-125">目标属性，应为 Azure AD 中的有效属性名称。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="c9ddb-126">此属性是区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="c9ddb-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="c9ddb-127">**targetDomain**</span></span> | <span data-ttu-id="c9ddb-128">string</span><span class="sxs-lookup"><span data-stu-id="c9ddb-128">string</span></span> |  <span data-ttu-id="c9ddb-129">使用 source 属性以匹配目标后缀域。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="c9ddb-130">如果提供为 null，source 属性将用于与目标属性相匹配。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="c9ddb-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9ddb-131">JSON representation</span></span>
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
