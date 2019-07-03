---
title: userCredentialUsageDetails 资源类型
description: 表示给定租户的自助服务密码重置用法。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: bb92f3bfc91e8fa418d6a33ad6a77a5fddbf9f10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521313"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="746e5-103">userCredentialUsageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="746e5-103">userCredentialUsageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="746e5-104">表示给定租户的自助服务密码重置用法。</span><span class="sxs-lookup"><span data-stu-id="746e5-104">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="746e5-105">详细信息包括用户信息、重置状态和失败原因。</span><span class="sxs-lookup"><span data-stu-id="746e5-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="746e5-106">方法</span><span class="sxs-lookup"><span data-stu-id="746e5-106">Methods</span></span>

| <span data-ttu-id="746e5-107">方法</span><span class="sxs-lookup"><span data-stu-id="746e5-107">Method</span></span>       | <span data-ttu-id="746e5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="746e5-108">Return Type</span></span> | <span data-ttu-id="746e5-109">说明</span><span class="sxs-lookup"><span data-stu-id="746e5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="746e5-110">列出 userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="746e5-110">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="746e5-111">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="746e5-111">userCredentialUsageDetails</span></span> | <span data-ttu-id="746e5-112">读取 userCredentialUsageDetails 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="746e5-112">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="746e5-113">属性</span><span class="sxs-lookup"><span data-stu-id="746e5-113">Properties</span></span>

| <span data-ttu-id="746e5-114">属性</span><span class="sxs-lookup"><span data-stu-id="746e5-114">Property</span></span>     | <span data-ttu-id="746e5-115">类型</span><span class="sxs-lookup"><span data-stu-id="746e5-115">Type</span></span>        | <span data-ttu-id="746e5-116">说明</span><span class="sxs-lookup"><span data-stu-id="746e5-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="746e5-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="746e5-117">authMethod</span></span> | <span data-ttu-id="746e5-118">string</span><span class="sxs-lookup"><span data-stu-id="746e5-118">string</span></span> | <span data-ttu-id="746e5-119">表示用户使用的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="746e5-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="746e5-120">可能的值是`email`: `mobileSMS`、 `mobileCall`、 `officePhone`、 `securityQuestion` 、(仅用于自助密码重置)、 `appNotification` `appCode`、和`alternateMobileCall` (仅在注册中受支持)。</span><span class="sxs-lookup"><span data-stu-id="746e5-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="746e5-121">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="746e5-121">eventDateTime</span></span> | <span data-ttu-id="746e5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="746e5-122">DateTimeOffset</span></span> | <span data-ttu-id="746e5-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="746e5-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="746e5-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="746e5-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="746e5-125">failureReason</span><span class="sxs-lookup"><span data-stu-id="746e5-125">failureReason</span></span> | <span data-ttu-id="746e5-126">String</span><span class="sxs-lookup"><span data-stu-id="746e5-126">String</span></span> | <span data-ttu-id="746e5-127">提供相应重置或注册工作流的失败原因。</span><span class="sxs-lookup"><span data-stu-id="746e5-127">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="746e5-128">功能</span><span class="sxs-lookup"><span data-stu-id="746e5-128">feature</span></span> | <span data-ttu-id="746e5-129">string</span><span class="sxs-lookup"><span data-stu-id="746e5-129">string</span></span> | <span data-ttu-id="746e5-130">可能的值为`registration` : `reset`和。</span><span class="sxs-lookup"><span data-stu-id="746e5-130">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="746e5-131">id</span><span class="sxs-lookup"><span data-stu-id="746e5-131">id</span></span> | <span data-ttu-id="746e5-132">String</span><span class="sxs-lookup"><span data-stu-id="746e5-132">String</span></span> | <span data-ttu-id="746e5-133">只读。</span><span class="sxs-lookup"><span data-stu-id="746e5-133">Read-only.</span></span> <span data-ttu-id="746e5-134">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="746e5-134">The unique identifier for the activity.</span></span> <span data-ttu-id="746e5-135">只读。</span><span class="sxs-lookup"><span data-stu-id="746e5-135">Read-only.</span></span>|
| <span data-ttu-id="746e5-136">isSuccess</span><span class="sxs-lookup"><span data-stu-id="746e5-136">isSuccess</span></span> | <span data-ttu-id="746e5-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="746e5-137">Boolean</span></span> | <span data-ttu-id="746e5-138">指示工作流是成功还是失败。</span><span class="sxs-lookup"><span data-stu-id="746e5-138">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="746e5-139">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="746e5-139">userDisplayName</span></span> | <span data-ttu-id="746e5-140">String</span><span class="sxs-lookup"><span data-stu-id="746e5-140">String</span></span> | <span data-ttu-id="746e5-141">执行重置或注册工作流的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="746e5-141">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="746e5-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="746e5-142">userPrincipalName</span></span> | <span data-ttu-id="746e5-143">字符串</span><span class="sxs-lookup"><span data-stu-id="746e5-143">String</span></span> | <span data-ttu-id="746e5-144">执行重置或注册工作流的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="746e5-144">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="746e5-145">关系</span><span class="sxs-lookup"><span data-stu-id="746e5-145">Relationships</span></span>

<span data-ttu-id="746e5-146">无。</span><span class="sxs-lookup"><span data-stu-id="746e5-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="746e5-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="746e5-147">JSON representation</span></span>

<span data-ttu-id="746e5-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="746e5-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
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