---
title: credentialUserRegistrationDetails 资源类型
description: 表示所有注册用户的 MFA 身份验证中自助服务密码重置和多重 (身份验证) 的详细信息。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c7e45b186e1ef7a3a96115f408cb5a0992e538fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159904"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="09885-103">credentialUserRegistrationDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="09885-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="09885-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09885-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09885-105">表示所有注册用户的 MFA 身份验证中自助服务密码重置和多重 (身份验证) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="09885-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="09885-106">详细信息包括用户信息、注册状态和使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="09885-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="09885-107">方法</span><span class="sxs-lookup"><span data-stu-id="09885-107">Methods</span></span>

| <span data-ttu-id="09885-108">方法</span><span class="sxs-lookup"><span data-stu-id="09885-108">Method</span></span>       | <span data-ttu-id="09885-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="09885-109">Return Type</span></span> | <span data-ttu-id="09885-110">说明</span><span class="sxs-lookup"><span data-stu-id="09885-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="09885-111">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="09885-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="09885-112">credentialUserRegistrationDetails 集合</span><span class="sxs-lookup"><span data-stu-id="09885-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="09885-113">获取给定租户 [的 credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="09885-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="09885-114">属性</span><span class="sxs-lookup"><span data-stu-id="09885-114">Properties</span></span>

| <span data-ttu-id="09885-115">属性</span><span class="sxs-lookup"><span data-stu-id="09885-115">Property</span></span>     | <span data-ttu-id="09885-116">类型</span><span class="sxs-lookup"><span data-stu-id="09885-116">Type</span></span>        | <span data-ttu-id="09885-117">说明</span><span class="sxs-lookup"><span data-stu-id="09885-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="09885-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="09885-118">authMethods</span></span> | <span data-ttu-id="09885-119">registrationAuthMethod 集合</span><span class="sxs-lookup"><span data-stu-id="09885-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="09885-120">表示用户已注册的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="09885-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="09885-121">可能的值是：、 (仅用于自助服务密码重置) 、和 (仅支持在注册 `email` `mobilePhone` `officePhone` `securityQuestion` `appNotification` `appCode` `alternateMobilePhone`) 。</span><span class="sxs-lookup"><span data-stu-id="09885-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="09885-122">id</span><span class="sxs-lookup"><span data-stu-id="09885-122">id</span></span> | <span data-ttu-id="09885-123">String</span><span class="sxs-lookup"><span data-stu-id="09885-123">String</span></span> | <span data-ttu-id="09885-124">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="09885-124">The unique identifier for the activity.</span></span> <span data-ttu-id="09885-125">只读。</span><span class="sxs-lookup"><span data-stu-id="09885-125">Read-only.</span></span>|
| <span data-ttu-id="09885-126">isCapable</span><span class="sxs-lookup"><span data-stu-id="09885-126">isCapable</span></span> | <span data-ttu-id="09885-127">布尔</span><span class="sxs-lookup"><span data-stu-id="09885-127">Boolean</span></span> | <span data-ttu-id="09885-128">指示用户是否已准备好执行自助服务密码重置或 MFA。</span><span class="sxs-lookup"><span data-stu-id="09885-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="09885-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="09885-129">isEnabled</span></span> | <span data-ttu-id="09885-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="09885-130">Boolean</span></span> | <span data-ttu-id="09885-131">指示用户是否已启用执行自助服务密码重置。</span><span class="sxs-lookup"><span data-stu-id="09885-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="09885-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="09885-132">isMfaRegistered</span></span> | <span data-ttu-id="09885-133">布尔</span><span class="sxs-lookup"><span data-stu-id="09885-133">Boolean</span></span> | <span data-ttu-id="09885-134">指示用户是否已注册 MFA。</span><span class="sxs-lookup"><span data-stu-id="09885-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="09885-135">isRegistered</span><span class="sxs-lookup"><span data-stu-id="09885-135">isRegistered</span></span> | <span data-ttu-id="09885-136">布尔</span><span class="sxs-lookup"><span data-stu-id="09885-136">Boolean</span></span> | <span data-ttu-id="09885-137">指示用户是否已注册任何用于自助密码重置的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="09885-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="09885-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="09885-138">userDisplayName</span></span> | <span data-ttu-id="09885-139">String</span><span class="sxs-lookup"><span data-stu-id="09885-139">String</span></span> | <span data-ttu-id="09885-140">提供相应用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="09885-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="09885-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09885-141">userPrincipalName</span></span> | <span data-ttu-id="09885-142">String</span><span class="sxs-lookup"><span data-stu-id="09885-142">String</span></span> | <span data-ttu-id="09885-143">提供相应用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="09885-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="09885-144">关系</span><span class="sxs-lookup"><span data-stu-id="09885-144">Relationships</span></span>

<span data-ttu-id="09885-145">无。</span><span class="sxs-lookup"><span data-stu-id="09885-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09885-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09885-146">JSON representation</span></span>

<span data-ttu-id="09885-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09885-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


