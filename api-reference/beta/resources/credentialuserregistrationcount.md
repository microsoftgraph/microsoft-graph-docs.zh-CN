---
title: credentialUserRegistrationCount 资源类型
description: 表示您的组织中的多少用户为自助密码重置和多重身份验证功能注册的用户的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: cd08bbcd6a189c2f76c130d28ea749745a5f8fca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507343"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="c7c07-103">credentialUserRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7c07-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="c7c07-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c7c07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7c07-105">表示您的组织中的多少用户为自助密码重置和多重身份验证功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c7c07-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="c7c07-106">方法</span><span class="sxs-lookup"><span data-stu-id="c7c07-106">Methods</span></span>

| <span data-ttu-id="c7c07-107">方法</span><span class="sxs-lookup"><span data-stu-id="c7c07-107">Method</span></span>       | <span data-ttu-id="c7c07-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7c07-108">Return Type</span></span> | <span data-ttu-id="c7c07-109">说明</span><span class="sxs-lookup"><span data-stu-id="c7c07-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c7c07-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="c7c07-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="c7c07-111">credentialUserRegistrationCount 集合</span><span class="sxs-lookup"><span data-stu-id="c7c07-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="c7c07-112">报告您的组织中的多少用户为自助密码重置和多重身份验证（MFA）功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c7c07-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="c7c07-113">属性</span><span class="sxs-lookup"><span data-stu-id="c7c07-113">Properties</span></span>

| <span data-ttu-id="c7c07-114">属性</span><span class="sxs-lookup"><span data-stu-id="c7c07-114">Property</span></span>     | <span data-ttu-id="c7c07-115">类型</span><span class="sxs-lookup"><span data-stu-id="c7c07-115">Type</span></span>        | <span data-ttu-id="c7c07-116">说明</span><span class="sxs-lookup"><span data-stu-id="c7c07-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c7c07-117">id</span><span class="sxs-lookup"><span data-stu-id="c7c07-117">id</span></span> | <span data-ttu-id="c7c07-118">String</span><span class="sxs-lookup"><span data-stu-id="c7c07-118">String</span></span> | <span data-ttu-id="c7c07-119">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c7c07-119">The unique identifier for the activity.</span></span> <span data-ttu-id="c7c07-120">只读。</span><span class="sxs-lookup"><span data-stu-id="c7c07-120">Read-only.</span></span> |
| <span data-ttu-id="c7c07-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="c7c07-121">totalUserCount</span></span> | <span data-ttu-id="c7c07-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c7c07-122">Int64</span></span> | <span data-ttu-id="c7c07-123">提供租户中的总用户计数。</span><span class="sxs-lookup"><span data-stu-id="c7c07-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="c7c07-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="c7c07-124">userRegistrationCounts</span></span> | <span data-ttu-id="c7c07-125">[userRegistrationCount](userregistrationcount.md)集合</span><span class="sxs-lookup"><span data-stu-id="c7c07-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="c7c07-126">租户中用户的注册计数和状态信息的集合。</span><span class="sxs-lookup"><span data-stu-id="c7c07-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7c07-127">关系</span><span class="sxs-lookup"><span data-stu-id="c7c07-127">Relationships</span></span>

<span data-ttu-id="c7c07-128">无。</span><span class="sxs-lookup"><span data-stu-id="c7c07-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7c07-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7c07-129">JSON representation</span></span>

<span data-ttu-id="c7c07-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7c07-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
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