---
title: impossibleTravelRiskEvent 资源类型
description: Azure Active Directory Identity Protection 检测到的风险事件，其中两个帐户登录发生在用户非典型位置，在登录之间的持续时间内，不可能在位置之间旅行。有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: c62dfda856bf2761290fff93b505669348eded0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440232"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="b1b14-103">impossibleTravelRiskEvent 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="b1b14-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="b1b14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="b1b14-105">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="b1b14-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="b1b14-106">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="b1b14-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="b1b14-107">[Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)检测到的风险事件，其中两个帐户登录发生在用户非典型位置，在登录之间的持续时间内，不可能在位置之间旅行。有关风险事件的完整信息，请参阅[Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="b1b14-107">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="b1b14-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b1b14-108">Methods</span></span>

| <span data-ttu-id="b1b14-109">方法</span><span class="sxs-lookup"><span data-stu-id="b1b14-109">Method</span></span>           | <span data-ttu-id="b1b14-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1b14-110">Return Type</span></span>    |<span data-ttu-id="b1b14-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1b14-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1b14-112">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="b1b14-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="b1b14-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="b1b14-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="b1b14-114">读取 impossibleTravelRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1b14-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1b14-115">属性</span><span class="sxs-lookup"><span data-stu-id="b1b14-115">Properties</span></span>
| <span data-ttu-id="b1b14-116">属性</span><span class="sxs-lookup"><span data-stu-id="b1b14-116">Property</span></span>     | <span data-ttu-id="b1b14-117">类型</span><span class="sxs-lookup"><span data-stu-id="b1b14-117">Type</span></span>   |<span data-ttu-id="b1b14-118">说明</span><span class="sxs-lookup"><span data-stu-id="b1b14-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1b14-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b14-119">closedDateTime</span></span>|<span data-ttu-id="b1b14-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b14-120">dateTimeOffset</span></span>| <span data-ttu-id="b1b14-121">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b1b14-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="b1b14-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b14-122">createdDateTime</span></span>|<span data-ttu-id="b1b14-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b14-123">dateTimeOffset</span></span>| <span data-ttu-id="b1b14-124">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b1b14-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="b1b14-125">这始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="b1b14-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="b1b14-126">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="b1b14-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="b1b14-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="b1b14-127">deviceInformation</span></span>|<span data-ttu-id="b1b14-128">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-128">string</span></span>| <span data-ttu-id="b1b14-129">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="b1b14-129">Information about the device</span></span>|
|<span data-ttu-id="b1b14-130">id</span><span class="sxs-lookup"><span data-stu-id="b1b14-130">id</span></span>|<span data-ttu-id="b1b14-131">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-131">string</span></span>| <span data-ttu-id="b1b14-132">只读</span><span class="sxs-lookup"><span data-stu-id="b1b14-132">Read-only</span></span>|
|<span data-ttu-id="b1b14-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b1b14-133">ipAddress</span></span>|<span data-ttu-id="b1b14-134">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-134">string</span></span>| <span data-ttu-id="b1b14-135">第二次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="b1b14-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="b1b14-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="b1b14-136">isAtypicalLocation</span></span>|<span data-ttu-id="b1b14-137">boolean</span><span class="sxs-lookup"><span data-stu-id="b1b14-137">boolean</span></span>| <span data-ttu-id="b1b14-138">如果其中一个位置对于用户来说是非典型位置</span><span class="sxs-lookup"><span data-stu-id="b1b14-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="b1b14-139">location</span><span class="sxs-lookup"><span data-stu-id="b1b14-139">location</span></span>|<span data-ttu-id="b1b14-140">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-140">string</span></span>| <span data-ttu-id="b1b14-141">附加到第二次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="b1b14-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="b1b14-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="b1b14-142">previousIPAddress</span></span>|<span data-ttu-id="b1b14-143">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-143">string</span></span>| <span data-ttu-id="b1b14-144">首次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="b1b14-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="b1b14-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="b1b14-145">previousLocation</span></span>|<span data-ttu-id="b1b14-146">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-146">string</span></span>| <span data-ttu-id="b1b14-147">附加到首次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="b1b14-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="b1b14-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b14-148">previousSigninDateTime</span></span>|<span data-ttu-id="b1b14-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b14-149">dateTimeOffset</span></span>| <span data-ttu-id="b1b14-150">首次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b1b14-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="b1b14-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b14-151">riskEventDateTime</span></span>|<span data-ttu-id="b1b14-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b14-152">dateTimeOffset</span></span>| <span data-ttu-id="b1b14-153">第二次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b1b14-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="b1b14-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="b1b14-154">riskEventStatus</span></span>|<span data-ttu-id="b1b14-155">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-155">string</span></span>| <span data-ttu-id="b1b14-156">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="b1b14-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="b1b14-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b1b14-157">riskLevel</span></span>|<span data-ttu-id="b1b14-158">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-158">string</span></span>| <span data-ttu-id="b1b14-159">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="b1b14-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="b1b14-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="b1b14-160">riskEventType</span></span>|<span data-ttu-id="b1b14-161">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-161">string</span></span>| <span data-ttu-id="b1b14-162">风险类型</span><span class="sxs-lookup"><span data-stu-id="b1b14-162">The type of risk</span></span>|
|<span data-ttu-id="b1b14-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="b1b14-163">userAgent</span></span>|<span data-ttu-id="b1b14-164">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-164">string</span></span>| <span data-ttu-id="b1b14-165">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="b1b14-165">The browser's user agent string</span></span>|
|<span data-ttu-id="b1b14-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1b14-166">userDisplayName</span></span>|<span data-ttu-id="b1b14-167">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-167">string</span></span>| <span data-ttu-id="b1b14-168">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="b1b14-168">The name of the user at risk</span></span>|
|<span data-ttu-id="b1b14-169">userId</span><span class="sxs-lookup"><span data-stu-id="b1b14-169">userId</span></span>|<span data-ttu-id="b1b14-170">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-170">string</span></span>| <span data-ttu-id="b1b14-171">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="b1b14-171">The id of the user at risk</span></span>|
|<span data-ttu-id="b1b14-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1b14-172">userPrincipalName</span></span>|<span data-ttu-id="b1b14-173">string</span><span class="sxs-lookup"><span data-stu-id="b1b14-173">string</span></span>| <span data-ttu-id="b1b14-174">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b1b14-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1b14-175">关系</span><span class="sxs-lookup"><span data-stu-id="b1b14-175">Relationships</span></span>
| <span data-ttu-id="b1b14-176">关系</span><span class="sxs-lookup"><span data-stu-id="b1b14-176">Relationship</span></span> | <span data-ttu-id="b1b14-177">类型</span><span class="sxs-lookup"><span data-stu-id="b1b14-177">Type</span></span>   |<span data-ttu-id="b1b14-178">说明</span><span class="sxs-lookup"><span data-stu-id="b1b14-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1b14-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="b1b14-179">impactedUser</span></span>|[<span data-ttu-id="b1b14-180">user</span><span class="sxs-lookup"><span data-stu-id="b1b14-180">user</span></span>](user.md)| <span data-ttu-id="b1b14-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="b1b14-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1b14-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1b14-183">JSON representation</span></span>

<span data-ttu-id="b1b14-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1b14-184">Here is a JSON representation of the resource.</span></span>

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
