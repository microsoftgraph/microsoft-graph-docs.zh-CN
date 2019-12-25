---
title: impossibleTravelRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件，其中两个帐户登录从用户的非典型位置发生，并且在登录之间的持续时间之间无法进行移动。有关详细信息，请参阅可在 Azure AD Identity Protection 文档中找到风险事件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: be2b5db09a20264525e783e05771f6d1da2783e2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866782"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="333a5-103">impossibleTravelRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="333a5-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="333a5-104">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="333a5-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="333a5-105">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="333a5-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="333a5-106">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的风险事件，其中两个帐户登录从用户的非典型位置发生，并且在登录之间的持续时间之间无法移动。有关风险事件的完整信息，请参阅[Azure AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="333a5-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="333a5-107">方法</span><span class="sxs-lookup"><span data-stu-id="333a5-107">Methods</span></span>

| <span data-ttu-id="333a5-108">方法</span><span class="sxs-lookup"><span data-stu-id="333a5-108">Method</span></span>           | <span data-ttu-id="333a5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="333a5-109">Return Type</span></span>    |<span data-ttu-id="333a5-110">说明</span><span class="sxs-lookup"><span data-stu-id="333a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="333a5-111">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="333a5-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="333a5-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="333a5-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="333a5-113">读取 impossibleTravelRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="333a5-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="333a5-114">属性</span><span class="sxs-lookup"><span data-stu-id="333a5-114">Properties</span></span>
| <span data-ttu-id="333a5-115">属性</span><span class="sxs-lookup"><span data-stu-id="333a5-115">Property</span></span>     | <span data-ttu-id="333a5-116">类型</span><span class="sxs-lookup"><span data-stu-id="333a5-116">Type</span></span>   |<span data-ttu-id="333a5-117">说明</span><span class="sxs-lookup"><span data-stu-id="333a5-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="333a5-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="333a5-118">closedDateTime</span></span>|<span data-ttu-id="333a5-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="333a5-119">dateTimeOffset</span></span>| <span data-ttu-id="333a5-120">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="333a5-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="333a5-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="333a5-121">createdDateTime</span></span>|<span data-ttu-id="333a5-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="333a5-122">dateTimeOffset</span></span>| <span data-ttu-id="333a5-123">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="333a5-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="333a5-124">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="333a5-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="333a5-125">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="333a5-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="333a5-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="333a5-126">deviceInformation</span></span>|<span data-ttu-id="333a5-127">string</span><span class="sxs-lookup"><span data-stu-id="333a5-127">string</span></span>| <span data-ttu-id="333a5-128">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="333a5-128">Information about the device</span></span>|
|<span data-ttu-id="333a5-129">id</span><span class="sxs-lookup"><span data-stu-id="333a5-129">id</span></span>|<span data-ttu-id="333a5-130">string</span><span class="sxs-lookup"><span data-stu-id="333a5-130">string</span></span>| <span data-ttu-id="333a5-131">只读</span><span class="sxs-lookup"><span data-stu-id="333a5-131">Read-only</span></span>|
|<span data-ttu-id="333a5-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="333a5-132">ipAddress</span></span>|<span data-ttu-id="333a5-133">string</span><span class="sxs-lookup"><span data-stu-id="333a5-133">string</span></span>| <span data-ttu-id="333a5-134">第二次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="333a5-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="333a5-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="333a5-135">isAtypicalLocation</span></span>|<span data-ttu-id="333a5-136">boolean</span><span class="sxs-lookup"><span data-stu-id="333a5-136">boolean</span></span>| <span data-ttu-id="333a5-137">如果其中一个位置对用户是典型的</span><span class="sxs-lookup"><span data-stu-id="333a5-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="333a5-138">location</span><span class="sxs-lookup"><span data-stu-id="333a5-138">location</span></span>|<span data-ttu-id="333a5-139">string</span><span class="sxs-lookup"><span data-stu-id="333a5-139">string</span></span>| <span data-ttu-id="333a5-140">连接到第二次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="333a5-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="333a5-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="333a5-141">previousIPAddress</span></span>|<span data-ttu-id="333a5-142">string</span><span class="sxs-lookup"><span data-stu-id="333a5-142">string</span></span>| <span data-ttu-id="333a5-143">第一次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="333a5-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="333a5-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="333a5-144">previousLocation</span></span>|<span data-ttu-id="333a5-145">string</span><span class="sxs-lookup"><span data-stu-id="333a5-145">string</span></span>| <span data-ttu-id="333a5-146">第一次登录的 IP 地址所连接的位置</span><span class="sxs-lookup"><span data-stu-id="333a5-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="333a5-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="333a5-147">previousSigninDateTime</span></span>|<span data-ttu-id="333a5-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="333a5-148">dateTimeOffset</span></span>| <span data-ttu-id="333a5-149">首次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="333a5-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="333a5-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="333a5-150">riskEventDateTime</span></span>|<span data-ttu-id="333a5-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="333a5-151">dateTimeOffset</span></span>| <span data-ttu-id="333a5-152">第二次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="333a5-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="333a5-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="333a5-153">riskEventStatus</span></span>|<span data-ttu-id="333a5-154">string</span><span class="sxs-lookup"><span data-stu-id="333a5-154">string</span></span>| <span data-ttu-id="333a5-155">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="333a5-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="333a5-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="333a5-156">riskLevel</span></span>|<span data-ttu-id="333a5-157">string</span><span class="sxs-lookup"><span data-stu-id="333a5-157">string</span></span>| <span data-ttu-id="333a5-158">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="333a5-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="333a5-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="333a5-159">riskEventType</span></span>|<span data-ttu-id="333a5-160">string</span><span class="sxs-lookup"><span data-stu-id="333a5-160">string</span></span>| <span data-ttu-id="333a5-161">风险的类型</span><span class="sxs-lookup"><span data-stu-id="333a5-161">The type of risk</span></span>|
|<span data-ttu-id="333a5-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="333a5-162">userAgent</span></span>|<span data-ttu-id="333a5-163">string</span><span class="sxs-lookup"><span data-stu-id="333a5-163">string</span></span>| <span data-ttu-id="333a5-164">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="333a5-164">The browser's user agent string</span></span>|
|<span data-ttu-id="333a5-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="333a5-165">userDisplayName</span></span>|<span data-ttu-id="333a5-166">string</span><span class="sxs-lookup"><span data-stu-id="333a5-166">string</span></span>| <span data-ttu-id="333a5-167">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="333a5-167">The name of the user at risk</span></span>|
|<span data-ttu-id="333a5-168">userId</span><span class="sxs-lookup"><span data-stu-id="333a5-168">userId</span></span>|<span data-ttu-id="333a5-169">string</span><span class="sxs-lookup"><span data-stu-id="333a5-169">string</span></span>| <span data-ttu-id="333a5-170">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="333a5-170">The id of the user at risk</span></span>|
|<span data-ttu-id="333a5-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="333a5-171">userPrincipalName</span></span>|<span data-ttu-id="333a5-172">string</span><span class="sxs-lookup"><span data-stu-id="333a5-172">string</span></span>| <span data-ttu-id="333a5-173">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="333a5-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="333a5-174">关系</span><span class="sxs-lookup"><span data-stu-id="333a5-174">Relationships</span></span>
| <span data-ttu-id="333a5-175">关系</span><span class="sxs-lookup"><span data-stu-id="333a5-175">Relationship</span></span> | <span data-ttu-id="333a5-176">类型</span><span class="sxs-lookup"><span data-stu-id="333a5-176">Type</span></span>   |<span data-ttu-id="333a5-177">说明</span><span class="sxs-lookup"><span data-stu-id="333a5-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="333a5-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="333a5-178">impactedUser</span></span>|[<span data-ttu-id="333a5-179">user</span><span class="sxs-lookup"><span data-stu-id="333a5-179">user</span></span>](user.md)| <span data-ttu-id="333a5-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="333a5-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="333a5-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="333a5-182">JSON representation</span></span>

<span data-ttu-id="333a5-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="333a5-183">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
