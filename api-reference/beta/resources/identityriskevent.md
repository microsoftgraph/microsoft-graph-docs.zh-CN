---
title: identityRiskEvent 资源类型
description: Azure Active Directory Identity Protection 检测到的风险事件。 它是每个特定风险事件类型的基类型：
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: acb48ce5ef63abf5ec2a09d8a3365a744bb8a668
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440288"
---
# <a name="identityriskevent-resource-type-deprecated"></a><span data-ttu-id="c7f76-104">identityRiskEvent 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="c7f76-104">identityRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="c7f76-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7f76-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="c7f76-106">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="c7f76-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="c7f76-107">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="c7f76-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="c7f76-108">Azure [Active Directory Identity Protection 检测到的风险事件](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="c7f76-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span> <span data-ttu-id="c7f76-109">它是每个特定风险事件类型的基类型：</span><span class="sxs-lookup"><span data-stu-id="c7f76-109">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="c7f76-110">事件类型</span><span class="sxs-lookup"><span data-stu-id="c7f76-110">Event type</span></span>         | <span data-ttu-id="c7f76-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7f76-111">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="c7f76-112">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-112">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="c7f76-113">从匿名 IP 地址登录。</span><span class="sxs-lookup"><span data-stu-id="c7f76-113">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="c7f76-114">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-114">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="c7f76-115">从受恶意软件感染的设备登录。</span><span class="sxs-lookup"><span data-stu-id="c7f76-115">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="c7f76-116">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-116">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="c7f76-117">无法到达非典型位置。</span><span class="sxs-lookup"><span data-stu-id="c7f76-117">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="c7f76-118">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-118">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="c7f76-119">凭据泄露的用户。</span><span class="sxs-lookup"><span data-stu-id="c7f76-119">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="c7f76-120">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-120">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="c7f76-121">从可疑 IP 地址登录。</span><span class="sxs-lookup"><span data-stu-id="c7f76-121">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="c7f76-122">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-122">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="c7f76-123">从不熟悉的位置登录。</span><span class="sxs-lookup"><span data-stu-id="c7f76-123">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="c7f76-124">有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/active-directory-reporting-risk-events)。</span><span class="sxs-lookup"><span data-stu-id="c7f76-124">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="c7f76-125">Methods</span><span class="sxs-lookup"><span data-stu-id="c7f76-125">Methods</span></span>

| <span data-ttu-id="c7f76-126">方法</span><span class="sxs-lookup"><span data-stu-id="c7f76-126">Method</span></span>           | <span data-ttu-id="c7f76-127">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7f76-127">Return Type</span></span>    |<span data-ttu-id="c7f76-128">说明</span><span class="sxs-lookup"><span data-stu-id="c7f76-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7f76-129">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-129">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="c7f76-130">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c7f76-130">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="c7f76-131">读取 identityRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7f76-131">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7f76-132">属性</span><span class="sxs-lookup"><span data-stu-id="c7f76-132">Properties</span></span>
| <span data-ttu-id="c7f76-133">属性</span><span class="sxs-lookup"><span data-stu-id="c7f76-133">Property</span></span>     | <span data-ttu-id="c7f76-134">类型</span><span class="sxs-lookup"><span data-stu-id="c7f76-134">Type</span></span>   |<span data-ttu-id="c7f76-135">说明</span><span class="sxs-lookup"><span data-stu-id="c7f76-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7f76-136">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f76-136">closedDateTime</span></span>|<span data-ttu-id="c7f76-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f76-137">dateTimeOffset</span></span>| <span data-ttu-id="c7f76-138">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c7f76-138">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c7f76-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f76-139">createdDateTime</span></span>|<span data-ttu-id="c7f76-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f76-140">dateTimeOffset</span></span>| <span data-ttu-id="c7f76-141">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c7f76-141">The date and time that the risk event was created.</span></span> <span data-ttu-id="c7f76-142">这始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c7f76-142">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c7f76-143">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="c7f76-143">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c7f76-144">id</span><span class="sxs-lookup"><span data-stu-id="c7f76-144">id</span></span>|<span data-ttu-id="c7f76-145">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-145">string</span></span>| <span data-ttu-id="c7f76-146">只读</span><span class="sxs-lookup"><span data-stu-id="c7f76-146">Read-only</span></span>|
|<span data-ttu-id="c7f76-147">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f76-147">riskEventDateTime</span></span>|<span data-ttu-id="c7f76-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f76-148">dateTimeOffset</span></span>| <span data-ttu-id="c7f76-149">发生风险事件的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c7f76-149">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c7f76-150">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c7f76-150">riskEventStatus</span></span>|<span data-ttu-id="c7f76-151">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-151">string</span></span>| <span data-ttu-id="c7f76-152">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="c7f76-152">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c7f76-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c7f76-153">riskLevel</span></span>|<span data-ttu-id="c7f76-154">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-154">string</span></span>| <span data-ttu-id="c7f76-155">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c7f76-155">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c7f76-156">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c7f76-156">riskEventType</span></span>|<span data-ttu-id="c7f76-157">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-157">string</span></span>| <span data-ttu-id="c7f76-158">风险类型</span><span class="sxs-lookup"><span data-stu-id="c7f76-158">The type of risk</span></span>|
|<span data-ttu-id="c7f76-159">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7f76-159">userDisplayName</span></span>|<span data-ttu-id="c7f76-160">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-160">string</span></span>| <span data-ttu-id="c7f76-161">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="c7f76-161">The name of the user at risk</span></span>|
|<span data-ttu-id="c7f76-162">userId</span><span class="sxs-lookup"><span data-stu-id="c7f76-162">userId</span></span>|<span data-ttu-id="c7f76-163">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-163">string</span></span>| <span data-ttu-id="c7f76-164">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="c7f76-164">The id of the user at risk</span></span>|
|<span data-ttu-id="c7f76-165">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7f76-165">userPrincipalName</span></span>|<span data-ttu-id="c7f76-166">string</span><span class="sxs-lookup"><span data-stu-id="c7f76-166">string</span></span>| <span data-ttu-id="c7f76-167">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c7f76-167">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7f76-168">关系</span><span class="sxs-lookup"><span data-stu-id="c7f76-168">Relationships</span></span>
| <span data-ttu-id="c7f76-169">关系</span><span class="sxs-lookup"><span data-stu-id="c7f76-169">Relationship</span></span> | <span data-ttu-id="c7f76-170">类型</span><span class="sxs-lookup"><span data-stu-id="c7f76-170">Type</span></span>   |<span data-ttu-id="c7f76-171">说明</span><span class="sxs-lookup"><span data-stu-id="c7f76-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7f76-172">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c7f76-172">impactedUser</span></span>|[<span data-ttu-id="c7f76-173">user</span><span class="sxs-lookup"><span data-stu-id="c7f76-173">user</span></span>](user.md)| <span data-ttu-id="c7f76-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="c7f76-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7f76-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7f76-176">JSON representation</span></span>

<span data-ttu-id="c7f76-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7f76-177">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
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
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
