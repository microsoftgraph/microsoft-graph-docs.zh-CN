---
title: identityRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件。 它是每个特定风险事件类型的基本类型：
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 47b8b7590be2d4b235bb04fe079b58cf65cb4ae7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866789"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="58d0e-104">identityRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="58d0e-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="58d0e-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="58d0e-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="58d0e-106">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="58d0e-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="58d0e-107">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="58d0e-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="58d0e-108">它是每个特定风险事件类型的基本类型：</span><span class="sxs-lookup"><span data-stu-id="58d0e-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="58d0e-109">事件类型</span><span class="sxs-lookup"><span data-stu-id="58d0e-109">Event type</span></span>         | <span data-ttu-id="58d0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="58d0e-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="58d0e-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="58d0e-112">来自匿名 IP 地址的登录。</span><span class="sxs-lookup"><span data-stu-id="58d0e-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="58d0e-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="58d0e-114">来自恶意软件感染的设备的登录。</span><span class="sxs-lookup"><span data-stu-id="58d0e-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="58d0e-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="58d0e-116">无法传播到非典型位置。</span><span class="sxs-lookup"><span data-stu-id="58d0e-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="58d0e-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="58d0e-118">凭据泄露的用户。</span><span class="sxs-lookup"><span data-stu-id="58d0e-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="58d0e-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="58d0e-120">来自可疑 IP 地址的登录。</span><span class="sxs-lookup"><span data-stu-id="58d0e-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="58d0e-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="58d0e-122">来自不熟悉位置的登录。</span><span class="sxs-lookup"><span data-stu-id="58d0e-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="58d0e-123">有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](/azure/active-directory/active-directory-reporting-risk-events)。</span><span class="sxs-lookup"><span data-stu-id="58d0e-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="58d0e-124">方法</span><span class="sxs-lookup"><span data-stu-id="58d0e-124">Methods</span></span>

| <span data-ttu-id="58d0e-125">方法</span><span class="sxs-lookup"><span data-stu-id="58d0e-125">Method</span></span>           | <span data-ttu-id="58d0e-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="58d0e-126">Return Type</span></span>    |<span data-ttu-id="58d0e-127">说明</span><span class="sxs-lookup"><span data-stu-id="58d0e-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58d0e-128">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="58d0e-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58d0e-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="58d0e-130">读取 identityRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58d0e-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58d0e-131">属性</span><span class="sxs-lookup"><span data-stu-id="58d0e-131">Properties</span></span>
| <span data-ttu-id="58d0e-132">属性</span><span class="sxs-lookup"><span data-stu-id="58d0e-132">Property</span></span>     | <span data-ttu-id="58d0e-133">类型</span><span class="sxs-lookup"><span data-stu-id="58d0e-133">Type</span></span>   |<span data-ttu-id="58d0e-134">说明</span><span class="sxs-lookup"><span data-stu-id="58d0e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58d0e-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="58d0e-135">closedDateTime</span></span>|<span data-ttu-id="58d0e-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58d0e-136">dateTimeOffset</span></span>| <span data-ttu-id="58d0e-137">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="58d0e-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="58d0e-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58d0e-138">createdDateTime</span></span>|<span data-ttu-id="58d0e-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58d0e-139">dateTimeOffset</span></span>| <span data-ttu-id="58d0e-140">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="58d0e-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="58d0e-141">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="58d0e-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="58d0e-142">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="58d0e-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="58d0e-143">id</span><span class="sxs-lookup"><span data-stu-id="58d0e-143">id</span></span>|<span data-ttu-id="58d0e-144">字符串</span><span class="sxs-lookup"><span data-stu-id="58d0e-144">string</span></span>| <span data-ttu-id="58d0e-145">只读</span><span class="sxs-lookup"><span data-stu-id="58d0e-145">Read-only</span></span>|
|<span data-ttu-id="58d0e-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="58d0e-146">riskEventDateTime</span></span>|<span data-ttu-id="58d0e-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58d0e-147">dateTimeOffset</span></span>| <span data-ttu-id="58d0e-148">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="58d0e-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="58d0e-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="58d0e-149">riskEventStatus</span></span>|<span data-ttu-id="58d0e-150">string</span><span class="sxs-lookup"><span data-stu-id="58d0e-150">string</span></span>| <span data-ttu-id="58d0e-151">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="58d0e-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="58d0e-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="58d0e-152">riskLevel</span></span>|<span data-ttu-id="58d0e-153">string</span><span class="sxs-lookup"><span data-stu-id="58d0e-153">string</span></span>| <span data-ttu-id="58d0e-154">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="58d0e-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="58d0e-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="58d0e-155">riskEventType</span></span>|<span data-ttu-id="58d0e-156">string</span><span class="sxs-lookup"><span data-stu-id="58d0e-156">string</span></span>| <span data-ttu-id="58d0e-157">风险的类型</span><span class="sxs-lookup"><span data-stu-id="58d0e-157">The type of risk</span></span>|
|<span data-ttu-id="58d0e-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="58d0e-158">userDisplayName</span></span>|<span data-ttu-id="58d0e-159">string</span><span class="sxs-lookup"><span data-stu-id="58d0e-159">string</span></span>| <span data-ttu-id="58d0e-160">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="58d0e-160">The name of the user at risk</span></span>|
|<span data-ttu-id="58d0e-161">userId</span><span class="sxs-lookup"><span data-stu-id="58d0e-161">userId</span></span>|<span data-ttu-id="58d0e-162">string</span><span class="sxs-lookup"><span data-stu-id="58d0e-162">string</span></span>| <span data-ttu-id="58d0e-163">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="58d0e-163">The id of the user at risk</span></span>|
|<span data-ttu-id="58d0e-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58d0e-164">userPrincipalName</span></span>|<span data-ttu-id="58d0e-165">string</span><span class="sxs-lookup"><span data-stu-id="58d0e-165">string</span></span>| <span data-ttu-id="58d0e-166">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="58d0e-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="58d0e-167">关系</span><span class="sxs-lookup"><span data-stu-id="58d0e-167">Relationships</span></span>
| <span data-ttu-id="58d0e-168">关系</span><span class="sxs-lookup"><span data-stu-id="58d0e-168">Relationship</span></span> | <span data-ttu-id="58d0e-169">类型</span><span class="sxs-lookup"><span data-stu-id="58d0e-169">Type</span></span>   |<span data-ttu-id="58d0e-170">说明</span><span class="sxs-lookup"><span data-stu-id="58d0e-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58d0e-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="58d0e-171">impactedUser</span></span>|[<span data-ttu-id="58d0e-172">user</span><span class="sxs-lookup"><span data-stu-id="58d0e-172">user</span></span>](user.md)| <span data-ttu-id="58d0e-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="58d0e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58d0e-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58d0e-175">JSON representation</span></span>

<span data-ttu-id="58d0e-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58d0e-176">Here is a JSON representation of the resource.</span></span>

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
