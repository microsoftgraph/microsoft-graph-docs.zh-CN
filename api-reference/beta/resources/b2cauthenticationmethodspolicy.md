---
title: b2cAuthenticationMethodsPolicy资源类型
description: 表示注册给在 Azure Active Directory （Azure AD） B2C 租户中配置的用户的本地帐户身份验证方法。
localization_priority: Priority
author: namkedia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e6b49f389e59b3f314414e2766a5e8fe9e3a9a6c
ms.sourcegitcommit: 92f545d2d9af13ac7aff9932eb265f136d089f79
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2021
ms.locfileid: "51996099"
---
# <a name="b2cauthenticationmethodspolicy-resource-type"></a><span data-ttu-id="73fc1-103">b2cAuthenticationMethodsPolicy资源类型</span><span class="sxs-lookup"><span data-stu-id="73fc1-103">b2cAuthenticationMethodsPolicy resource type</span></span>

<span data-ttu-id="73fc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73fc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73fc1-105">Azure Active Directory （Azure AD） B2C 允许租户管理员选择让最终用户通过本地账户注册的机制。</span><span class="sxs-lookup"><span data-stu-id="73fc1-105">Azure Active Directory (Azure AD) B2C allows tenant admins to choose a mechanism for letting end users register via local accounts.</span></span> <span data-ttu-id="73fc1-106">本地帐户是指由 Azure AD 执行标识断言的帐户，而不是Google或Facebook等联合身份提供商。</span><span class="sxs-lookup"><span data-stu-id="73fc1-106">Local accounts are the accounts where Azure AD does the identity assertion, as opposed to a federated identity provider such as Google or Facebook etc.</span></span>

<span data-ttu-id="73fc1-107">Azure AD B2C 中的本地帐户未遵循来自 Azure AD 的设置或范式。</span><span class="sxs-lookup"><span data-stu-id="73fc1-107">The local accounts in Azure AD B2C do not follow the settings or paradigms from Azure AD.</span></span> <span data-ttu-id="73fc1-108">Azure ad B2C 未使用或执行 Azure AD 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="73fc1-108">The Azure AD authentication methods policy is not used or enforced by Azure AD B2C.</span></span> <span data-ttu-id="73fc1-109">Azure AD B2C 将这些设置存储在不同的策略中，由用户流来消耗。</span><span class="sxs-lookup"><span data-stu-id="73fc1-109">Azure AD B2C stores these settings in a different policy, which is consumed by user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="73fc1-110">方法</span><span class="sxs-lookup"><span data-stu-id="73fc1-110">Methods</span></span>

| <span data-ttu-id="73fc1-111">方法</span><span class="sxs-lookup"><span data-stu-id="73fc1-111">Method</span></span>       | <span data-ttu-id="73fc1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="73fc1-112">Return type</span></span> | <span data-ttu-id="73fc1-113">Description</span><span class="sxs-lookup"><span data-stu-id="73fc1-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="73fc1-114">获取 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="73fc1-114">Get b2cAuthenticationMethodsPolicy</span></span>](../api/b2cauthenticationmethodspolicy-get.md) | [<span data-ttu-id="73fc1-115">b2cauthenticationmethodspolicy</span><span class="sxs-lookup"><span data-stu-id="73fc1-115">b2cauthenticationmethodspolicy</span></span>](b2cauthenticationmethodspolicy.md) | <span data-ttu-id="73fc1-116">读取 **b2cauthenticationmethodspolicy** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73fc1-116">Read the properties of a **b2cauthenticationmethodspolicy** object.</span></span> |
| [<span data-ttu-id="73fc1-117">更新 b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="73fc1-117">Update b2cAuthenticationMethodsPolicy</span></span>](../api/b2cauthenticationmethodspolicy-update.md) | <span data-ttu-id="73fc1-118">无</span><span class="sxs-lookup"><span data-stu-id="73fc1-118">None</span></span> | <span data-ttu-id="73fc1-119">更新 **b2cauthenticationmethodspolicy** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73fc1-119">Update the properties of a **b2cauthenticationmethodspolicy** objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="73fc1-120">属性</span><span class="sxs-lookup"><span data-stu-id="73fc1-120">Properties</span></span>

| <span data-ttu-id="73fc1-121">属性</span><span class="sxs-lookup"><span data-stu-id="73fc1-121">Property</span></span>     | <span data-ttu-id="73fc1-122">类型</span><span class="sxs-lookup"><span data-stu-id="73fc1-122">Type</span></span>        | <span data-ttu-id="73fc1-123">说明</span><span class="sxs-lookup"><span data-stu-id="73fc1-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73fc1-124">id</span><span class="sxs-lookup"><span data-stu-id="73fc1-124">id</span></span>|<span data-ttu-id="73fc1-125">String</span><span class="sxs-lookup"><span data-stu-id="73fc1-125">String</span></span>|<span data-ttu-id="73fc1-126">B2C认证方式策略的id。</span><span class="sxs-lookup"><span data-stu-id="73fc1-126">The id of the B2C authentication methods policy.</span></span> <span data-ttu-id="73fc1-127">这是一个只读属性，也是关键所在。</span><span class="sxs-lookup"><span data-stu-id="73fc1-127">This is a read only property and the key.</span></span>|
|<span data-ttu-id="73fc1-128">isEmailPasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="73fc1-128">isEmailPasswordAuthenticationEnabled</span></span>|<span data-ttu-id="73fc1-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="73fc1-129">Boolean</span></span>|<span data-ttu-id="73fc1-130">如果启用了电子邮件和密码身份验证方法，租户管理员可以使用电子邮件配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="73fc1-130">The tenant admin can configure local accounts using email if the email and password authentication method is enabled.</span></span>|
|<span data-ttu-id="73fc1-131">isUserNameAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="73fc1-131">isUserNameAuthenticationEnabled</span></span>|<span data-ttu-id="73fc1-132">布尔值</span><span class="sxs-lookup"><span data-stu-id="73fc1-132">Boolean</span></span>|<span data-ttu-id="73fc1-133">如果启用了用户名和密码身份验证方法，租户管理员可以使用用户名配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="73fc1-133">The tenant admin can configure local accounts using username if the username and password authentication method is enabled.</span></span>|
|<span data-ttu-id="73fc1-134">isPhoneOneTimePasswordAuthenticationEnabled</span><span class="sxs-lookup"><span data-stu-id="73fc1-134">isPhoneOneTimePasswordAuthenticationEnabled</span></span>|<span data-ttu-id="73fc1-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="73fc1-135">Boolean</span></span>|<span data-ttu-id="73fc1-136">如果已启用电话号码和一次性密码身份验证方法，则租户管理员可以使用电话号码配置本地帐户。</span><span class="sxs-lookup"><span data-stu-id="73fc1-136">The tenant admin can configure local accounts using phone number if the phone number and one-time password authentication method is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73fc1-137">关系</span><span class="sxs-lookup"><span data-stu-id="73fc1-137">Relationships</span></span>

<span data-ttu-id="73fc1-138">无。</span><span class="sxs-lookup"><span data-stu-id="73fc1-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73fc1-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73fc1-139">JSON representation</span></span>

<span data-ttu-id="73fc1-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73fc1-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false,
    "isPhoneOneTimePasswordAuthenticationEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "b2cAuthenticationMethodsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
