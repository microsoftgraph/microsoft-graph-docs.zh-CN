---
title: userCredentialUsageDetails 资源类型
description: 表示给定租户的自助服务密码重置使用情况。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3992272aa6917aa43d2ffdb4c4c980b88fc60e7e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159813"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="8d382-103">userCredentialUsageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d382-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="8d382-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d382-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d382-105">表示给定租户的自助服务密码重置使用情况。</span><span class="sxs-lookup"><span data-stu-id="8d382-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="8d382-106">详细信息包括用户信息、重置状态和失败原因。</span><span class="sxs-lookup"><span data-stu-id="8d382-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="8d382-107">方法</span><span class="sxs-lookup"><span data-stu-id="8d382-107">Methods</span></span>

| <span data-ttu-id="8d382-108">方法</span><span class="sxs-lookup"><span data-stu-id="8d382-108">Method</span></span>       | <span data-ttu-id="8d382-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d382-109">Return Type</span></span> | <span data-ttu-id="8d382-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d382-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8d382-111">列出 userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="8d382-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="8d382-112">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="8d382-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="8d382-113">读取 userCredentialUsageDetails 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d382-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d382-114">属性</span><span class="sxs-lookup"><span data-stu-id="8d382-114">Properties</span></span>

| <span data-ttu-id="8d382-115">属性</span><span class="sxs-lookup"><span data-stu-id="8d382-115">Property</span></span>     | <span data-ttu-id="8d382-116">类型</span><span class="sxs-lookup"><span data-stu-id="8d382-116">Type</span></span>        | <span data-ttu-id="8d382-117">说明</span><span class="sxs-lookup"><span data-stu-id="8d382-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8d382-118">authMethod</span><span class="sxs-lookup"><span data-stu-id="8d382-118">authMethod</span></span> | <span data-ttu-id="8d382-119">string</span><span class="sxs-lookup"><span data-stu-id="8d382-119">string</span></span> | <span data-ttu-id="8d382-120">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8d382-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="8d382-121">可能的值是： ， ， ， (仅用于自助服务密码重置) 、 、 和 (`email` `mobileSMS` 仅在注册 `mobileCall` `officePhone` `securityQuestion` `appNotification` `appCode` `alternateMobileCall`) 。</span><span class="sxs-lookup"><span data-stu-id="8d382-121">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="8d382-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8d382-122">eventDateTime</span></span> | <span data-ttu-id="8d382-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d382-123">DateTimeOffset</span></span> | <span data-ttu-id="8d382-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8d382-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d382-125">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8d382-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="8d382-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="8d382-126">failureReason</span></span> | <span data-ttu-id="8d382-127">String</span><span class="sxs-lookup"><span data-stu-id="8d382-127">String</span></span> | <span data-ttu-id="8d382-128">提供相应重置或注册工作流的失败原因。</span><span class="sxs-lookup"><span data-stu-id="8d382-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="8d382-129">功能</span><span class="sxs-lookup"><span data-stu-id="8d382-129">feature</span></span> | <span data-ttu-id="8d382-130">string</span><span class="sxs-lookup"><span data-stu-id="8d382-130">string</span></span> | <span data-ttu-id="8d382-131">可能的值是： `registration` 和 `reset` 。</span><span class="sxs-lookup"><span data-stu-id="8d382-131">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="8d382-132">id</span><span class="sxs-lookup"><span data-stu-id="8d382-132">id</span></span> | <span data-ttu-id="8d382-133">String</span><span class="sxs-lookup"><span data-stu-id="8d382-133">String</span></span> | <span data-ttu-id="8d382-134">只读。</span><span class="sxs-lookup"><span data-stu-id="8d382-134">Read-only.</span></span> <span data-ttu-id="8d382-135">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8d382-135">The unique identifier for the activity.</span></span> <span data-ttu-id="8d382-136">只读。</span><span class="sxs-lookup"><span data-stu-id="8d382-136">Read-only.</span></span>|
| <span data-ttu-id="8d382-137">isSuccess</span><span class="sxs-lookup"><span data-stu-id="8d382-137">isSuccess</span></span> | <span data-ttu-id="8d382-138">布尔</span><span class="sxs-lookup"><span data-stu-id="8d382-138">Boolean</span></span> | <span data-ttu-id="8d382-139">指示工作流是成功还是失败。</span><span class="sxs-lookup"><span data-stu-id="8d382-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="8d382-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d382-140">userDisplayName</span></span> | <span data-ttu-id="8d382-141">String</span><span class="sxs-lookup"><span data-stu-id="8d382-141">String</span></span> | <span data-ttu-id="8d382-142">执行重置或注册工作流的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="8d382-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="8d382-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d382-143">userPrincipalName</span></span> | <span data-ttu-id="8d382-144">String</span><span class="sxs-lookup"><span data-stu-id="8d382-144">String</span></span> | <span data-ttu-id="8d382-145">执行重置或注册工作流的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="8d382-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d382-146">关系</span><span class="sxs-lookup"><span data-stu-id="8d382-146">Relationships</span></span>

<span data-ttu-id="8d382-147">无。</span><span class="sxs-lookup"><span data-stu-id="8d382-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d382-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d382-148">JSON representation</span></span>

<span data-ttu-id="8d382-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d382-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

