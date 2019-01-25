---
title: identityRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护风险事件。 它是为每个特定的风险事件类型的基类型：
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514178"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="c6ad0-104">identityRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6ad0-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6ad0-105">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)风险事件。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="c6ad0-106">它是为每个特定的风险事件类型的基类型：</span><span class="sxs-lookup"><span data-stu-id="c6ad0-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="c6ad0-107">事件类型</span><span class="sxs-lookup"><span data-stu-id="c6ad0-107">Event type</span></span>         | <span data-ttu-id="c6ad0-108">说明</span><span class="sxs-lookup"><span data-stu-id="c6ad0-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="c6ad0-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="c6ad0-110">从匿名登录 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="c6ad0-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="c6ad0-112">登录从感染恶意软件的设备。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="c6ad0-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="c6ad0-114">对在典型的位置的意思出差。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="c6ad0-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="c6ad0-116">具有泄漏凭据的用户。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="c6ad0-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="c6ad0-118">登录从可疑 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="c6ad0-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="c6ad0-120">登录从不熟悉的位置。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="c6ad0-121">[Azure AD 身份保护文档](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="c6ad0-122">方法</span><span class="sxs-lookup"><span data-stu-id="c6ad0-122">Methods</span></span>

| <span data-ttu-id="c6ad0-123">方法</span><span class="sxs-lookup"><span data-stu-id="c6ad0-123">Method</span></span>           | <span data-ttu-id="c6ad0-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6ad0-124">Return Type</span></span>    |<span data-ttu-id="c6ad0-125">说明</span><span class="sxs-lookup"><span data-stu-id="c6ad0-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6ad0-126">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="c6ad0-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c6ad0-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="c6ad0-128">读取属性和 identityRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6ad0-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6ad0-129">Properties</span></span>
| <span data-ttu-id="c6ad0-130">属性</span><span class="sxs-lookup"><span data-stu-id="c6ad0-130">Property</span></span>     | <span data-ttu-id="c6ad0-131">类型</span><span class="sxs-lookup"><span data-stu-id="c6ad0-131">Type</span></span>   |<span data-ttu-id="c6ad0-132">说明</span><span class="sxs-lookup"><span data-stu-id="c6ad0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ad0-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ad0-133">closedDateTime</span></span>|<span data-ttu-id="c6ad0-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ad0-134">dateTimeOffset</span></span>| <span data-ttu-id="c6ad0-135">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="c6ad0-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c6ad0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ad0-136">createdDateTime</span></span>|<span data-ttu-id="c6ad0-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ad0-137">dateTimeOffset</span></span>| <span data-ttu-id="c6ad0-138">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="c6ad0-139">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c6ad0-140">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c6ad0-141">id</span><span class="sxs-lookup"><span data-stu-id="c6ad0-141">id</span></span>|<span data-ttu-id="c6ad0-142">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-142">string</span></span>| <span data-ttu-id="c6ad0-143">只读</span><span class="sxs-lookup"><span data-stu-id="c6ad0-143">Read-only</span></span>|
|<span data-ttu-id="c6ad0-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ad0-144">riskEventDateTime</span></span>|<span data-ttu-id="c6ad0-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ad0-145">dateTimeOffset</span></span>| <span data-ttu-id="c6ad0-146">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="c6ad0-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c6ad0-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c6ad0-147">riskEventStatus</span></span>|<span data-ttu-id="c6ad0-148">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-148">string</span></span>| <span data-ttu-id="c6ad0-149">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c6ad0-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c6ad0-150">riskLevel</span></span>|<span data-ttu-id="c6ad0-151">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-151">string</span></span>| <span data-ttu-id="c6ad0-152">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c6ad0-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c6ad0-153">riskEventType</span></span>|<span data-ttu-id="c6ad0-154">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-154">string</span></span>| <span data-ttu-id="c6ad0-155">风险类型</span><span class="sxs-lookup"><span data-stu-id="c6ad0-155">The type of risk</span></span>|
|<span data-ttu-id="c6ad0-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6ad0-156">userDisplayName</span></span>|<span data-ttu-id="c6ad0-157">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-157">string</span></span>| <span data-ttu-id="c6ad0-158">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="c6ad0-158">The name of the user at risk</span></span>|
|<span data-ttu-id="c6ad0-159">userId</span><span class="sxs-lookup"><span data-stu-id="c6ad0-159">userId</span></span>|<span data-ttu-id="c6ad0-160">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-160">string</span></span>| <span data-ttu-id="c6ad0-161">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="c6ad0-161">The id of the user at risk</span></span>|
|<span data-ttu-id="c6ad0-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6ad0-162">userPrincipalName</span></span>|<span data-ttu-id="c6ad0-163">string</span><span class="sxs-lookup"><span data-stu-id="c6ad0-163">string</span></span>| <span data-ttu-id="c6ad0-164">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c6ad0-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ad0-165">关系</span><span class="sxs-lookup"><span data-stu-id="c6ad0-165">Relationships</span></span>
| <span data-ttu-id="c6ad0-166">关系</span><span class="sxs-lookup"><span data-stu-id="c6ad0-166">Relationship</span></span> | <span data-ttu-id="c6ad0-167">类型</span><span class="sxs-lookup"><span data-stu-id="c6ad0-167">Type</span></span>   |<span data-ttu-id="c6ad0-168">说明</span><span class="sxs-lookup"><span data-stu-id="c6ad0-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6ad0-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c6ad0-169">impactedUser</span></span>|[<span data-ttu-id="c6ad0-170">user</span><span class="sxs-lookup"><span data-stu-id="c6ad0-170">user</span></span>](user.md)| <span data-ttu-id="c6ad0-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6ad0-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6ad0-173">JSON representation</span></span>

<span data-ttu-id="c6ad0-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6ad0-174">Here is a JSON representation of the resource.</span></span> 

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
