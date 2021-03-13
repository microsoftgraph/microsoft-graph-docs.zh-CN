---
title: authenticationMethod 资源类型
description: 表示注册到用户的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cf36866aa0263896a4f7d8a0a4f59146f2f934cb
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761477"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="5fabf-103">authenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fabf-103">authenticationMethod resource type</span></span>

<span data-ttu-id="5fabf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fabf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fabf-105">表示注册到用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="5fabf-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="5fabf-106">[身份验证方法是](/azure/active-directory/authentication/concept-authentication-methods)用户用来向系统进行身份验证或以其他方式证明其身份的方法。</span><span class="sxs-lookup"><span data-stu-id="5fabf-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="5fabf-107">一些示例包括密码、 (短信或语音呼叫) 、FIDO2 安全密钥等。</span><span class="sxs-lookup"><span data-stu-id="5fabf-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

## <a name="methods"></a><span data-ttu-id="5fabf-108">方法</span><span class="sxs-lookup"><span data-stu-id="5fabf-108">Methods</span></span>

| <span data-ttu-id="5fabf-109">方法</span><span class="sxs-lookup"><span data-stu-id="5fabf-109">Method</span></span>       | <span data-ttu-id="5fabf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fabf-110">Return type</span></span> | <span data-ttu-id="5fabf-111">说明</span><span class="sxs-lookup"><span data-stu-id="5fabf-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5fabf-112">列出 authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="5fabf-112">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="5fabf-113">[authenticationMethod](authenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fabf-113">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="5fabf-114">读取用户的所有 **authenticationMethod** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5fabf-114">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="5fabf-115">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5fabf-115">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="5fabf-116">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5fabf-116">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="5fabf-117">读取 **authenticationMethod 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="5fabf-117">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fabf-118">属性</span><span class="sxs-lookup"><span data-stu-id="5fabf-118">Properties</span></span>

| <span data-ttu-id="5fabf-119">属性</span><span class="sxs-lookup"><span data-stu-id="5fabf-119">Property</span></span>     | <span data-ttu-id="5fabf-120">类型</span><span class="sxs-lookup"><span data-stu-id="5fabf-120">Type</span></span>        | <span data-ttu-id="5fabf-121">说明</span><span class="sxs-lookup"><span data-stu-id="5fabf-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5fabf-122">id</span><span class="sxs-lookup"><span data-stu-id="5fabf-122">id</span></span>|<span data-ttu-id="5fabf-123">String</span><span class="sxs-lookup"><span data-stu-id="5fabf-123">String</span></span>| <span data-ttu-id="5fabf-124">注册到此用户的身份验证方法的此实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="5fabf-124">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="5fabf-125">只读。</span><span class="sxs-lookup"><span data-stu-id="5fabf-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5fabf-126">关系</span><span class="sxs-lookup"><span data-stu-id="5fabf-126">Relationships</span></span>

<span data-ttu-id="5fabf-127">无。</span><span class="sxs-lookup"><span data-stu-id="5fabf-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fabf-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fabf-128">JSON representation</span></span>

<span data-ttu-id="5fabf-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fabf-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->