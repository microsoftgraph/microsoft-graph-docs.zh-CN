---
title: credentialUsageSummary 资源类型
description: 表示组织中的多少用户使用自助密码重置功能的当前状态。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 736575ba8958a45cad76f7142967c2a629b0732a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458024"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="c32c8-103">credentialUsageSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c32c8-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="c32c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c32c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c32c8-105">表示组织中的多少用户使用自助密码重置功能的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c32c8-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="c32c8-106">方法</span><span class="sxs-lookup"><span data-stu-id="c32c8-106">Methods</span></span>

| <span data-ttu-id="c32c8-107">方法</span><span class="sxs-lookup"><span data-stu-id="c32c8-107">Method</span></span>       | <span data-ttu-id="c32c8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c32c8-108">Return Type</span></span> | <span data-ttu-id="c32c8-109">说明</span><span class="sxs-lookup"><span data-stu-id="c32c8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c32c8-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c32c8-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="c32c8-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="c32c8-111">credentialUsageSummary</span></span> | <span data-ttu-id="c32c8-112">读取 credentialUsageSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c32c8-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c32c8-113">属性</span><span class="sxs-lookup"><span data-stu-id="c32c8-113">Properties</span></span>

| <span data-ttu-id="c32c8-114">属性</span><span class="sxs-lookup"><span data-stu-id="c32c8-114">Property</span></span>     | <span data-ttu-id="c32c8-115">类型</span><span class="sxs-lookup"><span data-stu-id="c32c8-115">Type</span></span>        | <span data-ttu-id="c32c8-116">说明</span><span class="sxs-lookup"><span data-stu-id="c32c8-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c32c8-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="c32c8-117">authMethod</span></span> | <span data-ttu-id="c32c8-118">string</span><span class="sxs-lookup"><span data-stu-id="c32c8-118">string</span></span> | <span data-ttu-id="c32c8-119">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c32c8-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="c32c8-120">可能的值是`email`： `mobileSMS`、 `mobileCall`、 `officePhone`、 `securityQuestion` 、（仅用于自助密码重置）、 `appNotification` `appCode`、和`alternateMobileCall` （仅支持注册）。</span><span class="sxs-lookup"><span data-stu-id="c32c8-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="c32c8-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="c32c8-121">failureActivityCount</span></span> | <span data-ttu-id="c32c8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c32c8-122">Int64</span></span> | <span data-ttu-id="c32c8-123">提供失败重置或注册数据的计数。</span><span class="sxs-lookup"><span data-stu-id="c32c8-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="c32c8-124">功能</span><span class="sxs-lookup"><span data-stu-id="c32c8-124">feature</span></span> | <span data-ttu-id="c32c8-125">string</span><span class="sxs-lookup"><span data-stu-id="c32c8-125">string</span></span> | <span data-ttu-id="c32c8-126">定义要报告的功能。</span><span class="sxs-lookup"><span data-stu-id="c32c8-126">Defines the feature to report.</span></span> <span data-ttu-id="c32c8-127">可能的值为`registration` ： `reset`和。</span><span class="sxs-lookup"><span data-stu-id="c32c8-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="c32c8-128">id</span><span class="sxs-lookup"><span data-stu-id="c32c8-128">id</span></span> | <span data-ttu-id="c32c8-129">String</span><span class="sxs-lookup"><span data-stu-id="c32c8-129">String</span></span> | <span data-ttu-id="c32c8-130">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c32c8-130">The unique identifier for the activity.</span></span> <span data-ttu-id="c32c8-131">只读。</span><span class="sxs-lookup"><span data-stu-id="c32c8-131">Read-only.</span></span> |
| <span data-ttu-id="c32c8-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="c32c8-132">successfulActivityCount</span></span> | <span data-ttu-id="c32c8-133">Int64</span><span class="sxs-lookup"><span data-stu-id="c32c8-133">Int64</span></span> | <span data-ttu-id="c32c8-134">提供成功注册或重置的次数。</span><span class="sxs-lookup"><span data-stu-id="c32c8-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c32c8-135">关系</span><span class="sxs-lookup"><span data-stu-id="c32c8-135">Relationships</span></span>

<span data-ttu-id="c32c8-136">无。</span><span class="sxs-lookup"><span data-stu-id="c32c8-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c32c8-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c32c8-137">JSON representation</span></span>

<span data-ttu-id="c32c8-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c32c8-138">The following is a JSON representation of the resource.</span></span>

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