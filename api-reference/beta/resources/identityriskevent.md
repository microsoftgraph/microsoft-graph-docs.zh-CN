---
title: identityRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件。 它是每个特定风险事件类型的基本类型：
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa8fef43c462559d5c4420637b635b5371ef90ab
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181727"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="44899-104">identityRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="44899-104">identityRiskEvent resource type</span></span>

<span data-ttu-id="44899-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44899-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="44899-106">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="44899-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="44899-107">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="44899-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="44899-108">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="44899-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="44899-109">它是每个特定风险事件类型的基本类型：</span><span class="sxs-lookup"><span data-stu-id="44899-109">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="44899-110">事件类型</span><span class="sxs-lookup"><span data-stu-id="44899-110">Event type</span></span>         | <span data-ttu-id="44899-111">说明</span><span class="sxs-lookup"><span data-stu-id="44899-111">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="44899-112">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-112">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="44899-113">来自匿名 IP 地址的登录。</span><span class="sxs-lookup"><span data-stu-id="44899-113">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="44899-114">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-114">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="44899-115">来自恶意软件感染的设备的登录。</span><span class="sxs-lookup"><span data-stu-id="44899-115">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="44899-116">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-116">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="44899-117">无法传播到非典型位置。</span><span class="sxs-lookup"><span data-stu-id="44899-117">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="44899-118">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-118">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="44899-119">凭据泄露的用户。</span><span class="sxs-lookup"><span data-stu-id="44899-119">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="44899-120">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-120">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="44899-121">来自可疑 IP 地址的登录。</span><span class="sxs-lookup"><span data-stu-id="44899-121">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="44899-122">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-122">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="44899-123">来自不熟悉位置的登录。</span><span class="sxs-lookup"><span data-stu-id="44899-123">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="44899-124">有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](/azure/active-directory/active-directory-reporting-risk-events)。</span><span class="sxs-lookup"><span data-stu-id="44899-124">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="44899-125">方法</span><span class="sxs-lookup"><span data-stu-id="44899-125">Methods</span></span>

| <span data-ttu-id="44899-126">方法</span><span class="sxs-lookup"><span data-stu-id="44899-126">Method</span></span>           | <span data-ttu-id="44899-127">返回类型</span><span class="sxs-lookup"><span data-stu-id="44899-127">Return Type</span></span>    |<span data-ttu-id="44899-128">说明</span><span class="sxs-lookup"><span data-stu-id="44899-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44899-129">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-129">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="44899-130">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44899-130">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="44899-131">读取 identityRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44899-131">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44899-132">属性</span><span class="sxs-lookup"><span data-stu-id="44899-132">Properties</span></span>
| <span data-ttu-id="44899-133">属性</span><span class="sxs-lookup"><span data-stu-id="44899-133">Property</span></span>     | <span data-ttu-id="44899-134">类型</span><span class="sxs-lookup"><span data-stu-id="44899-134">Type</span></span>   |<span data-ttu-id="44899-135">说明</span><span class="sxs-lookup"><span data-stu-id="44899-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44899-136">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="44899-136">closedDateTime</span></span>|<span data-ttu-id="44899-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44899-137">dateTimeOffset</span></span>| <span data-ttu-id="44899-138">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="44899-138">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="44899-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44899-139">createdDateTime</span></span>|<span data-ttu-id="44899-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44899-140">dateTimeOffset</span></span>| <span data-ttu-id="44899-141">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="44899-141">The date and time that the risk event was created.</span></span> <span data-ttu-id="44899-142">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="44899-142">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="44899-143">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="44899-143">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="44899-144">id</span><span class="sxs-lookup"><span data-stu-id="44899-144">id</span></span>|<span data-ttu-id="44899-145">字符串</span><span class="sxs-lookup"><span data-stu-id="44899-145">string</span></span>| <span data-ttu-id="44899-146">只读</span><span class="sxs-lookup"><span data-stu-id="44899-146">Read-only</span></span>|
|<span data-ttu-id="44899-147">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="44899-147">riskEventDateTime</span></span>|<span data-ttu-id="44899-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44899-148">dateTimeOffset</span></span>| <span data-ttu-id="44899-149">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="44899-149">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="44899-150">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="44899-150">riskEventStatus</span></span>|<span data-ttu-id="44899-151">string</span><span class="sxs-lookup"><span data-stu-id="44899-151">string</span></span>| <span data-ttu-id="44899-152">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="44899-152">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="44899-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="44899-153">riskLevel</span></span>|<span data-ttu-id="44899-154">string</span><span class="sxs-lookup"><span data-stu-id="44899-154">string</span></span>| <span data-ttu-id="44899-155">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="44899-155">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="44899-156">riskEventType</span><span class="sxs-lookup"><span data-stu-id="44899-156">riskEventType</span></span>|<span data-ttu-id="44899-157">string</span><span class="sxs-lookup"><span data-stu-id="44899-157">string</span></span>| <span data-ttu-id="44899-158">风险的类型</span><span class="sxs-lookup"><span data-stu-id="44899-158">The type of risk</span></span>|
|<span data-ttu-id="44899-159">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="44899-159">userDisplayName</span></span>|<span data-ttu-id="44899-160">string</span><span class="sxs-lookup"><span data-stu-id="44899-160">string</span></span>| <span data-ttu-id="44899-161">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="44899-161">The name of the user at risk</span></span>|
|<span data-ttu-id="44899-162">userId</span><span class="sxs-lookup"><span data-stu-id="44899-162">userId</span></span>|<span data-ttu-id="44899-163">string</span><span class="sxs-lookup"><span data-stu-id="44899-163">string</span></span>| <span data-ttu-id="44899-164">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="44899-164">The id of the user at risk</span></span>|
|<span data-ttu-id="44899-165">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44899-165">userPrincipalName</span></span>|<span data-ttu-id="44899-166">string</span><span class="sxs-lookup"><span data-stu-id="44899-166">string</span></span>| <span data-ttu-id="44899-167">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="44899-167">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="44899-168">关系</span><span class="sxs-lookup"><span data-stu-id="44899-168">Relationships</span></span>
| <span data-ttu-id="44899-169">关系</span><span class="sxs-lookup"><span data-stu-id="44899-169">Relationship</span></span> | <span data-ttu-id="44899-170">类型</span><span class="sxs-lookup"><span data-stu-id="44899-170">Type</span></span>   |<span data-ttu-id="44899-171">说明</span><span class="sxs-lookup"><span data-stu-id="44899-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44899-172">impactedUser</span><span class="sxs-lookup"><span data-stu-id="44899-172">impactedUser</span></span>|[<span data-ttu-id="44899-173">user</span><span class="sxs-lookup"><span data-stu-id="44899-173">user</span></span>](user.md)| <span data-ttu-id="44899-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="44899-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44899-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44899-176">JSON representation</span></span>

<span data-ttu-id="44899-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44899-177">Here is a JSON representation of the resource.</span></span>

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
