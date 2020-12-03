---
title: credentialUsageSummary 资源类型
description: 表示组织中的多少用户使用自助密码重置功能的当前状态。
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9807e333fd13443462d2d3237150820afd254baa
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523145"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="1634b-103">credentialUsageSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1634b-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="1634b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1634b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1634b-105">表示组织中的多少用户使用自助密码重置功能的当前状态。</span><span class="sxs-lookup"><span data-stu-id="1634b-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="1634b-106">方法</span><span class="sxs-lookup"><span data-stu-id="1634b-106">Methods</span></span>

| <span data-ttu-id="1634b-107">方法</span><span class="sxs-lookup"><span data-stu-id="1634b-107">Method</span></span>       | <span data-ttu-id="1634b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1634b-108">Return Type</span></span> | <span data-ttu-id="1634b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1634b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1634b-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="1634b-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="1634b-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="1634b-111">credentialUsageSummary</span></span> | <span data-ttu-id="1634b-112">读取 credentialUsageSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1634b-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1634b-113">属性</span><span class="sxs-lookup"><span data-stu-id="1634b-113">Properties</span></span>

| <span data-ttu-id="1634b-114">属性</span><span class="sxs-lookup"><span data-stu-id="1634b-114">Property</span></span>     | <span data-ttu-id="1634b-115">类型</span><span class="sxs-lookup"><span data-stu-id="1634b-115">Type</span></span>        | <span data-ttu-id="1634b-116">说明</span><span class="sxs-lookup"><span data-stu-id="1634b-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1634b-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="1634b-117">authMethod</span></span> | <span data-ttu-id="1634b-118">string</span><span class="sxs-lookup"><span data-stu-id="1634b-118">string</span></span> | <span data-ttu-id="1634b-119">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="1634b-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="1634b-120">可能的值为： `email` 、、、、 `mobileSMS` `mobileCall` `officePhone` `securityQuestion` (仅用于自助密码重置) 、、 `appNotification` `appCode` 和  `alternateMobileCall` (仅支持注册) 。</span><span class="sxs-lookup"><span data-stu-id="1634b-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="1634b-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="1634b-121">failureActivityCount</span></span> | <span data-ttu-id="1634b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1634b-122">Int64</span></span> | <span data-ttu-id="1634b-123">提供失败重置或注册数据的计数。</span><span class="sxs-lookup"><span data-stu-id="1634b-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="1634b-124">功能</span><span class="sxs-lookup"><span data-stu-id="1634b-124">feature</span></span> | <span data-ttu-id="1634b-125">string</span><span class="sxs-lookup"><span data-stu-id="1634b-125">string</span></span> | <span data-ttu-id="1634b-126">定义要报告的功能。</span><span class="sxs-lookup"><span data-stu-id="1634b-126">Defines the feature to report.</span></span> <span data-ttu-id="1634b-127">可能的值为： `registration` 和 `reset` 。</span><span class="sxs-lookup"><span data-stu-id="1634b-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="1634b-128">id</span><span class="sxs-lookup"><span data-stu-id="1634b-128">id</span></span> | <span data-ttu-id="1634b-129">String</span><span class="sxs-lookup"><span data-stu-id="1634b-129">String</span></span> | <span data-ttu-id="1634b-130">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1634b-130">The unique identifier for the activity.</span></span> <span data-ttu-id="1634b-131">只读。</span><span class="sxs-lookup"><span data-stu-id="1634b-131">Read-only.</span></span> |
| <span data-ttu-id="1634b-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="1634b-132">successfulActivityCount</span></span> | <span data-ttu-id="1634b-133">Int64</span><span class="sxs-lookup"><span data-stu-id="1634b-133">Int64</span></span> | <span data-ttu-id="1634b-134">提供成功注册或重置的次数。</span><span class="sxs-lookup"><span data-stu-id="1634b-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1634b-135">关系</span><span class="sxs-lookup"><span data-stu-id="1634b-135">Relationships</span></span>

<span data-ttu-id="1634b-136">无。</span><span class="sxs-lookup"><span data-stu-id="1634b-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1634b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1634b-137">JSON representation</span></span>

<span data-ttu-id="1634b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1634b-138">The following is a JSON representation of the resource.</span></span>

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

