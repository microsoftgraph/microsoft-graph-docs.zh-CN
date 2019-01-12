---
title: identityRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护风险事件。 它是为每个特定的风险事件类型的基类型：
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: be5e4afaa5bf85581c904ed94f07433243651ee9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953645"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="a4802-104">identityRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4802-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="a4802-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4802-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4802-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4802-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4802-107">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)风险事件。</span><span class="sxs-lookup"><span data-stu-id="a4802-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="a4802-108">它是为每个特定的风险事件类型的基类型：</span><span class="sxs-lookup"><span data-stu-id="a4802-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="a4802-109">事件类型</span><span class="sxs-lookup"><span data-stu-id="a4802-109">Event type</span></span>         | <span data-ttu-id="a4802-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4802-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="a4802-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="a4802-112">从匿名登录 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="a4802-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="a4802-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="a4802-114">登录从感染恶意软件的设备。</span><span class="sxs-lookup"><span data-stu-id="a4802-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="a4802-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="a4802-116">对在典型的位置的意思出差。</span><span class="sxs-lookup"><span data-stu-id="a4802-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="a4802-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="a4802-118">具有泄漏凭据的用户。</span><span class="sxs-lookup"><span data-stu-id="a4802-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="a4802-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="a4802-120">登录从可疑 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="a4802-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="a4802-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="a4802-122">登录从不熟悉的位置。</span><span class="sxs-lookup"><span data-stu-id="a4802-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="a4802-123">[Azure AD 身份保护文档](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="a4802-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="a4802-124">方法</span><span class="sxs-lookup"><span data-stu-id="a4802-124">Methods</span></span>

| <span data-ttu-id="a4802-125">方法</span><span class="sxs-lookup"><span data-stu-id="a4802-125">Method</span></span>           | <span data-ttu-id="a4802-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4802-126">Return Type</span></span>    |<span data-ttu-id="a4802-127">说明</span><span class="sxs-lookup"><span data-stu-id="a4802-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4802-128">获取 identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="a4802-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="a4802-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="a4802-130">读取属性和 identityRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a4802-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4802-131">属性</span><span class="sxs-lookup"><span data-stu-id="a4802-131">Properties</span></span>
| <span data-ttu-id="a4802-132">属性</span><span class="sxs-lookup"><span data-stu-id="a4802-132">Property</span></span>     | <span data-ttu-id="a4802-133">类型</span><span class="sxs-lookup"><span data-stu-id="a4802-133">Type</span></span>   |<span data-ttu-id="a4802-134">说明</span><span class="sxs-lookup"><span data-stu-id="a4802-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4802-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4802-135">closedDateTime</span></span>|<span data-ttu-id="a4802-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4802-136">dateTimeOffset</span></span>| <span data-ttu-id="a4802-137">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="a4802-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="a4802-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4802-138">createdDateTime</span></span>|<span data-ttu-id="a4802-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4802-139">dateTimeOffset</span></span>| <span data-ttu-id="a4802-140">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="a4802-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="a4802-141">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="a4802-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="a4802-142">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="a4802-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="a4802-143">id</span><span class="sxs-lookup"><span data-stu-id="a4802-143">id</span></span>|<span data-ttu-id="a4802-144">string</span><span class="sxs-lookup"><span data-stu-id="a4802-144">string</span></span>| <span data-ttu-id="a4802-145">只读</span><span class="sxs-lookup"><span data-stu-id="a4802-145">Read-only</span></span>|
|<span data-ttu-id="a4802-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="a4802-146">riskEventDateTime</span></span>|<span data-ttu-id="a4802-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4802-147">dateTimeOffset</span></span>| <span data-ttu-id="a4802-148">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="a4802-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="a4802-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="a4802-149">riskEventStatus</span></span>|<span data-ttu-id="a4802-150">string</span><span class="sxs-lookup"><span data-stu-id="a4802-150">string</span></span>| <span data-ttu-id="a4802-151">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="a4802-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="a4802-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="a4802-152">riskLevel</span></span>|<span data-ttu-id="a4802-153">string</span><span class="sxs-lookup"><span data-stu-id="a4802-153">string</span></span>| <span data-ttu-id="a4802-154">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="a4802-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="a4802-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="a4802-155">riskEventType</span></span>|<span data-ttu-id="a4802-156">string</span><span class="sxs-lookup"><span data-stu-id="a4802-156">string</span></span>| <span data-ttu-id="a4802-157">风险类型</span><span class="sxs-lookup"><span data-stu-id="a4802-157">The type of risk</span></span>|
|<span data-ttu-id="a4802-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a4802-158">userDisplayName</span></span>|<span data-ttu-id="a4802-159">string</span><span class="sxs-lookup"><span data-stu-id="a4802-159">string</span></span>| <span data-ttu-id="a4802-160">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="a4802-160">The name of the user at risk</span></span>|
|<span data-ttu-id="a4802-161">userId</span><span class="sxs-lookup"><span data-stu-id="a4802-161">userId</span></span>|<span data-ttu-id="a4802-162">string</span><span class="sxs-lookup"><span data-stu-id="a4802-162">string</span></span>| <span data-ttu-id="a4802-163">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="a4802-163">The id of the user at risk</span></span>|
|<span data-ttu-id="a4802-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4802-164">userPrincipalName</span></span>|<span data-ttu-id="a4802-165">string</span><span class="sxs-lookup"><span data-stu-id="a4802-165">string</span></span>| <span data-ttu-id="a4802-166">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a4802-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4802-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="a4802-167">Relationships</span></span>
| <span data-ttu-id="a4802-168">关系</span><span class="sxs-lookup"><span data-stu-id="a4802-168">Relationship</span></span> | <span data-ttu-id="a4802-169">类型</span><span class="sxs-lookup"><span data-stu-id="a4802-169">Type</span></span>   |<span data-ttu-id="a4802-170">说明</span><span class="sxs-lookup"><span data-stu-id="a4802-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4802-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="a4802-171">impactedUser</span></span>|[<span data-ttu-id="a4802-172">用户</span><span class="sxs-lookup"><span data-stu-id="a4802-172">user</span></span>](user.md)| <span data-ttu-id="a4802-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a4802-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4802-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4802-175">JSON representation</span></span>

<span data-ttu-id="a4802-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4802-176">Here is a JSON representation of the resource.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
