---
title: locatedRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护基于位置数据的风险事件。 位于的风险事件类型包括：
localization_priority: Normal
ms.openlocfilehash: 256c7a980fb9540e7e80337a5b8aad29fe73f26a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867555"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="0e86a-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e86a-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="0e86a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e86a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e86a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e86a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e86a-107">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)基于位置数据的风险事件。</span><span class="sxs-lookup"><span data-stu-id="0e86a-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="0e86a-108">位于的风险事件类型包括：</span><span class="sxs-lookup"><span data-stu-id="0e86a-108">Located risk event types include:</span></span>
* [<span data-ttu-id="0e86a-109">从匿名登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="0e86a-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="0e86a-110">从感染恶意软件的设备登录</span><span class="sxs-lookup"><span data-stu-id="0e86a-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="0e86a-111">对在典型的位置的意思出差</span><span class="sxs-lookup"><span data-stu-id="0e86a-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="0e86a-112">登录从可疑 IP 地址</span><span class="sxs-lookup"><span data-stu-id="0e86a-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="0e86a-113">[从不熟悉位置登录](unfamiliarlocationriskevent.md)[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="0e86a-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="0e86a-114">方法</span><span class="sxs-lookup"><span data-stu-id="0e86a-114">Methods</span></span>

| <span data-ttu-id="0e86a-115">方法</span><span class="sxs-lookup"><span data-stu-id="0e86a-115">Method</span></span>           | <span data-ttu-id="0e86a-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e86a-116">Return Type</span></span>    |<span data-ttu-id="0e86a-117">说明</span><span class="sxs-lookup"><span data-stu-id="0e86a-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e86a-118">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0e86a-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="0e86a-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0e86a-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="0e86a-120">读取属性和 locatedRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0e86a-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e86a-121">属性</span><span class="sxs-lookup"><span data-stu-id="0e86a-121">Properties</span></span>
| <span data-ttu-id="0e86a-122">属性</span><span class="sxs-lookup"><span data-stu-id="0e86a-122">Property</span></span>     | <span data-ttu-id="0e86a-123">类型</span><span class="sxs-lookup"><span data-stu-id="0e86a-123">Type</span></span>   |<span data-ttu-id="0e86a-124">Description</span><span class="sxs-lookup"><span data-stu-id="0e86a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e86a-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86a-125">closedDateTime</span></span>|<span data-ttu-id="0e86a-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86a-126">dateTimeOffset</span></span>| <span data-ttu-id="0e86a-127">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="0e86a-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="0e86a-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86a-128">createdDateTime</span></span>|<span data-ttu-id="0e86a-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86a-129">dateTimeOffset</span></span>| <span data-ttu-id="0e86a-130">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="0e86a-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="0e86a-131">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="0e86a-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="0e86a-132">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="0e86a-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="0e86a-133">id</span><span class="sxs-lookup"><span data-stu-id="0e86a-133">id</span></span>|<span data-ttu-id="0e86a-134">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-134">string</span></span>| <span data-ttu-id="0e86a-135">只读</span><span class="sxs-lookup"><span data-stu-id="0e86a-135">Read-only</span></span>|
|<span data-ttu-id="0e86a-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0e86a-136">ipAddress</span></span>|<span data-ttu-id="0e86a-137">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-137">string</span></span>| <span data-ttu-id="0e86a-138">登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="0e86a-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="0e86a-139">location</span><span class="sxs-lookup"><span data-stu-id="0e86a-139">location</span></span>|<span data-ttu-id="0e86a-140">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-140">string</span></span>| <span data-ttu-id="0e86a-141">挂接到登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="0e86a-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="0e86a-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86a-142">riskEventDateTime</span></span>|<span data-ttu-id="0e86a-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86a-143">dateTimeOffset</span></span>| <span data-ttu-id="0e86a-144">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="0e86a-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="0e86a-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="0e86a-145">riskEventStatus</span></span>|<span data-ttu-id="0e86a-146">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-146">string</span></span>| <span data-ttu-id="0e86a-147">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="0e86a-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="0e86a-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0e86a-148">riskLevel</span></span>|<span data-ttu-id="0e86a-149">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-149">string</span></span>| <span data-ttu-id="0e86a-150">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0e86a-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="0e86a-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="0e86a-151">riskEventType</span></span>|<span data-ttu-id="0e86a-152">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-152">string</span></span>| <span data-ttu-id="0e86a-153">风险类型</span><span class="sxs-lookup"><span data-stu-id="0e86a-153">The type of risk</span></span>|
|<span data-ttu-id="0e86a-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e86a-154">userDisplayName</span></span>|<span data-ttu-id="0e86a-155">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-155">string</span></span>| <span data-ttu-id="0e86a-156">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="0e86a-156">The name of the user at risk</span></span>|
|<span data-ttu-id="0e86a-157">userId</span><span class="sxs-lookup"><span data-stu-id="0e86a-157">userId</span></span>|<span data-ttu-id="0e86a-158">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-158">string</span></span>| <span data-ttu-id="0e86a-159">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="0e86a-159">The id of the user at risk</span></span>|
|<span data-ttu-id="0e86a-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e86a-160">userPrincipalName</span></span>|<span data-ttu-id="0e86a-161">string</span><span class="sxs-lookup"><span data-stu-id="0e86a-161">string</span></span>| <span data-ttu-id="0e86a-162">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="0e86a-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e86a-163">Relationships</span><span class="sxs-lookup"><span data-stu-id="0e86a-163">Relationships</span></span>
| <span data-ttu-id="0e86a-164">关系</span><span class="sxs-lookup"><span data-stu-id="0e86a-164">Relationship</span></span> | <span data-ttu-id="0e86a-165">类型</span><span class="sxs-lookup"><span data-stu-id="0e86a-165">Type</span></span>   |<span data-ttu-id="0e86a-166">Description</span><span class="sxs-lookup"><span data-stu-id="0e86a-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e86a-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="0e86a-167">impactedUser</span></span>|[<span data-ttu-id="0e86a-168">用户</span><span class="sxs-lookup"><span data-stu-id="0e86a-168">user</span></span>](user.md)| <span data-ttu-id="0e86a-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0e86a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e86a-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e86a-171">JSON representation</span></span>

<span data-ttu-id="0e86a-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e86a-172">Here is a JSON representation of the resource.</span></span>

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
