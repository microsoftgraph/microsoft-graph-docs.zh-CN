---
title: authenticationMethod 资源类型
description: 表示向用户注册的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fefa2ed8ee17a898b51e7bc21b3e13ec64f68d56
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557834"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="92b26-103">authenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="92b26-103">authenticationMethod resource type</span></span>

<span data-ttu-id="92b26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92b26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92b26-105">表示向用户注册的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="92b26-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="92b26-106">[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)是用户使用的一种方法，用于对系统进行身份验证或为其证明身份。</span><span class="sxs-lookup"><span data-stu-id="92b26-106">An [authentication method](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="92b26-107">一些示例包括密码、电话（可通过短信或语音呼叫使用）、FIDO2 安全密钥等。</span><span class="sxs-lookup"><span data-stu-id="92b26-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span> <span data-ttu-id="92b26-108">目前实施了密码和电话方法。</span><span class="sxs-lookup"><span data-stu-id="92b26-108">Currently, password and phone methods are implemented.</span></span>

## <a name="methods"></a><span data-ttu-id="92b26-109">方法</span><span class="sxs-lookup"><span data-stu-id="92b26-109">Methods</span></span>

| <span data-ttu-id="92b26-110">方法</span><span class="sxs-lookup"><span data-stu-id="92b26-110">Method</span></span>       | <span data-ttu-id="92b26-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="92b26-111">Return type</span></span> | <span data-ttu-id="92b26-112">说明</span><span class="sxs-lookup"><span data-stu-id="92b26-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="92b26-113">列出 authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="92b26-113">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="92b26-114">[authenticationMethod](authenticationmethod.md)集合</span><span class="sxs-lookup"><span data-stu-id="92b26-114">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="92b26-115">读取用户的所有**authenticationMethod**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92b26-115">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="92b26-116">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92b26-116">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="92b26-117">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92b26-117">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="92b26-118">读取**authenticationMethod**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92b26-118">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="92b26-119">属性</span><span class="sxs-lookup"><span data-stu-id="92b26-119">Properties</span></span>

| <span data-ttu-id="92b26-120">属性</span><span class="sxs-lookup"><span data-stu-id="92b26-120">Property</span></span>     | <span data-ttu-id="92b26-121">类型</span><span class="sxs-lookup"><span data-stu-id="92b26-121">Type</span></span>        | <span data-ttu-id="92b26-122">说明</span><span class="sxs-lookup"><span data-stu-id="92b26-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92b26-123">id</span><span class="sxs-lookup"><span data-stu-id="92b26-123">id</span></span>|<span data-ttu-id="92b26-124">String</span><span class="sxs-lookup"><span data-stu-id="92b26-124">String</span></span>| <span data-ttu-id="92b26-125">向此用户注册的身份验证方法的此实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="92b26-125">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="92b26-126">只读。</span><span class="sxs-lookup"><span data-stu-id="92b26-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="92b26-127">关系</span><span class="sxs-lookup"><span data-stu-id="92b26-127">Relationships</span></span>

<span data-ttu-id="92b26-128">无。</span><span class="sxs-lookup"><span data-stu-id="92b26-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92b26-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92b26-129">JSON representation</span></span>

<span data-ttu-id="92b26-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92b26-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "",
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
