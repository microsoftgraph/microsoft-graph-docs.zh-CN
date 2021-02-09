---
title: credentialUserRegistrationCount 资源类型
description: 表示组织中注册自助密码重置和多重身份验证功能的用户数的当前状态。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 521c8eca7c3233000bf04f2324e8990fd25c55f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159918"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="9fc3a-103">credentialUserRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fc3a-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="9fc3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fc3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc3a-105">表示组织中注册自助密码重置和多重身份验证功能的用户数的当前状态。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="9fc3a-106">方法</span><span class="sxs-lookup"><span data-stu-id="9fc3a-106">Methods</span></span>

| <span data-ttu-id="9fc3a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9fc3a-107">Method</span></span>       | <span data-ttu-id="9fc3a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9fc3a-108">Return Type</span></span> | <span data-ttu-id="9fc3a-109">说明</span><span class="sxs-lookup"><span data-stu-id="9fc3a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9fc3a-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="9fc3a-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="9fc3a-111">credentialUserRegistrationCount 集合</span><span class="sxs-lookup"><span data-stu-id="9fc3a-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="9fc3a-112">报告组织中有多少用户注册了自助服务密码重置和多重身份验证的当前状态， (MFA) 功能。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fc3a-113">属性</span><span class="sxs-lookup"><span data-stu-id="9fc3a-113">Properties</span></span>

| <span data-ttu-id="9fc3a-114">属性</span><span class="sxs-lookup"><span data-stu-id="9fc3a-114">Property</span></span>     | <span data-ttu-id="9fc3a-115">类型</span><span class="sxs-lookup"><span data-stu-id="9fc3a-115">Type</span></span>        | <span data-ttu-id="9fc3a-116">说明</span><span class="sxs-lookup"><span data-stu-id="9fc3a-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9fc3a-117">id</span><span class="sxs-lookup"><span data-stu-id="9fc3a-117">id</span></span> | <span data-ttu-id="9fc3a-118">String</span><span class="sxs-lookup"><span data-stu-id="9fc3a-118">String</span></span> | <span data-ttu-id="9fc3a-119">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-119">The unique identifier for the activity.</span></span> <span data-ttu-id="9fc3a-120">只读。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-120">Read-only.</span></span> |
| <span data-ttu-id="9fc3a-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="9fc3a-121">totalUserCount</span></span> | <span data-ttu-id="9fc3a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9fc3a-122">Int64</span></span> | <span data-ttu-id="9fc3a-123">提供租户中的用户总数。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="9fc3a-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="9fc3a-124">userRegistrationCounts</span></span> | <span data-ttu-id="9fc3a-125">[userRegistrationCount](userregistrationcount.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fc3a-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="9fc3a-126">租户中用户的注册计数和状态信息的集合。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9fc3a-127">关系</span><span class="sxs-lookup"><span data-stu-id="9fc3a-127">Relationships</span></span>

<span data-ttu-id="9fc3a-128">无。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fc3a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fc3a-129">JSON representation</span></span>

<span data-ttu-id="9fc3a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fc3a-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

