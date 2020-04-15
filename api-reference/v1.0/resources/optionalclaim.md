---
title: optionalClaim 资源类型
description: 在此处提供说明
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: def69ff8da77eedbaf4cd48669594994764cb2a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468322"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="44365-103">optionalClaim 资源类型</span><span class="sxs-lookup"><span data-stu-id="44365-103">optionalClaim resource type</span></span>

<span data-ttu-id="44365-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44365-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44365-105">包含与[应用程序](application.md)关联的可选声明</span><span class="sxs-lookup"><span data-stu-id="44365-105">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="44365-106">.</span><span class="sxs-lookup"><span data-stu-id="44365-106">.</span></span> <span data-ttu-id="44365-107">OptionalClaims `idToken`资源`accessToken`的、 `saml2Token`和属性是[optionalClaims](optionalclaims.md) **optionalClaim**的集合。</span><span class="sxs-lookup"><span data-stu-id="44365-107">The `idToken`, `accessToken`, and `saml2Token` properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="44365-108">如果特定声明支持，还可以使用`additionalProperties`属性修改 optionalClaim 的行为。</span><span class="sxs-lookup"><span data-stu-id="44365-108">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span>

<span data-ttu-id="44365-109">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="44365-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="44365-110">属性</span><span class="sxs-lookup"><span data-stu-id="44365-110">Properties</span></span>

| <span data-ttu-id="44365-111">属性</span><span class="sxs-lookup"><span data-stu-id="44365-111">Property</span></span>     | <span data-ttu-id="44365-112">类型</span><span class="sxs-lookup"><span data-stu-id="44365-112">Type</span></span>        | <span data-ttu-id="44365-113">说明</span><span class="sxs-lookup"><span data-stu-id="44365-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44365-114">additionalProperties</span><span class="sxs-lookup"><span data-stu-id="44365-114">additionalProperties</span></span>|<span data-ttu-id="44365-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="44365-115">String collection</span></span>| <span data-ttu-id="44365-116">声明的其他属性。</span><span class="sxs-lookup"><span data-stu-id="44365-116">Additional properties of the claim.</span></span> <span data-ttu-id="44365-117">如果某个属性存在于此集合中，它将修改在 name 属性中指定的可选声明的行为。</span><span class="sxs-lookup"><span data-stu-id="44365-117">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="44365-118">组成部分</span><span class="sxs-lookup"><span data-stu-id="44365-118">essential</span></span>|<span data-ttu-id="44365-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="44365-119">Boolean</span></span>| <span data-ttu-id="44365-120">如果值为 true，则客户端指定的声明是为确保最终用户请求的特定任务的平稳授权体验所必需的。</span><span class="sxs-lookup"><span data-stu-id="44365-120">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="44365-121">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="44365-121">The default value is false.</span></span>|
|<span data-ttu-id="44365-122">name</span><span class="sxs-lookup"><span data-stu-id="44365-122">name</span></span>|<span data-ttu-id="44365-123">String</span><span class="sxs-lookup"><span data-stu-id="44365-123">String</span></span>| <span data-ttu-id="44365-124">可选声明的名称。</span><span class="sxs-lookup"><span data-stu-id="44365-124">The name of the optional claim.</span></span> |
|<span data-ttu-id="44365-125">source</span><span class="sxs-lookup"><span data-stu-id="44365-125">source</span></span>|<span data-ttu-id="44365-126">String</span><span class="sxs-lookup"><span data-stu-id="44365-126">String</span></span>| <span data-ttu-id="44365-127">声明的源（目录对象）。</span><span class="sxs-lookup"><span data-stu-id="44365-127">The source (directory object) of the claim.</span></span> <span data-ttu-id="44365-128">来自扩展属性的预定义声明和用户定义的声明。</span><span class="sxs-lookup"><span data-stu-id="44365-128">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="44365-129">如果源值为 null，则声明是预定义的可选声明。</span><span class="sxs-lookup"><span data-stu-id="44365-129">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="44365-130">如果源值为 user，则 name 属性中的值是用户对象的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44365-130">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44365-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44365-131">JSON representation</span></span>

<span data-ttu-id="44365-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44365-132">The following is a JSON representation of the resource.</span></span>

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