---
title: optionalClaim 资源类型
description: 包含与应用程序关联的可选声明。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5e21ab86fb3ef34edea546546211782906e04251
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128531"
---
# <a name="optionalclaim-resource-type"></a><span data-ttu-id="8f45e-103">optionalClaim 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f45e-103">optionalClaim resource type</span></span>

<span data-ttu-id="8f45e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f45e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f45e-105">包含与应用程序关联的可选 [声明](application.md)</span><span class="sxs-lookup"><span data-stu-id="8f45e-105">Contains an optional claim associated with an [application](application.md)</span></span> <!-- or a service principal --><span data-ttu-id="8f45e-106">.</span><span class="sxs-lookup"><span data-stu-id="8f45e-106">.</span></span> <span data-ttu-id="8f45e-107">[optionalClaims](optionalclaims.md)资源的 **idToken** **、accessToken** 和 **saml2Token** 属性是 **optionalClaim 的集合**。</span><span class="sxs-lookup"><span data-stu-id="8f45e-107">The **idToken**, **accessToken**, and **saml2Token** properties of the [optionalClaims](optionalclaims.md) resource is a collection of **optionalClaim**.</span></span> <span data-ttu-id="8f45e-108">如果特定声明支持，您还可以使用该属性修改 optionalClaim `additionalProperties` 的行为。</span><span class="sxs-lookup"><span data-stu-id="8f45e-108">If supported by a specific claim, you can also modify the behavior of the optionalClaim using the `additionalProperties` property.</span></span> 

<span data-ttu-id="8f45e-109">有关详细信息，请参阅[向 Azure AD 应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="8f45e-109">See [provide optional claims to your Azure AD app](/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span>

## <a name="properties"></a><span data-ttu-id="8f45e-110">属性</span><span class="sxs-lookup"><span data-stu-id="8f45e-110">Properties</span></span>

| <span data-ttu-id="8f45e-111">属性</span><span class="sxs-lookup"><span data-stu-id="8f45e-111">Property</span></span>     | <span data-ttu-id="8f45e-112">类型</span><span class="sxs-lookup"><span data-stu-id="8f45e-112">Type</span></span>        | <span data-ttu-id="8f45e-113">说明</span><span class="sxs-lookup"><span data-stu-id="8f45e-113">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f45e-114">additionalProperties</span><span class="sxs-lookup"><span data-stu-id="8f45e-114">additionalProperties</span></span>|<span data-ttu-id="8f45e-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8f45e-115">String collection</span></span>| <span data-ttu-id="8f45e-116">声明的其他属性。</span><span class="sxs-lookup"><span data-stu-id="8f45e-116">Additional properties of the claim.</span></span> <span data-ttu-id="8f45e-117">如果属性存在于该集合中，则它会修改在 name 属性中指定的可选声明的行为。</span><span class="sxs-lookup"><span data-stu-id="8f45e-117">If a property exists in this collection, it modifies the behavior of the optional claim specified in the name property.</span></span> |
|<span data-ttu-id="8f45e-118">essential</span><span class="sxs-lookup"><span data-stu-id="8f45e-118">essential</span></span>|<span data-ttu-id="8f45e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f45e-119">Boolean</span></span>| <span data-ttu-id="8f45e-120">如果值为 true，则客户端指定的声明是确保最终用户请求的特定任务的流畅授权体验所必需的。</span><span class="sxs-lookup"><span data-stu-id="8f45e-120">If the value is true, the claim specified by the client is necessary to ensure a smooth authorization experience for the specific task requested by the end user.</span></span> <span data-ttu-id="8f45e-121">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="8f45e-121">The default value is false.</span></span>|
|<span data-ttu-id="8f45e-122">name</span><span class="sxs-lookup"><span data-stu-id="8f45e-122">name</span></span>|<span data-ttu-id="8f45e-123">字符串</span><span class="sxs-lookup"><span data-stu-id="8f45e-123">String</span></span>| <span data-ttu-id="8f45e-124">可选声明的名称。</span><span class="sxs-lookup"><span data-stu-id="8f45e-124">The name of the optional claim.</span></span> |
|<span data-ttu-id="8f45e-125">source</span><span class="sxs-lookup"><span data-stu-id="8f45e-125">source</span></span>|<span data-ttu-id="8f45e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="8f45e-126">String</span></span>| <span data-ttu-id="8f45e-127">源 (声明) 目录对象。</span><span class="sxs-lookup"><span data-stu-id="8f45e-127">The source (directory object) of the claim.</span></span> <span data-ttu-id="8f45e-128">扩展属性中具有预定义声明和用户定义的声明。</span><span class="sxs-lookup"><span data-stu-id="8f45e-128">There are predefined claims and user-defined claims from extension properties.</span></span> <span data-ttu-id="8f45e-129">如果源值为空，则声明是预定义的可选声明。</span><span class="sxs-lookup"><span data-stu-id="8f45e-129">If the source value is null, the claim is a predefined optional claim.</span></span> <span data-ttu-id="8f45e-130">如果源值是用户，则 name 属性中的值是用户对象的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8f45e-130">If the source value is user, the value in the name property is the extension property from the user object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f45e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f45e-131">JSON representation</span></span>

<span data-ttu-id="8f45e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f45e-132">The following is a JSON representation of the resource.</span></span>

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
