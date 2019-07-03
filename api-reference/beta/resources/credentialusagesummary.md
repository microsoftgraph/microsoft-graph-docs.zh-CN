---
title: credentialUsageSummary 资源类型
description: 表示组织中的多少用户使用自助密码重置功能的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 46fc3f90b7a7f286d61a324e7b5f439d467a4978
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520768"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="c6b01-103">credentialUsageSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6b01-103">credentialUsageSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6b01-104">表示组织中的多少用户使用自助密码重置功能的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c6b01-104">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="c6b01-105">方法</span><span class="sxs-lookup"><span data-stu-id="c6b01-105">Methods</span></span>

| <span data-ttu-id="c6b01-106">方法</span><span class="sxs-lookup"><span data-stu-id="c6b01-106">Method</span></span>       | <span data-ttu-id="c6b01-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6b01-107">Return Type</span></span> | <span data-ttu-id="c6b01-108">说明</span><span class="sxs-lookup"><span data-stu-id="c6b01-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c6b01-109">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c6b01-109">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="c6b01-110">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c6b01-110">credentialUsageSummary</span></span> | <span data-ttu-id="c6b01-111">读取 credentialUsageSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6b01-111">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6b01-112">属性</span><span class="sxs-lookup"><span data-stu-id="c6b01-112">Properties</span></span>

| <span data-ttu-id="c6b01-113">属性</span><span class="sxs-lookup"><span data-stu-id="c6b01-113">Property</span></span>     | <span data-ttu-id="c6b01-114">类型</span><span class="sxs-lookup"><span data-stu-id="c6b01-114">Type</span></span>        | <span data-ttu-id="c6b01-115">说明</span><span class="sxs-lookup"><span data-stu-id="c6b01-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c6b01-116">authMethod</span><span class="sxs-lookup"><span data-stu-id="c6b01-116">authMethod</span></span> | <span data-ttu-id="c6b01-117">string</span><span class="sxs-lookup"><span data-stu-id="c6b01-117">string</span></span> | <span data-ttu-id="c6b01-118">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c6b01-118">Represents the authentication method that the user used.</span></span> <span data-ttu-id="c6b01-119">可能的值是`email`: `mobileSMS`、 `mobileCall`、 `officePhone`、 `securityQuestion` 、(仅用于自助密码重置)、 `appNotification` `appCode`、和`alternateMobileCall` (仅支持注册)。</span><span class="sxs-lookup"><span data-stu-id="c6b01-119">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="c6b01-120">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="c6b01-120">failureActivityCount</span></span> | <span data-ttu-id="c6b01-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c6b01-121">Int64</span></span> | <span data-ttu-id="c6b01-122">提供失败重置或注册数据的计数。</span><span class="sxs-lookup"><span data-stu-id="c6b01-122">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="c6b01-123">功能</span><span class="sxs-lookup"><span data-stu-id="c6b01-123">feature</span></span> | <span data-ttu-id="c6b01-124">string</span><span class="sxs-lookup"><span data-stu-id="c6b01-124">string</span></span> | <span data-ttu-id="c6b01-125">定义要报告的功能。</span><span class="sxs-lookup"><span data-stu-id="c6b01-125">Defines the feature to report.</span></span> <span data-ttu-id="c6b01-126">可能的值为`registration` : `reset`和。</span><span class="sxs-lookup"><span data-stu-id="c6b01-126">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="c6b01-127">id</span><span class="sxs-lookup"><span data-stu-id="c6b01-127">id</span></span> | <span data-ttu-id="c6b01-128">String</span><span class="sxs-lookup"><span data-stu-id="c6b01-128">String</span></span> | <span data-ttu-id="c6b01-129">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c6b01-129">The unique identifier for the activity.</span></span> <span data-ttu-id="c6b01-130">只读。</span><span class="sxs-lookup"><span data-stu-id="c6b01-130">Read-only.</span></span> |
| <span data-ttu-id="c6b01-131">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="c6b01-131">successfulActivityCount</span></span> | <span data-ttu-id="c6b01-132">Int64</span><span class="sxs-lookup"><span data-stu-id="c6b01-132">Int64</span></span> | <span data-ttu-id="c6b01-133">提供成功注册或重置的次数。</span><span class="sxs-lookup"><span data-stu-id="c6b01-133">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c6b01-134">关系</span><span class="sxs-lookup"><span data-stu-id="c6b01-134">Relationships</span></span>

<span data-ttu-id="c6b01-135">无。</span><span class="sxs-lookup"><span data-stu-id="c6b01-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6b01-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6b01-136">JSON representation</span></span>

<span data-ttu-id="c6b01-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6b01-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->