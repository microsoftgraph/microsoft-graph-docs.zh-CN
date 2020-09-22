---
title: impossibleTravelRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件，其中两个帐户登录从用户的非典型位置发生，并且在登录之间的持续时间之间无法进行移动。有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 893fa85da721f3e28c92f8d9317da0cfb9d9c57e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016553"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="af808-103">impossibleTravelRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="af808-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="af808-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="af808-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="af808-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="af808-106">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="af808-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="af808-107">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的风险事件，其中两个帐户登录从用户的非典型位置发生，并且在登录之间的持续时间之间无法进行移动。有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="af808-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="af808-108">方法</span><span class="sxs-lookup"><span data-stu-id="af808-108">Methods</span></span>

| <span data-ttu-id="af808-109">方法</span><span class="sxs-lookup"><span data-stu-id="af808-109">Method</span></span>           | <span data-ttu-id="af808-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="af808-110">Return Type</span></span>    |<span data-ttu-id="af808-111">说明</span><span class="sxs-lookup"><span data-stu-id="af808-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af808-112">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="af808-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="af808-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="af808-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="af808-114">读取 impossibleTravelRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af808-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af808-115">属性</span><span class="sxs-lookup"><span data-stu-id="af808-115">Properties</span></span>
| <span data-ttu-id="af808-116">属性</span><span class="sxs-lookup"><span data-stu-id="af808-116">Property</span></span>     | <span data-ttu-id="af808-117">类型</span><span class="sxs-lookup"><span data-stu-id="af808-117">Type</span></span>   |<span data-ttu-id="af808-118">说明</span><span class="sxs-lookup"><span data-stu-id="af808-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af808-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="af808-119">closedDateTime</span></span>|<span data-ttu-id="af808-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af808-120">dateTimeOffset</span></span>| <span data-ttu-id="af808-121">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="af808-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="af808-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af808-122">createdDateTime</span></span>|<span data-ttu-id="af808-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af808-123">dateTimeOffset</span></span>| <span data-ttu-id="af808-124">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af808-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="af808-125">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="af808-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="af808-126">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="af808-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="af808-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="af808-127">deviceInformation</span></span>|<span data-ttu-id="af808-128">string</span><span class="sxs-lookup"><span data-stu-id="af808-128">string</span></span>| <span data-ttu-id="af808-129">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="af808-129">Information about the device</span></span>|
|<span data-ttu-id="af808-130">id</span><span class="sxs-lookup"><span data-stu-id="af808-130">id</span></span>|<span data-ttu-id="af808-131">string</span><span class="sxs-lookup"><span data-stu-id="af808-131">string</span></span>| <span data-ttu-id="af808-132">只读</span><span class="sxs-lookup"><span data-stu-id="af808-132">Read-only</span></span>|
|<span data-ttu-id="af808-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="af808-133">ipAddress</span></span>|<span data-ttu-id="af808-134">string</span><span class="sxs-lookup"><span data-stu-id="af808-134">string</span></span>| <span data-ttu-id="af808-135">第二次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="af808-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="af808-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="af808-136">isAtypicalLocation</span></span>|<span data-ttu-id="af808-137">boolean</span><span class="sxs-lookup"><span data-stu-id="af808-137">boolean</span></span>| <span data-ttu-id="af808-138">如果其中一个位置对用户是典型的</span><span class="sxs-lookup"><span data-stu-id="af808-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="af808-139">location</span><span class="sxs-lookup"><span data-stu-id="af808-139">location</span></span>|<span data-ttu-id="af808-140">string</span><span class="sxs-lookup"><span data-stu-id="af808-140">string</span></span>| <span data-ttu-id="af808-141">连接到第二次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="af808-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="af808-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="af808-142">previousIPAddress</span></span>|<span data-ttu-id="af808-143">string</span><span class="sxs-lookup"><span data-stu-id="af808-143">string</span></span>| <span data-ttu-id="af808-144">第一次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="af808-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="af808-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="af808-145">previousLocation</span></span>|<span data-ttu-id="af808-146">string</span><span class="sxs-lookup"><span data-stu-id="af808-146">string</span></span>| <span data-ttu-id="af808-147">第一次登录的 IP 地址所连接的位置</span><span class="sxs-lookup"><span data-stu-id="af808-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="af808-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="af808-148">previousSigninDateTime</span></span>|<span data-ttu-id="af808-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af808-149">dateTimeOffset</span></span>| <span data-ttu-id="af808-150">首次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="af808-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="af808-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="af808-151">riskEventDateTime</span></span>|<span data-ttu-id="af808-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af808-152">dateTimeOffset</span></span>| <span data-ttu-id="af808-153">第二次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="af808-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="af808-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="af808-154">riskEventStatus</span></span>|<span data-ttu-id="af808-155">string</span><span class="sxs-lookup"><span data-stu-id="af808-155">string</span></span>| <span data-ttu-id="af808-156">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="af808-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="af808-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="af808-157">riskLevel</span></span>|<span data-ttu-id="af808-158">string</span><span class="sxs-lookup"><span data-stu-id="af808-158">string</span></span>| <span data-ttu-id="af808-159">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="af808-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="af808-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="af808-160">riskEventType</span></span>|<span data-ttu-id="af808-161">string</span><span class="sxs-lookup"><span data-stu-id="af808-161">string</span></span>| <span data-ttu-id="af808-162">风险的类型</span><span class="sxs-lookup"><span data-stu-id="af808-162">The type of risk</span></span>|
|<span data-ttu-id="af808-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="af808-163">userAgent</span></span>|<span data-ttu-id="af808-164">string</span><span class="sxs-lookup"><span data-stu-id="af808-164">string</span></span>| <span data-ttu-id="af808-165">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="af808-165">The browser's user agent string</span></span>|
|<span data-ttu-id="af808-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="af808-166">userDisplayName</span></span>|<span data-ttu-id="af808-167">string</span><span class="sxs-lookup"><span data-stu-id="af808-167">string</span></span>| <span data-ttu-id="af808-168">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="af808-168">The name of the user at risk</span></span>|
|<span data-ttu-id="af808-169">userId</span><span class="sxs-lookup"><span data-stu-id="af808-169">userId</span></span>|<span data-ttu-id="af808-170">string</span><span class="sxs-lookup"><span data-stu-id="af808-170">string</span></span>| <span data-ttu-id="af808-171">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="af808-171">The id of the user at risk</span></span>|
|<span data-ttu-id="af808-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af808-172">userPrincipalName</span></span>|<span data-ttu-id="af808-173">string</span><span class="sxs-lookup"><span data-stu-id="af808-173">string</span></span>| <span data-ttu-id="af808-174">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="af808-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="af808-175">关系</span><span class="sxs-lookup"><span data-stu-id="af808-175">Relationships</span></span>
| <span data-ttu-id="af808-176">关系</span><span class="sxs-lookup"><span data-stu-id="af808-176">Relationship</span></span> | <span data-ttu-id="af808-177">类型</span><span class="sxs-lookup"><span data-stu-id="af808-177">Type</span></span>   |<span data-ttu-id="af808-178">说明</span><span class="sxs-lookup"><span data-stu-id="af808-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af808-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="af808-179">impactedUser</span></span>|[<span data-ttu-id="af808-180">用户</span><span class="sxs-lookup"><span data-stu-id="af808-180">user</span></span>](user.md)| <span data-ttu-id="af808-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="af808-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af808-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af808-183">JSON representation</span></span>

<span data-ttu-id="af808-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af808-184">Here is a JSON representation of the resource.</span></span>

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


