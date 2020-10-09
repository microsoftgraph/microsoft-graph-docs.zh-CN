---
title: optionalClaim 资源类型
description: 包含与应用程序关联的可选声明。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f40574cb80ab458d1675507b796b43b95e19cf41
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401144"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="601d4-103">optionalClaim 资源类型</span><span class="sxs-lookup"><span data-stu-id="601d4-103">optionalClaim resource type</span></span>

<span data-ttu-id="601d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="601d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="601d4-105">包含与[应用程序](application.md)关联的可选声明</span><span class="sxs-lookup"><span data-stu-id="601d4-105">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="601d4-106">.</span><span class="sxs-lookup"><span data-stu-id="601d4-106">.</span></span> <span data-ttu-id="601d4-107">[OptionalClaims](optionalclaims.md)资源的**idToken**、 **AccessToken**和**saml2Token**属性是**optionalClaim**的集合。</span><span class="sxs-lookup"><span data-stu-id="601d4-107">The **idToken**, **accessToken**, and **saml2Token** properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="601d4-108">如果特定声明支持，还可以使用属性修改 optionalClaim 的行为 `additionalProperties` 。</span><span class="sxs-lookup"><span data-stu-id="601d4-108">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span> 

<span data-ttu-id="601d4-109">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="601d4-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="601d4-110">属性</span><span class="sxs-lookup"><span data-stu-id="601d4-110">Properties</span></span>

| <span data-ttu-id="601d4-111">属性</span><span class="sxs-lookup"><span data-stu-id="601d4-111">Property</span></span>     | <span data-ttu-id="601d4-112">类型</span><span class="sxs-lookup"><span data-stu-id="601d4-112">Type</span></span>        | <span data-ttu-id="601d4-113">说明</span><span class="sxs-lookup"><span data-stu-id="601d4-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="601d4-114">additionalProperties</span><span class="sxs-lookup"><span data-stu-id="601d4-114">additionalProperties</span></span>|<span data-ttu-id="601d4-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="601d4-115">String collection</span></span>| <span data-ttu-id="601d4-116">声明的其他属性。</span><span class="sxs-lookup"><span data-stu-id="601d4-116">Additional properties of the claim.</span></span> <span data-ttu-id="601d4-117">如果某个属性存在于此集合中，它将修改在 name 属性中指定的可选声明的行为。</span><span class="sxs-lookup"><span data-stu-id="601d4-117">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="601d4-118">组成部分</span><span class="sxs-lookup"><span data-stu-id="601d4-118">essential</span></span>|<span data-ttu-id="601d4-119">布尔</span><span class="sxs-lookup"><span data-stu-id="601d4-119">Boolean</span></span>| <span data-ttu-id="601d4-120">如果值为 true，则客户端指定的声明是为确保最终用户请求的特定任务的平稳授权体验所必需的。</span><span class="sxs-lookup"><span data-stu-id="601d4-120">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="601d4-121">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="601d4-121">The default value is false.</span></span>|
|<span data-ttu-id="601d4-122">name</span><span class="sxs-lookup"><span data-stu-id="601d4-122">name</span></span>|<span data-ttu-id="601d4-123">字符串</span><span class="sxs-lookup"><span data-stu-id="601d4-123">String</span></span>| <span data-ttu-id="601d4-124">可选声明的名称。</span><span class="sxs-lookup"><span data-stu-id="601d4-124">The name of the optional claim.</span></span> |
|<span data-ttu-id="601d4-125">source</span><span class="sxs-lookup"><span data-stu-id="601d4-125">source</span></span>|<span data-ttu-id="601d4-126">字符串</span><span class="sxs-lookup"><span data-stu-id="601d4-126">String</span></span>| <span data-ttu-id="601d4-127">声明的源 (directory 对象) 。</span><span class="sxs-lookup"><span data-stu-id="601d4-127">The source (directory object) of the claim.</span></span> <span data-ttu-id="601d4-128">来自扩展属性的预定义声明和用户定义的声明。</span><span class="sxs-lookup"><span data-stu-id="601d4-128">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="601d4-129">如果源值为 null，则声明是预定义的可选声明。</span><span class="sxs-lookup"><span data-stu-id="601d4-129">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="601d4-130">如果源值为 user，则 name 属性中的值是用户对象的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="601d4-130">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="601d4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="601d4-131">JSON representation</span></span>

<span data-ttu-id="601d4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="601d4-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.optionalClaim",
  "baseType": null
}-->

```json
{
  "additionalProperties": ["String"],
  "essential": true,
  "name": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "optionalClaim resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->