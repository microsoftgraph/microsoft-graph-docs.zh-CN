---
title: optionalClaim 资源类型
description: 在此处提供说明
localization_priority: Normal
author: sureshja
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 355a9e558f76a8dd38ea227950bb9c3938aa21c4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869813"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="9fcac-103">optionalClaim 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fcac-103">optionalClaim resource type</span></span>

<span data-ttu-id="9fcac-104">包含与[应用程序](application.md)关联的可选声明</span><span class="sxs-lookup"><span data-stu-id="9fcac-104">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="9fcac-105">.</span><span class="sxs-lookup"><span data-stu-id="9fcac-105"></span></span> <span data-ttu-id="9fcac-106">OptionalClaims `idToken`资源`accessToken`的、 `saml2Token`和属性是[](optionalclaims.md) **optionalClaim**的集合。</span><span class="sxs-lookup"><span data-stu-id="9fcac-106">The `idToken`, `accessToken`, and `saml2Token` properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="9fcac-107">如果特定声明支持，还可以使用`additionalProperties`属性修改 optionalClaim 的行为。</span><span class="sxs-lookup"><span data-stu-id="9fcac-107">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span>

<span data-ttu-id="9fcac-108">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="9fcac-108">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="9fcac-109">属性</span><span class="sxs-lookup"><span data-stu-id="9fcac-109">Properties</span></span>

| <span data-ttu-id="9fcac-110">属性</span><span class="sxs-lookup"><span data-stu-id="9fcac-110">Property</span></span>     | <span data-ttu-id="9fcac-111">类型</span><span class="sxs-lookup"><span data-stu-id="9fcac-111">Type</span></span>        | <span data-ttu-id="9fcac-112">说明</span><span class="sxs-lookup"><span data-stu-id="9fcac-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9fcac-113">additionalProperties</span><span class="sxs-lookup"><span data-stu-id="9fcac-113">additionalProperties</span></span>|<span data-ttu-id="9fcac-114">String collection</span><span class="sxs-lookup"><span data-stu-id="9fcac-114">String collection</span></span>| <span data-ttu-id="9fcac-115">声明的其他属性。</span><span class="sxs-lookup"><span data-stu-id="9fcac-115">Additional properties of the claim.</span></span> <span data-ttu-id="9fcac-116">如果某个属性存在于此集合中，它将修改在 name 属性中指定的可选声明的行为。</span><span class="sxs-lookup"><span data-stu-id="9fcac-116">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="9fcac-117">组成部分</span><span class="sxs-lookup"><span data-stu-id="9fcac-117">essential</span></span>|<span data-ttu-id="9fcac-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcac-118">Boolean</span></span>| <span data-ttu-id="9fcac-119">如果值为 true，则客户端指定的声明是为确保最终用户请求的特定任务的平稳授权体验所必需的。</span><span class="sxs-lookup"><span data-stu-id="9fcac-119">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="9fcac-120">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="9fcac-120">The default value is false.</span></span>|
|<span data-ttu-id="9fcac-121">name</span><span class="sxs-lookup"><span data-stu-id="9fcac-121">name</span></span>|<span data-ttu-id="9fcac-122">String</span><span class="sxs-lookup"><span data-stu-id="9fcac-122">String</span></span>| <span data-ttu-id="9fcac-123">可选声明的名称。</span><span class="sxs-lookup"><span data-stu-id="9fcac-123">The name of the optional claim.</span></span> |
|<span data-ttu-id="9fcac-124">source</span><span class="sxs-lookup"><span data-stu-id="9fcac-124">source</span></span>|<span data-ttu-id="9fcac-125">String</span><span class="sxs-lookup"><span data-stu-id="9fcac-125">String</span></span>| <span data-ttu-id="9fcac-126">声明的源（目录对象）。</span><span class="sxs-lookup"><span data-stu-id="9fcac-126">The source (directory object) of the claim.</span></span> <span data-ttu-id="9fcac-127">来自扩展属性的预定义声明和用户定义的声明。</span><span class="sxs-lookup"><span data-stu-id="9fcac-127">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="9fcac-128">如果源值为 null，则声明是预定义的可选声明。</span><span class="sxs-lookup"><span data-stu-id="9fcac-128">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="9fcac-129">如果源值为 user，则 name 属性中的值是用户对象的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="9fcac-129">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9fcac-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fcac-130">JSON representation</span></span>

<span data-ttu-id="9fcac-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fcac-131">The following is a JSON representation of the resource.</span></span>

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