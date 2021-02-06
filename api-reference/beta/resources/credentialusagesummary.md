---
title: credentialUsageSummary 资源类型
description: 表示组织中使用自助服务密码重置功能的用户数的当前状态。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 43a17f91a1424d9ac8c0a388ef5404bbadf05189
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136281"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="a1445-103">credentialUsageSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1445-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="a1445-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1445-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1445-105">表示组织中使用自助服务密码重置功能的用户数的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a1445-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="a1445-106">方法</span><span class="sxs-lookup"><span data-stu-id="a1445-106">Methods</span></span>

| <span data-ttu-id="a1445-107">方法</span><span class="sxs-lookup"><span data-stu-id="a1445-107">Method</span></span>       | <span data-ttu-id="a1445-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1445-108">Return Type</span></span> | <span data-ttu-id="a1445-109">说明</span><span class="sxs-lookup"><span data-stu-id="a1445-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a1445-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="a1445-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="a1445-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="a1445-111">credentialUsageSummary</span></span> | <span data-ttu-id="a1445-112">读取 credentialUsageSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1445-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a1445-113">属性</span><span class="sxs-lookup"><span data-stu-id="a1445-113">Properties</span></span>

| <span data-ttu-id="a1445-114">属性</span><span class="sxs-lookup"><span data-stu-id="a1445-114">Property</span></span>     | <span data-ttu-id="a1445-115">类型</span><span class="sxs-lookup"><span data-stu-id="a1445-115">Type</span></span>        | <span data-ttu-id="a1445-116">说明</span><span class="sxs-lookup"><span data-stu-id="a1445-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a1445-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="a1445-117">authMethod</span></span> | <span data-ttu-id="a1445-118">string</span><span class="sxs-lookup"><span data-stu-id="a1445-118">string</span></span> | <span data-ttu-id="a1445-119">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a1445-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="a1445-120">可能的值是： ， ， ， (仅用于自助服务密码重置) 、 、 和 (仅 `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` `appNotification` `appCode`  `alternateMobileCall` 支持注册) 。</span><span class="sxs-lookup"><span data-stu-id="a1445-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="a1445-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="a1445-121">failureActivityCount</span></span> | <span data-ttu-id="a1445-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a1445-122">Int64</span></span> | <span data-ttu-id="a1445-123">提供失败的重置或注册数据计数。</span><span class="sxs-lookup"><span data-stu-id="a1445-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="a1445-124">功能</span><span class="sxs-lookup"><span data-stu-id="a1445-124">feature</span></span> | <span data-ttu-id="a1445-125">string</span><span class="sxs-lookup"><span data-stu-id="a1445-125">string</span></span> | <span data-ttu-id="a1445-126">定义要报告的功能。</span><span class="sxs-lookup"><span data-stu-id="a1445-126">Defines the feature to report.</span></span> <span data-ttu-id="a1445-127">可能的值是： `registration` 和 `reset` 。</span><span class="sxs-lookup"><span data-stu-id="a1445-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="a1445-128">id</span><span class="sxs-lookup"><span data-stu-id="a1445-128">id</span></span> | <span data-ttu-id="a1445-129">字符串</span><span class="sxs-lookup"><span data-stu-id="a1445-129">String</span></span> | <span data-ttu-id="a1445-130">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a1445-130">The unique identifier for the activity.</span></span> <span data-ttu-id="a1445-131">只读。</span><span class="sxs-lookup"><span data-stu-id="a1445-131">Read-only.</span></span> |
| <span data-ttu-id="a1445-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="a1445-132">successfulActivityCount</span></span> | <span data-ttu-id="a1445-133">Int64</span><span class="sxs-lookup"><span data-stu-id="a1445-133">Int64</span></span> | <span data-ttu-id="a1445-134">提供成功注册或重置的计数。</span><span class="sxs-lookup"><span data-stu-id="a1445-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a1445-135">关系</span><span class="sxs-lookup"><span data-stu-id="a1445-135">Relationships</span></span>

<span data-ttu-id="a1445-136">无。</span><span class="sxs-lookup"><span data-stu-id="a1445-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1445-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1445-137">JSON representation</span></span>

<span data-ttu-id="a1445-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1445-138">The following is a JSON representation of the resource.</span></span>

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

