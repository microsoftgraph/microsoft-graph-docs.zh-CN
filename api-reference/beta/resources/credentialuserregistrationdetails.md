---
title: credentialUserRegistrationDetails 资源类型
description: 表示对所有注册用户使用自助密码重置和多重身份验证 (MFA) 的详细信息。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 414cd6977f4e3c15ab7b82bd88329e9e3549f137
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520767"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="dfd45-103">credentialUserRegistrationDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfd45-103">credentialUserRegistrationDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfd45-104">表示对所有注册用户使用自助密码重置和多重身份验证 (MFA) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dfd45-104">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="dfd45-105">详细信息包括用户信息、注册状态和使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="dfd45-105">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="dfd45-106">方法</span><span class="sxs-lookup"><span data-stu-id="dfd45-106">Methods</span></span>

| <span data-ttu-id="dfd45-107">方法</span><span class="sxs-lookup"><span data-stu-id="dfd45-107">Method</span></span>       | <span data-ttu-id="dfd45-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfd45-108">Return Type</span></span> | <span data-ttu-id="dfd45-109">说明</span><span class="sxs-lookup"><span data-stu-id="dfd45-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dfd45-110">列出 credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="dfd45-110">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="dfd45-111">credentialUserRegistrationDetails 集合</span><span class="sxs-lookup"><span data-stu-id="dfd45-111">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="dfd45-112">获取给定租户的[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="dfd45-112">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="dfd45-113">属性</span><span class="sxs-lookup"><span data-stu-id="dfd45-113">Properties</span></span>

| <span data-ttu-id="dfd45-114">属性</span><span class="sxs-lookup"><span data-stu-id="dfd45-114">Property</span></span>     | <span data-ttu-id="dfd45-115">类型</span><span class="sxs-lookup"><span data-stu-id="dfd45-115">Type</span></span>        | <span data-ttu-id="dfd45-116">说明</span><span class="sxs-lookup"><span data-stu-id="dfd45-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dfd45-117">authMethods</span><span class="sxs-lookup"><span data-stu-id="dfd45-117">authMethods</span></span> | <span data-ttu-id="dfd45-118">registrationAuthMethod 集合</span><span class="sxs-lookup"><span data-stu-id="dfd45-118">registrationAuthMethod collection</span></span> | <span data-ttu-id="dfd45-119">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="dfd45-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="dfd45-120">可能的值为`email`: `mobilePhone`、 `officePhone`、 `securityQuestion` 、(仅用于自助密码重置)、 `appNotification` `appCode`、和`alternateMobilePhone` (仅在注册中受支持)。</span><span class="sxs-lookup"><span data-stu-id="dfd45-120">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="dfd45-121">id</span><span class="sxs-lookup"><span data-stu-id="dfd45-121">id</span></span> | <span data-ttu-id="dfd45-122">String</span><span class="sxs-lookup"><span data-stu-id="dfd45-122">String</span></span> | <span data-ttu-id="dfd45-123">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dfd45-123">The unique identifier for the activity.</span></span> <span data-ttu-id="dfd45-124">只读。</span><span class="sxs-lookup"><span data-stu-id="dfd45-124">Read-only.</span></span>|
| <span data-ttu-id="dfd45-125">isCapable</span><span class="sxs-lookup"><span data-stu-id="dfd45-125">isCapable</span></span> | <span data-ttu-id="dfd45-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfd45-126">Boolean</span></span> | <span data-ttu-id="dfd45-127">指示用户是否已准备好执行自助密码重置或进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="dfd45-127">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="dfd45-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="dfd45-128">isEnabled</span></span> | <span data-ttu-id="dfd45-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfd45-129">Boolean</span></span> | <span data-ttu-id="dfd45-130">Indiciates 是否允许用户执行自助密码重置。</span><span class="sxs-lookup"><span data-stu-id="dfd45-130">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="dfd45-131">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="dfd45-131">isMfaRegistered</span></span> | <span data-ttu-id="dfd45-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfd45-132">Boolean</span></span> | <span data-ttu-id="dfd45-133">Indiciates 是否为用户注册了 MFA。</span><span class="sxs-lookup"><span data-stu-id="dfd45-133">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="dfd45-134">isRegistered</span><span class="sxs-lookup"><span data-stu-id="dfd45-134">isRegistered</span></span> | <span data-ttu-id="dfd45-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfd45-135">Boolean</span></span> | <span data-ttu-id="dfd45-136">指示用户是否已将任何身份验证方法注册为自助密码重置。</span><span class="sxs-lookup"><span data-stu-id="dfd45-136">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="dfd45-137">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dfd45-137">userDisplayName</span></span> | <span data-ttu-id="dfd45-138">String</span><span class="sxs-lookup"><span data-stu-id="dfd45-138">String</span></span> | <span data-ttu-id="dfd45-139">提供相应用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="dfd45-139">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="dfd45-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dfd45-140">userPrincipalName</span></span> | <span data-ttu-id="dfd45-141">字符串</span><span class="sxs-lookup"><span data-stu-id="dfd45-141">String</span></span> | <span data-ttu-id="dfd45-142">提供相应用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="dfd45-142">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dfd45-143">关系</span><span class="sxs-lookup"><span data-stu-id="dfd45-143">Relationships</span></span>

<span data-ttu-id="dfd45-144">无。</span><span class="sxs-lookup"><span data-stu-id="dfd45-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfd45-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfd45-145">JSON representation</span></span>

<span data-ttu-id="dfd45-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfd45-146">The following is a JSON representation of the resource.</span></span>

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