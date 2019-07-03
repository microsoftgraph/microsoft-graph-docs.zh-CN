---
title: credentialUserRegistrationCount 资源类型
description: 表示您的组织中的多少用户为自助密码重置和多重身份验证功能注册的用户的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 42c722b04493767d3dbcaf713157d931569d8c32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478239"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="ce8ca-103">credentialUserRegistrationCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce8ca-103">credentialUserRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce8ca-104">表示您的组织中的多少用户为自助密码重置和多重身份验证功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-104">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="ce8ca-105">方法</span><span class="sxs-lookup"><span data-stu-id="ce8ca-105">Methods</span></span>

| <span data-ttu-id="ce8ca-106">方法</span><span class="sxs-lookup"><span data-stu-id="ce8ca-106">Method</span></span>       | <span data-ttu-id="ce8ca-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ce8ca-107">Return Type</span></span> | <span data-ttu-id="ce8ca-108">说明</span><span class="sxs-lookup"><span data-stu-id="ce8ca-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ce8ca-109">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="ce8ca-109">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="ce8ca-110">credentialUserRegistrationCount 集合</span><span class="sxs-lookup"><span data-stu-id="ce8ca-110">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="ce8ca-111">报告您的组织中的多少用户为自助密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-111">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce8ca-112">属性</span><span class="sxs-lookup"><span data-stu-id="ce8ca-112">Properties</span></span>

| <span data-ttu-id="ce8ca-113">属性</span><span class="sxs-lookup"><span data-stu-id="ce8ca-113">Property</span></span>     | <span data-ttu-id="ce8ca-114">类型</span><span class="sxs-lookup"><span data-stu-id="ce8ca-114">Type</span></span>        | <span data-ttu-id="ce8ca-115">说明</span><span class="sxs-lookup"><span data-stu-id="ce8ca-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ce8ca-116">id</span><span class="sxs-lookup"><span data-stu-id="ce8ca-116">id</span></span> | <span data-ttu-id="ce8ca-117">String</span><span class="sxs-lookup"><span data-stu-id="ce8ca-117">String</span></span> | <span data-ttu-id="ce8ca-118">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-118">The unique identifier for the activity.</span></span> <span data-ttu-id="ce8ca-119">只读。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-119">Read-only.</span></span> |
| <span data-ttu-id="ce8ca-120">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="ce8ca-120">totalUserCount</span></span> | <span data-ttu-id="ce8ca-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ce8ca-121">Int64</span></span> | <span data-ttu-id="ce8ca-122">提供租户中的总用户计数。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-122">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="ce8ca-123">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="ce8ca-123">userRegistrationCounts</span></span> | <span data-ttu-id="ce8ca-124">[userRegistrationCount](userregistrationcount.md)集合</span><span class="sxs-lookup"><span data-stu-id="ce8ca-124">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="ce8ca-125">租户中用户的注册计数和状态信息的集合。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-125">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ce8ca-126">关系</span><span class="sxs-lookup"><span data-stu-id="ce8ca-126">Relationships</span></span>

<span data-ttu-id="ce8ca-127">无。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce8ca-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce8ca-128">JSON representation</span></span>

<span data-ttu-id="ce8ca-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce8ca-129">The following is a JSON representation of the resource.</span></span>

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