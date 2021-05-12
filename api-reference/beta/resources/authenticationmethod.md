---
title: authenticationMethod 资源类型
description: 表示注册到用户的身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9ab808934491793b796be1c66fc87051ed6e9b29
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335623"
---
# <a name="authenticationmethod-resource-type"></a><span data-ttu-id="3ff3e-103">authenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ff3e-103">authenticationMethod resource type</span></span>

<span data-ttu-id="3ff3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ff3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ff3e-105">表示注册到用户的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-105">Represents an authentication method registered to a user.</span></span> <span data-ttu-id="3ff3e-106">[身份验证方法是](/azure/active-directory/authentication/concept-authentication-methods)用户用来向系统进行身份验证或以其他方式证明其身份的方法。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-106">An [authentication method](/azure/active-directory/authentication/concept-authentication-methods) is something used by a user to authenticate or otherwise prove their identity to the system.</span></span> <span data-ttu-id="3ff3e-107">一些示例包括密码、 (电话短信或语音呼叫) 、FIDO2 安全密钥等。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-107">Some examples include password, phone (usable via SMS or voice call), FIDO2 security keys, and more.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3ff3e-108">列出用户的身份验证方法仅返回此 API 版本支持的方法。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-108">Listing users' authentication methods only returns methods supported on this API version.</span></span> <span data-ttu-id="3ff3e-109">有关 [当前支持的方法的列表，请参阅 Azure AD 身份验证](authenticationmethods-overview.md) 方法 API 概述。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-109">See [Azure AD authentication methods API overview](authenticationmethods-overview.md) for a list of currently supported methods.</span></span>

## <a name="methods"></a><span data-ttu-id="3ff3e-110">方法</span><span class="sxs-lookup"><span data-stu-id="3ff3e-110">Methods</span></span>

| <span data-ttu-id="3ff3e-111">方法</span><span class="sxs-lookup"><span data-stu-id="3ff3e-111">Method</span></span>       | <span data-ttu-id="3ff3e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ff3e-112">Return type</span></span> | <span data-ttu-id="3ff3e-113">说明</span><span class="sxs-lookup"><span data-stu-id="3ff3e-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3ff3e-114">列出 authenticationMethods</span><span class="sxs-lookup"><span data-stu-id="3ff3e-114">List authenticationMethods</span></span>](../api/authentication-list-methods.md) | <span data-ttu-id="3ff3e-115">[authenticationMethod](authenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ff3e-115">[authenticationMethod](authenticationmethod.md) collection</span></span> | <span data-ttu-id="3ff3e-116">读取用户的所有 **authenticationMethod** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-116">Read the properties and relationships of all of a user's **authenticationMethod** objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ff3e-117">属性</span><span class="sxs-lookup"><span data-stu-id="3ff3e-117">Properties</span></span>

| <span data-ttu-id="3ff3e-118">属性</span><span class="sxs-lookup"><span data-stu-id="3ff3e-118">Property</span></span>     | <span data-ttu-id="3ff3e-119">类型</span><span class="sxs-lookup"><span data-stu-id="3ff3e-119">Type</span></span>        | <span data-ttu-id="3ff3e-120">说明</span><span class="sxs-lookup"><span data-stu-id="3ff3e-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ff3e-121">id</span><span class="sxs-lookup"><span data-stu-id="3ff3e-121">id</span></span>|<span data-ttu-id="3ff3e-122">String</span><span class="sxs-lookup"><span data-stu-id="3ff3e-122">String</span></span>| <span data-ttu-id="3ff3e-123">注册到此用户的身份验证方法的此实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-123">The identifier of this instance of an authentication method registered to this user.</span></span> <span data-ttu-id="3ff3e-124">只读。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3ff3e-125">关系</span><span class="sxs-lookup"><span data-stu-id="3ff3e-125">Relationships</span></span>

<span data-ttu-id="3ff3e-126">无。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ff3e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ff3e-127">JSON representation</span></span>

<span data-ttu-id="3ff3e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ff3e-128">The following is a JSON representation of the resource.</span></span>

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