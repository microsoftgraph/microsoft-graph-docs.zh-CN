---
title: authenticationMethod 资源类型
description: 表示向用户注册的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6afb785527b2d2448e54533ce02c0a72bf84353
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402343"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="f695a-103">authenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="f695a-103">authenticationMethod resource type</span></span>

<span data-ttu-id="f695a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f695a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f695a-105">表示向用户注册的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f695a-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="f695a-106">[身份验证方法](/azure/active-directory/authentication/concept-authentication-methods)是用户使用的一种方法，用于对系统进行身份验证或为其证明身份。</span><span class="sxs-lookup"><span data-stu-id="f695a-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="f695a-107">一些示例包括密码、电话 (可通过短信或语音呼叫) FIDO2 安全密钥等。</span><span class="sxs-lookup"><span data-stu-id="f695a-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span> <span data-ttu-id="f695a-108">目前实施了密码和电话方法。</span><span class="sxs-lookup"><span data-stu-id="f695a-108">Currently, password and phone methods are implemented.</span></span>

## <a name="methods"></a><span data-ttu-id="f695a-109">方法</span><span class="sxs-lookup"><span data-stu-id="f695a-109">Methods</span></span>

| <span data-ttu-id="f695a-110">方法</span><span class="sxs-lookup"><span data-stu-id="f695a-110">Method</span></span>       | <span data-ttu-id="f695a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f695a-111">Return type</span></span> | <span data-ttu-id="f695a-112">说明</span><span class="sxs-lookup"><span data-stu-id="f695a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f695a-113">列出 authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="f695a-113">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="f695a-114">[authenticationMethod](authenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f695a-114">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="f695a-115">读取用户的所有 **authenticationMethod** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f695a-115">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |
| [<span data-ttu-id="f695a-116">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f695a-116">Get authenticationMethod</span></span>](../api/authenticationmethod-get.md) | [<span data-ttu-id="f695a-117">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f695a-117">authenticationMethod</span></span>](authenticationmethod.md) | <span data-ttu-id="f695a-118">读取 **authenticationMethod** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f695a-118">Read the properties and relationships of an **authenticationMethod** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f695a-119">属性</span><span class="sxs-lookup"><span data-stu-id="f695a-119">Properties</span></span>

| <span data-ttu-id="f695a-120">属性</span><span class="sxs-lookup"><span data-stu-id="f695a-120">Property</span></span>     | <span data-ttu-id="f695a-121">类型</span><span class="sxs-lookup"><span data-stu-id="f695a-121">Type</span></span>        | <span data-ttu-id="f695a-122">说明</span><span class="sxs-lookup"><span data-stu-id="f695a-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f695a-123">id</span><span class="sxs-lookup"><span data-stu-id="f695a-123">id</span></span>|<span data-ttu-id="f695a-124">字符串</span><span class="sxs-lookup"><span data-stu-id="f695a-124">String</span></span>| <span data-ttu-id="f695a-125">向此用户注册的身份验证方法的此实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="f695a-125">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="f695a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="f695a-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f695a-127">关系</span><span class="sxs-lookup"><span data-stu-id="f695a-127">Relationships</span></span>

<span data-ttu-id="f695a-128">无。</span><span class="sxs-lookup"><span data-stu-id="f695a-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f695a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f695a-129">JSON representation</span></span>

<span data-ttu-id="f695a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f695a-130">The following is a JSON representation of the resource.</span></span>

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