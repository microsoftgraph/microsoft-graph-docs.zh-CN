---
title: credentialUsageSummary 资源类型
description: 表示组织中的多少用户使用自助密码重置功能的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 17fc4535e5132b6bf6c2f6eab4a94b5a58ef9bb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507350"
---
# <a name="credentialusagesummary-resource-type"></a><span data-ttu-id="83c79-103">credentialUsageSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="83c79-103">credentialUsageSummary resource type</span></span>

<span data-ttu-id="83c79-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="83c79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83c79-105">表示组织中的多少用户使用自助密码重置功能的当前状态。</span><span class="sxs-lookup"><span data-stu-id="83c79-105">Represents the current state of how many users in your organization are using self-service password reset capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="83c79-106">方法</span><span class="sxs-lookup"><span data-stu-id="83c79-106">Methods</span></span>

| <span data-ttu-id="83c79-107">方法</span><span class="sxs-lookup"><span data-stu-id="83c79-107">Method</span></span>       | <span data-ttu-id="83c79-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="83c79-108">Return Type</span></span> | <span data-ttu-id="83c79-109">说明</span><span class="sxs-lookup"><span data-stu-id="83c79-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="83c79-110">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="83c79-110">getCredentialUsageSummary</span></span>](../api/reportroot-getcredentialusagesummary.md) | <span data-ttu-id="83c79-111">credentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="83c79-111">credentialUsageSummary</span></span> | <span data-ttu-id="83c79-112">读取 credentialUsageSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83c79-112">Read properties and relationships of a credentialUsageSummary object.</span></span> |

## <a name="properties"></a><span data-ttu-id="83c79-113">属性</span><span class="sxs-lookup"><span data-stu-id="83c79-113">Properties</span></span>

| <span data-ttu-id="83c79-114">属性</span><span class="sxs-lookup"><span data-stu-id="83c79-114">Property</span></span>     | <span data-ttu-id="83c79-115">类型</span><span class="sxs-lookup"><span data-stu-id="83c79-115">Type</span></span>        | <span data-ttu-id="83c79-116">说明</span><span class="sxs-lookup"><span data-stu-id="83c79-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="83c79-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="83c79-117">authMethod</span></span> | <span data-ttu-id="83c79-118">string</span><span class="sxs-lookup"><span data-stu-id="83c79-118">string</span></span> | <span data-ttu-id="83c79-119">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="83c79-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="83c79-120">可能的值是`email`： `mobileSMS`、 `mobileCall`、 `officePhone`、 `securityQuestion` 、（仅用于自助密码重置）、 `appNotification` `appCode`、和`alternateMobileCall` （仅支持注册）。</span><span class="sxs-lookup"><span data-stu-id="83c79-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and  `alternateMobileCall` (only supported for registration).</span></span> |
| <span data-ttu-id="83c79-121">failureActivityCount</span><span class="sxs-lookup"><span data-stu-id="83c79-121">failureActivityCount</span></span> | <span data-ttu-id="83c79-122">Int64</span><span class="sxs-lookup"><span data-stu-id="83c79-122">Int64</span></span> | <span data-ttu-id="83c79-123">提供失败重置或注册数据的计数。</span><span class="sxs-lookup"><span data-stu-id="83c79-123">Provides the count of failed resets or registration data.</span></span> |
| <span data-ttu-id="83c79-124">功能</span><span class="sxs-lookup"><span data-stu-id="83c79-124">feature</span></span> | <span data-ttu-id="83c79-125">string</span><span class="sxs-lookup"><span data-stu-id="83c79-125">string</span></span> | <span data-ttu-id="83c79-126">定义要报告的功能。</span><span class="sxs-lookup"><span data-stu-id="83c79-126">Defines the feature to report.</span></span> <span data-ttu-id="83c79-127">可能的值为`registration` ： `reset`和。</span><span class="sxs-lookup"><span data-stu-id="83c79-127">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="83c79-128">id</span><span class="sxs-lookup"><span data-stu-id="83c79-128">id</span></span> | <span data-ttu-id="83c79-129">String</span><span class="sxs-lookup"><span data-stu-id="83c79-129">String</span></span> | <span data-ttu-id="83c79-130">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="83c79-130">The unique identifier for the activity.</span></span> <span data-ttu-id="83c79-131">只读。</span><span class="sxs-lookup"><span data-stu-id="83c79-131">Read-only.</span></span> |
| <span data-ttu-id="83c79-132">successfulActivityCount</span><span class="sxs-lookup"><span data-stu-id="83c79-132">successfulActivityCount</span></span> | <span data-ttu-id="83c79-133">Int64</span><span class="sxs-lookup"><span data-stu-id="83c79-133">Int64</span></span> | <span data-ttu-id="83c79-134">提供成功注册或重置的次数。</span><span class="sxs-lookup"><span data-stu-id="83c79-134">Provides the count of successful registrations or resets.</span></span> |

## <a name="relationships"></a><span data-ttu-id="83c79-135">关系</span><span class="sxs-lookup"><span data-stu-id="83c79-135">Relationships</span></span>

<span data-ttu-id="83c79-136">无。</span><span class="sxs-lookup"><span data-stu-id="83c79-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83c79-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83c79-137">JSON representation</span></span>

<span data-ttu-id="83c79-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83c79-138">The following is a JSON representation of the resource.</span></span>

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