---
title: leakedCredentialsRiskEvent 资源类型
description: Azure Active Directory Identity Protection 检测到的风险事件，其中已检测到帐户的凭据为通配符。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: ac8e9dc0c2adb685513c74658464f4a79af5cb45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442977"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="09165-104">leakedCredentialsRiskEvent 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="09165-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="09165-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09165-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="09165-106">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="09165-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="09165-107">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="09165-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="09165-108">Azure [Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) 检测到的风险事件，其中已对帐户凭据进行通配符检测。</span><span class="sxs-lookup"><span data-stu-id="09165-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="09165-109">有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="09165-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="09165-110">Methods</span><span class="sxs-lookup"><span data-stu-id="09165-110">Methods</span></span>

| <span data-ttu-id="09165-111">方法</span><span class="sxs-lookup"><span data-stu-id="09165-111">Method</span></span>           | <span data-ttu-id="09165-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="09165-112">Return Type</span></span>    |<span data-ttu-id="09165-113">说明</span><span class="sxs-lookup"><span data-stu-id="09165-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09165-114">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="09165-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="09165-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="09165-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="09165-116">读取 leakedCredentialsRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09165-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09165-117">属性</span><span class="sxs-lookup"><span data-stu-id="09165-117">Properties</span></span>
| <span data-ttu-id="09165-118">属性</span><span class="sxs-lookup"><span data-stu-id="09165-118">Property</span></span>     | <span data-ttu-id="09165-119">类型</span><span class="sxs-lookup"><span data-stu-id="09165-119">Type</span></span>   |<span data-ttu-id="09165-120">说明</span><span class="sxs-lookup"><span data-stu-id="09165-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09165-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="09165-121">closedDateTime</span></span>|<span data-ttu-id="09165-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09165-122">dateTimeOffset</span></span>| <span data-ttu-id="09165-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="09165-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="09165-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09165-124">createdDateTime</span></span>|<span data-ttu-id="09165-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09165-125">dateTimeOffset</span></span>| <span data-ttu-id="09165-126">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="09165-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="09165-127">这始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="09165-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="09165-128">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="09165-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="09165-129">id</span><span class="sxs-lookup"><span data-stu-id="09165-129">id</span></span>|<span data-ttu-id="09165-130">string</span><span class="sxs-lookup"><span data-stu-id="09165-130">string</span></span>| <span data-ttu-id="09165-131">只读</span><span class="sxs-lookup"><span data-stu-id="09165-131">Read-only</span></span>|
|<span data-ttu-id="09165-132">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="09165-132">riskEventDateTime</span></span>|<span data-ttu-id="09165-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09165-133">dateTimeOffset</span></span>| <span data-ttu-id="09165-134">发生风险事件的日期和时间</span><span class="sxs-lookup"><span data-stu-id="09165-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="09165-135">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="09165-135">riskEventStatus</span></span>|<span data-ttu-id="09165-136">string</span><span class="sxs-lookup"><span data-stu-id="09165-136">string</span></span>| <span data-ttu-id="09165-137">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="09165-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="09165-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="09165-138">riskLevel</span></span>|<span data-ttu-id="09165-139">string</span><span class="sxs-lookup"><span data-stu-id="09165-139">string</span></span>| <span data-ttu-id="09165-140">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="09165-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="09165-141">riskEventType</span><span class="sxs-lookup"><span data-stu-id="09165-141">riskEventType</span></span>|<span data-ttu-id="09165-142">string</span><span class="sxs-lookup"><span data-stu-id="09165-142">string</span></span>| <span data-ttu-id="09165-143">风险类型</span><span class="sxs-lookup"><span data-stu-id="09165-143">The type of risk</span></span>|
|<span data-ttu-id="09165-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="09165-144">userDisplayName</span></span>|<span data-ttu-id="09165-145">string</span><span class="sxs-lookup"><span data-stu-id="09165-145">string</span></span>| <span data-ttu-id="09165-146">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="09165-146">The name of the user at risk</span></span>|
|<span data-ttu-id="09165-147">userId</span><span class="sxs-lookup"><span data-stu-id="09165-147">userId</span></span>|<span data-ttu-id="09165-148">string</span><span class="sxs-lookup"><span data-stu-id="09165-148">string</span></span>| <span data-ttu-id="09165-149">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="09165-149">The id of the user at risk</span></span>|
|<span data-ttu-id="09165-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09165-150">userPrincipalName</span></span>|<span data-ttu-id="09165-151">string</span><span class="sxs-lookup"><span data-stu-id="09165-151">string</span></span>| <span data-ttu-id="09165-152">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="09165-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="09165-153">关系</span><span class="sxs-lookup"><span data-stu-id="09165-153">Relationships</span></span>
| <span data-ttu-id="09165-154">关系</span><span class="sxs-lookup"><span data-stu-id="09165-154">Relationship</span></span> | <span data-ttu-id="09165-155">类型</span><span class="sxs-lookup"><span data-stu-id="09165-155">Type</span></span>   |<span data-ttu-id="09165-156">说明</span><span class="sxs-lookup"><span data-stu-id="09165-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09165-157">impactedUser</span><span class="sxs-lookup"><span data-stu-id="09165-157">impactedUser</span></span>|[<span data-ttu-id="09165-158">user</span><span class="sxs-lookup"><span data-stu-id="09165-158">user</span></span>](user.md)| <span data-ttu-id="09165-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="09165-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09165-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09165-161">JSON representation</span></span>

<span data-ttu-id="09165-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09165-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
