---
title: credentialUserRegistrationDetails 资源类型
description: 表示对所有注册用户使用自助密码重置和多重身份验证 (MFA) 的详细信息。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: fb852bb20fa8564f81e3dbcb027fced3d630f36b
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598456"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="cbd4a-103">credentialUserRegistrationDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbd4a-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="cbd4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbd4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbd4a-105">表示对所有注册用户使用自助密码重置和多重身份验证 (MFA) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="cbd4a-106">详细信息包括用户信息、注册状态和使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="cbd4a-107">方法</span><span class="sxs-lookup"><span data-stu-id="cbd4a-107">Methods</span></span>

| <span data-ttu-id="cbd4a-108">方法</span><span class="sxs-lookup"><span data-stu-id="cbd4a-108">Method</span></span>       | <span data-ttu-id="cbd4a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cbd4a-109">Return Type</span></span> | <span data-ttu-id="cbd4a-110">说明</span><span class="sxs-lookup"><span data-stu-id="cbd4a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cbd4a-111">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="cbd4a-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="cbd4a-112">credentialUserRegistrationDetails 集合</span><span class="sxs-lookup"><span data-stu-id="cbd4a-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="cbd4a-113">获取给定租户的[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="cbd4a-114">属性</span><span class="sxs-lookup"><span data-stu-id="cbd4a-114">Properties</span></span>

| <span data-ttu-id="cbd4a-115">属性</span><span class="sxs-lookup"><span data-stu-id="cbd4a-115">Property</span></span>     | <span data-ttu-id="cbd4a-116">类型</span><span class="sxs-lookup"><span data-stu-id="cbd4a-116">Type</span></span>        | <span data-ttu-id="cbd4a-117">说明</span><span class="sxs-lookup"><span data-stu-id="cbd4a-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cbd4a-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="cbd4a-118">authMethods</span></span> | <span data-ttu-id="cbd4a-119">registrationAuthMethod 集合</span><span class="sxs-lookup"><span data-stu-id="cbd4a-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="cbd4a-120">表示用户已注册的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="cbd4a-121">可能的值为： `email` 、 `mobilePhone` 、、 `officePhone` `securityQuestion` (仅用于自助密码重置) 、、 `appNotification` `appCode` 和 `alternateMobilePhone` (仅在注册) 中受支持。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="cbd4a-122">id</span><span class="sxs-lookup"><span data-stu-id="cbd4a-122">id</span></span> | <span data-ttu-id="cbd4a-123">String</span><span class="sxs-lookup"><span data-stu-id="cbd4a-123">String</span></span> | <span data-ttu-id="cbd4a-124">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-124">The unique identifier for the activity.</span></span> <span data-ttu-id="cbd4a-125">只读。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-125">Read-only.</span></span>|
| <span data-ttu-id="cbd4a-126">isCapable</span><span class="sxs-lookup"><span data-stu-id="cbd4a-126">isCapable</span></span> | <span data-ttu-id="cbd4a-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="cbd4a-127">Boolean</span></span> | <span data-ttu-id="cbd4a-128">指示用户是否已准备好执行自助密码重置或进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="cbd4a-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cbd4a-129">isEnabled</span></span> | <span data-ttu-id="cbd4a-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbd4a-130">Boolean</span></span> | <span data-ttu-id="cbd4a-131">Indiciates 是否允许用户执行自助密码重置。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="cbd4a-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="cbd4a-132">isMfaRegistered</span></span> | <span data-ttu-id="cbd4a-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="cbd4a-133">Boolean</span></span> | <span data-ttu-id="cbd4a-134">Indiciates 是否为用户注册了 MFA。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="cbd4a-135">isRegistered</span><span class="sxs-lookup"><span data-stu-id="cbd4a-135">isRegistered</span></span> | <span data-ttu-id="cbd4a-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="cbd4a-136">Boolean</span></span> | <span data-ttu-id="cbd4a-137">指示用户是否已将任何身份验证方法注册为自助密码重置。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="cbd4a-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cbd4a-138">userDisplayName</span></span> | <span data-ttu-id="cbd4a-139">String</span><span class="sxs-lookup"><span data-stu-id="cbd4a-139">String</span></span> | <span data-ttu-id="cbd4a-140">提供相应用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="cbd4a-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cbd4a-141">userPrincipalName</span></span> | <span data-ttu-id="cbd4a-142">String</span><span class="sxs-lookup"><span data-stu-id="cbd4a-142">String</span></span> | <span data-ttu-id="cbd4a-143">提供相应用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbd4a-144">关系</span><span class="sxs-lookup"><span data-stu-id="cbd4a-144">Relationships</span></span>

<span data-ttu-id="cbd4a-145">无。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbd4a-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbd4a-146">JSON representation</span></span>

<span data-ttu-id="cbd4a-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbd4a-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "baseType": "",
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
