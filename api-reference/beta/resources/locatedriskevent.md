---
title: locatedRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护基于位置数据的风险事件。 位于的风险事件类型包括：
ms.openlocfilehash: e84cff5985905977b6b1eeb75a9ef9703a2a2078
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044396"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="fe2bf-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe2bf-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="fe2bf-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe2bf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe2bf-107">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)基于位置数据的风险事件。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="fe2bf-108">位于的风险事件类型包括：</span><span class="sxs-lookup"><span data-stu-id="fe2bf-108">Located risk event types include:</span></span>
* [<span data-ttu-id="fe2bf-109">从匿名登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="fe2bf-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="fe2bf-110">从感染恶意软件的设备登录</span><span class="sxs-lookup"><span data-stu-id="fe2bf-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="fe2bf-111">对在典型的位置的意思出差</span><span class="sxs-lookup"><span data-stu-id="fe2bf-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="fe2bf-112">登录从可疑 IP 地址</span><span class="sxs-lookup"><span data-stu-id="fe2bf-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="fe2bf-113">[从不熟悉位置登录](unfamiliarlocationriskevent.md)[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="fe2bf-114">方法</span><span class="sxs-lookup"><span data-stu-id="fe2bf-114">Methods</span></span>

| <span data-ttu-id="fe2bf-115">方法</span><span class="sxs-lookup"><span data-stu-id="fe2bf-115">Method</span></span>           | <span data-ttu-id="fe2bf-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe2bf-116">Return Type</span></span>    |<span data-ttu-id="fe2bf-117">说明</span><span class="sxs-lookup"><span data-stu-id="fe2bf-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe2bf-118">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fe2bf-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="fe2bf-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fe2bf-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="fe2bf-120">读取属性和 locatedRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe2bf-121">属性</span><span class="sxs-lookup"><span data-stu-id="fe2bf-121">Properties</span></span>
| <span data-ttu-id="fe2bf-122">属性</span><span class="sxs-lookup"><span data-stu-id="fe2bf-122">Property</span></span>     | <span data-ttu-id="fe2bf-123">类型</span><span class="sxs-lookup"><span data-stu-id="fe2bf-123">Type</span></span>   |<span data-ttu-id="fe2bf-124">说明</span><span class="sxs-lookup"><span data-stu-id="fe2bf-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe2bf-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe2bf-125">closedDateTime</span></span>|<span data-ttu-id="fe2bf-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe2bf-126">dateTimeOffset</span></span>| <span data-ttu-id="fe2bf-127">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="fe2bf-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="fe2bf-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe2bf-128">createdDateTime</span></span>|<span data-ttu-id="fe2bf-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe2bf-129">dateTimeOffset</span></span>| <span data-ttu-id="fe2bf-130">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="fe2bf-131">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="fe2bf-132">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="fe2bf-133">id</span><span class="sxs-lookup"><span data-stu-id="fe2bf-133">id</span></span>|<span data-ttu-id="fe2bf-134">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-134">string</span></span>| <span data-ttu-id="fe2bf-135">只读</span><span class="sxs-lookup"><span data-stu-id="fe2bf-135">Read-only</span></span>|
|<span data-ttu-id="fe2bf-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="fe2bf-136">ipAddress</span></span>|<span data-ttu-id="fe2bf-137">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-137">string</span></span>| <span data-ttu-id="fe2bf-138">登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="fe2bf-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="fe2bf-139">location</span><span class="sxs-lookup"><span data-stu-id="fe2bf-139">location</span></span>|<span data-ttu-id="fe2bf-140">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-140">string</span></span>| <span data-ttu-id="fe2bf-141">挂接到登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="fe2bf-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="fe2bf-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="fe2bf-142">riskEventDateTime</span></span>|<span data-ttu-id="fe2bf-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe2bf-143">dateTimeOffset</span></span>| <span data-ttu-id="fe2bf-144">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="fe2bf-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="fe2bf-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="fe2bf-145">riskEventStatus</span></span>|<span data-ttu-id="fe2bf-146">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-146">string</span></span>| <span data-ttu-id="fe2bf-147">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="fe2bf-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="fe2bf-148">riskLevel</span></span>|<span data-ttu-id="fe2bf-149">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-149">string</span></span>| <span data-ttu-id="fe2bf-150">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="fe2bf-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="fe2bf-151">riskEventType</span></span>|<span data-ttu-id="fe2bf-152">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-152">string</span></span>| <span data-ttu-id="fe2bf-153">风险类型</span><span class="sxs-lookup"><span data-stu-id="fe2bf-153">The type of risk</span></span>|
|<span data-ttu-id="fe2bf-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe2bf-154">userDisplayName</span></span>|<span data-ttu-id="fe2bf-155">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-155">string</span></span>| <span data-ttu-id="fe2bf-156">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="fe2bf-156">The name of the user at risk</span></span>|
|<span data-ttu-id="fe2bf-157">userId</span><span class="sxs-lookup"><span data-stu-id="fe2bf-157">userId</span></span>|<span data-ttu-id="fe2bf-158">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-158">string</span></span>| <span data-ttu-id="fe2bf-159">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="fe2bf-159">The id of the user at risk</span></span>|
|<span data-ttu-id="fe2bf-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe2bf-160">userPrincipalName</span></span>|<span data-ttu-id="fe2bf-161">string</span><span class="sxs-lookup"><span data-stu-id="fe2bf-161">string</span></span>| <span data-ttu-id="fe2bf-162">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="fe2bf-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe2bf-163">Relationships</span><span class="sxs-lookup"><span data-stu-id="fe2bf-163">Relationships</span></span>
| <span data-ttu-id="fe2bf-164">关系</span><span class="sxs-lookup"><span data-stu-id="fe2bf-164">Relationship</span></span> | <span data-ttu-id="fe2bf-165">类型</span><span class="sxs-lookup"><span data-stu-id="fe2bf-165">Type</span></span>   |<span data-ttu-id="fe2bf-166">说明</span><span class="sxs-lookup"><span data-stu-id="fe2bf-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe2bf-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="fe2bf-167">impactedUser</span></span>|[<span data-ttu-id="fe2bf-168">用户</span><span class="sxs-lookup"><span data-stu-id="fe2bf-168">user</span></span>](user.md)| <span data-ttu-id="fe2bf-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe2bf-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe2bf-171">JSON representation</span></span>

<span data-ttu-id="fe2bf-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe2bf-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->