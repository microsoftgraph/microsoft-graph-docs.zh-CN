---
title: identityRiskEvent 资源类型
description: 'Azure Active Directory 标识保护检测到的风险事件。 它是每个特定风险事件类型的基本类型:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506389"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="c286d-104">identityRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c286d-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c286d-105">[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="c286d-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="c286d-106">它是每个特定风险事件类型的基本类型:</span><span class="sxs-lookup"><span data-stu-id="c286d-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="c286d-107">事件类型</span><span class="sxs-lookup"><span data-stu-id="c286d-107">Event type</span></span>         | <span data-ttu-id="c286d-108">说明</span><span class="sxs-lookup"><span data-stu-id="c286d-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="c286d-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="c286d-110">来自匿名 IP 地址的登录。</span><span class="sxs-lookup"><span data-stu-id="c286d-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="c286d-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="c286d-112">来自恶意软件感染的设备的登录。</span><span class="sxs-lookup"><span data-stu-id="c286d-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="c286d-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="c286d-114">无法传播到非典型位置。</span><span class="sxs-lookup"><span data-stu-id="c286d-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="c286d-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="c286d-116">凭据泄露的用户。</span><span class="sxs-lookup"><span data-stu-id="c286d-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="c286d-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="c286d-118">来自可疑 IP 地址的登录。</span><span class="sxs-lookup"><span data-stu-id="c286d-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="c286d-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="c286d-120">来自不熟悉位置的登录。</span><span class="sxs-lookup"><span data-stu-id="c286d-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="c286d-121">有关风险事件的完整信息, 请参阅[Azure AD Identity Protection 文档](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)。</span><span class="sxs-lookup"><span data-stu-id="c286d-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="c286d-122">方法</span><span class="sxs-lookup"><span data-stu-id="c286d-122">Methods</span></span>

| <span data-ttu-id="c286d-123">方法</span><span class="sxs-lookup"><span data-stu-id="c286d-123">Method</span></span>           | <span data-ttu-id="c286d-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="c286d-124">Return Type</span></span>    |<span data-ttu-id="c286d-125">说明</span><span class="sxs-lookup"><span data-stu-id="c286d-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c286d-126">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="c286d-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c286d-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="c286d-128">读取 identityRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c286d-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c286d-129">属性</span><span class="sxs-lookup"><span data-stu-id="c286d-129">Properties</span></span>
| <span data-ttu-id="c286d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c286d-130">Property</span></span>     | <span data-ttu-id="c286d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c286d-131">Type</span></span>   |<span data-ttu-id="c286d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c286d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c286d-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c286d-133">closedDateTime</span></span>|<span data-ttu-id="c286d-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c286d-134">dateTimeOffset</span></span>| <span data-ttu-id="c286d-135">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c286d-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c286d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c286d-136">createdDateTime</span></span>|<span data-ttu-id="c286d-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c286d-137">dateTimeOffset</span></span>| <span data-ttu-id="c286d-138">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c286d-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="c286d-139">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c286d-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c286d-140">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="c286d-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c286d-141">id</span><span class="sxs-lookup"><span data-stu-id="c286d-141">id</span></span>|<span data-ttu-id="c286d-142">string</span><span class="sxs-lookup"><span data-stu-id="c286d-142">string</span></span>| <span data-ttu-id="c286d-143">只读</span><span class="sxs-lookup"><span data-stu-id="c286d-143">Read-only</span></span>|
|<span data-ttu-id="c286d-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c286d-144">riskEventDateTime</span></span>|<span data-ttu-id="c286d-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c286d-145">dateTimeOffset</span></span>| <span data-ttu-id="c286d-146">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c286d-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c286d-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c286d-147">riskEventStatus</span></span>|<span data-ttu-id="c286d-148">字符串</span><span class="sxs-lookup"><span data-stu-id="c286d-148">string</span></span>| <span data-ttu-id="c286d-149">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="c286d-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c286d-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c286d-150">riskLevel</span></span>|<span data-ttu-id="c286d-151">string</span><span class="sxs-lookup"><span data-stu-id="c286d-151">string</span></span>| <span data-ttu-id="c286d-152">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c286d-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c286d-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c286d-153">riskEventType</span></span>|<span data-ttu-id="c286d-154">字符串</span><span class="sxs-lookup"><span data-stu-id="c286d-154">string</span></span>| <span data-ttu-id="c286d-155">风险的类型</span><span class="sxs-lookup"><span data-stu-id="c286d-155">The type of risk</span></span>|
|<span data-ttu-id="c286d-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c286d-156">userDisplayName</span></span>|<span data-ttu-id="c286d-157">字符串</span><span class="sxs-lookup"><span data-stu-id="c286d-157">string</span></span>| <span data-ttu-id="c286d-158">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="c286d-158">The name of the user at risk</span></span>|
|<span data-ttu-id="c286d-159">userId</span><span class="sxs-lookup"><span data-stu-id="c286d-159">userId</span></span>|<span data-ttu-id="c286d-160">字符串</span><span class="sxs-lookup"><span data-stu-id="c286d-160">string</span></span>| <span data-ttu-id="c286d-161">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="c286d-161">The id of the user at risk</span></span>|
|<span data-ttu-id="c286d-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c286d-162">userPrincipalName</span></span>|<span data-ttu-id="c286d-163">字符串</span><span class="sxs-lookup"><span data-stu-id="c286d-163">string</span></span>| <span data-ttu-id="c286d-164">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c286d-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c286d-165">关系</span><span class="sxs-lookup"><span data-stu-id="c286d-165">Relationships</span></span>
| <span data-ttu-id="c286d-166">关系</span><span class="sxs-lookup"><span data-stu-id="c286d-166">Relationship</span></span> | <span data-ttu-id="c286d-167">类型</span><span class="sxs-lookup"><span data-stu-id="c286d-167">Type</span></span>   |<span data-ttu-id="c286d-168">说明</span><span class="sxs-lookup"><span data-stu-id="c286d-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c286d-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c286d-169">impactedUser</span></span>|[<span data-ttu-id="c286d-170">用户</span><span class="sxs-lookup"><span data-stu-id="c286d-170">user</span></span>](user.md)| <span data-ttu-id="c286d-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="c286d-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c286d-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c286d-173">JSON representation</span></span>

<span data-ttu-id="c286d-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c286d-174">Here is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
