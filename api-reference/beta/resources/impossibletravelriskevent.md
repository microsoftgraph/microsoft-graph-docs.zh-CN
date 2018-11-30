---
title: impossibleTravelRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护其中两个帐户登录发生从用户在典型的位置，并将不可能要登录宏的完整信息之间的工期中的位置之间的差旅风险事件Azure AD 身份保护文档中找不到风险事件。
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041783"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="49129-103">impossibleTravelRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="49129-103">impossibleTravelRiskEvent resource type</span></span>

> <span data-ttu-id="49129-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49129-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49129-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49129-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49129-106">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中两个帐户登录发生从用户在典型的位置，并将不可能要登录宏完成之间的工期中的位置之间的差旅风险事件[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的信息。</span><span class="sxs-lookup"><span data-stu-id="49129-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="49129-107">方法</span><span class="sxs-lookup"><span data-stu-id="49129-107">Methods</span></span>

| <span data-ttu-id="49129-108">方法</span><span class="sxs-lookup"><span data-stu-id="49129-108">Method</span></span>           | <span data-ttu-id="49129-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="49129-109">Return Type</span></span>    |<span data-ttu-id="49129-110">说明</span><span class="sxs-lookup"><span data-stu-id="49129-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49129-111">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="49129-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="49129-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="49129-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="49129-113">读取属性和 impossibleTravelRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="49129-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="49129-114">属性</span><span class="sxs-lookup"><span data-stu-id="49129-114">Properties</span></span>
| <span data-ttu-id="49129-115">属性</span><span class="sxs-lookup"><span data-stu-id="49129-115">Property</span></span>     | <span data-ttu-id="49129-116">类型</span><span class="sxs-lookup"><span data-stu-id="49129-116">Type</span></span>   |<span data-ttu-id="49129-117">说明</span><span class="sxs-lookup"><span data-stu-id="49129-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49129-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="49129-118">closedDateTime</span></span>|<span data-ttu-id="49129-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49129-119">dateTimeOffset</span></span>| <span data-ttu-id="49129-120">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="49129-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="49129-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49129-121">createdDateTime</span></span>|<span data-ttu-id="49129-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49129-122">dateTimeOffset</span></span>| <span data-ttu-id="49129-123">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="49129-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="49129-124">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="49129-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="49129-125">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="49129-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="49129-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="49129-126">deviceInformation</span></span>|<span data-ttu-id="49129-127">string</span><span class="sxs-lookup"><span data-stu-id="49129-127">string</span></span>| <span data-ttu-id="49129-128">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="49129-128">Information about the device</span></span>|
|<span data-ttu-id="49129-129">id</span><span class="sxs-lookup"><span data-stu-id="49129-129">id</span></span>|<span data-ttu-id="49129-130">string</span><span class="sxs-lookup"><span data-stu-id="49129-130">string</span></span>| <span data-ttu-id="49129-131">只读</span><span class="sxs-lookup"><span data-stu-id="49129-131">Read-only</span></span>|
|<span data-ttu-id="49129-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="49129-132">ipAddress</span></span>|<span data-ttu-id="49129-133">string</span><span class="sxs-lookup"><span data-stu-id="49129-133">string</span></span>| <span data-ttu-id="49129-134">IP 地址的第二个登录</span><span class="sxs-lookup"><span data-stu-id="49129-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="49129-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="49129-135">isAtypicalLocation</span></span>|<span data-ttu-id="49129-136">boolean</span><span class="sxs-lookup"><span data-stu-id="49129-136">boolean</span></span>| <span data-ttu-id="49129-137">如果在位置之一是用户在典型</span><span class="sxs-lookup"><span data-stu-id="49129-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="49129-138">location</span><span class="sxs-lookup"><span data-stu-id="49129-138">location</span></span>|<span data-ttu-id="49129-139">string</span><span class="sxs-lookup"><span data-stu-id="49129-139">string</span></span>| <span data-ttu-id="49129-140">挂接到第二个登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="49129-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="49129-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="49129-141">previousIPAddress</span></span>|<span data-ttu-id="49129-142">string</span><span class="sxs-lookup"><span data-stu-id="49129-142">string</span></span>| <span data-ttu-id="49129-143">首次登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="49129-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="49129-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="49129-144">previousLocation</span></span>|<span data-ttu-id="49129-145">string</span><span class="sxs-lookup"><span data-stu-id="49129-145">string</span></span>| <span data-ttu-id="49129-146">挂接到首次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="49129-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="49129-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="49129-147">previousSigninDateTime</span></span>|<span data-ttu-id="49129-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49129-148">dateTimeOffset</span></span>| <span data-ttu-id="49129-149">日期和时间的首次登录</span><span class="sxs-lookup"><span data-stu-id="49129-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="49129-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="49129-150">riskEventDateTime</span></span>|<span data-ttu-id="49129-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49129-151">dateTimeOffset</span></span>| <span data-ttu-id="49129-152">日期和时间的第二个登录</span><span class="sxs-lookup"><span data-stu-id="49129-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="49129-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="49129-153">riskEventStatus</span></span>|<span data-ttu-id="49129-154">string</span><span class="sxs-lookup"><span data-stu-id="49129-154">string</span></span>| <span data-ttu-id="49129-155">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="49129-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="49129-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="49129-156">riskLevel</span></span>|<span data-ttu-id="49129-157">string</span><span class="sxs-lookup"><span data-stu-id="49129-157">string</span></span>| <span data-ttu-id="49129-158">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="49129-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="49129-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="49129-159">riskEventType</span></span>|<span data-ttu-id="49129-160">string</span><span class="sxs-lookup"><span data-stu-id="49129-160">string</span></span>| <span data-ttu-id="49129-161">风险类型</span><span class="sxs-lookup"><span data-stu-id="49129-161">The type of risk</span></span>|
|<span data-ttu-id="49129-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="49129-162">userAgent</span></span>|<span data-ttu-id="49129-163">string</span><span class="sxs-lookup"><span data-stu-id="49129-163">string</span></span>| <span data-ttu-id="49129-164">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="49129-164">The browser's user agent string</span></span>|
|<span data-ttu-id="49129-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="49129-165">userDisplayName</span></span>|<span data-ttu-id="49129-166">string</span><span class="sxs-lookup"><span data-stu-id="49129-166">string</span></span>| <span data-ttu-id="49129-167">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="49129-167">The name of the user at risk</span></span>|
|<span data-ttu-id="49129-168">userId</span><span class="sxs-lookup"><span data-stu-id="49129-168">userId</span></span>|<span data-ttu-id="49129-169">string</span><span class="sxs-lookup"><span data-stu-id="49129-169">string</span></span>| <span data-ttu-id="49129-170">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="49129-170">The id of the user at risk</span></span>|
|<span data-ttu-id="49129-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="49129-171">userPrincipalName</span></span>|<span data-ttu-id="49129-172">string</span><span class="sxs-lookup"><span data-stu-id="49129-172">string</span></span>| <span data-ttu-id="49129-173">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="49129-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="49129-174">Relationships</span><span class="sxs-lookup"><span data-stu-id="49129-174">Relationships</span></span>
| <span data-ttu-id="49129-175">关系</span><span class="sxs-lookup"><span data-stu-id="49129-175">Relationship</span></span> | <span data-ttu-id="49129-176">类型</span><span class="sxs-lookup"><span data-stu-id="49129-176">Type</span></span>   |<span data-ttu-id="49129-177">说明</span><span class="sxs-lookup"><span data-stu-id="49129-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49129-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="49129-178">impactedUser</span></span>|[<span data-ttu-id="49129-179">用户</span><span class="sxs-lookup"><span data-stu-id="49129-179">user</span></span>](user.md)| <span data-ttu-id="49129-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="49129-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49129-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49129-182">JSON representation</span></span>

<span data-ttu-id="49129-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49129-183">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->