---
title: impossibleTravelRiskEvent 资源类型
description: 由 Azure Active Directory Identity Protection 检测到的风险事件，其中两个帐户登录发生在用户非典型位置，在两次登录之间的持续时间内，无法在这两个位置之间进行。有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: e05760bc4e3c60d3d4079965cdf01b0d5f630a77
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547006"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="8695d-103">impossibleTravelRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="8695d-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="8695d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8695d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="8695d-105">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="8695d-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="8695d-106">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="8695d-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="8695d-107">[由 Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)检测到的风险事件，其中两个帐户登录发生在用户非典型位置，在两次登录之间的持续时间内，无法在这两个位置之间旅行。有关风险事件的完整信息，请参阅[Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="8695d-107">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="8695d-108">方法</span><span class="sxs-lookup"><span data-stu-id="8695d-108">Methods</span></span>

| <span data-ttu-id="8695d-109">方法</span><span class="sxs-lookup"><span data-stu-id="8695d-109">Method</span></span>           | <span data-ttu-id="8695d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8695d-110">Return Type</span></span>    |<span data-ttu-id="8695d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8695d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8695d-112">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8695d-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="8695d-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8695d-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="8695d-114">读取 impossibleTravelRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8695d-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8695d-115">属性</span><span class="sxs-lookup"><span data-stu-id="8695d-115">Properties</span></span>
| <span data-ttu-id="8695d-116">属性</span><span class="sxs-lookup"><span data-stu-id="8695d-116">Property</span></span>     | <span data-ttu-id="8695d-117">类型</span><span class="sxs-lookup"><span data-stu-id="8695d-117">Type</span></span>   |<span data-ttu-id="8695d-118">说明</span><span class="sxs-lookup"><span data-stu-id="8695d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8695d-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="8695d-119">closedDateTime</span></span>|<span data-ttu-id="8695d-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8695d-120">dateTimeOffset</span></span>| <span data-ttu-id="8695d-121">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="8695d-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="8695d-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8695d-122">createdDateTime</span></span>|<span data-ttu-id="8695d-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8695d-123">dateTimeOffset</span></span>| <span data-ttu-id="8695d-124">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8695d-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="8695d-125">这始终大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="8695d-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="8695d-126">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="8695d-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="8695d-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="8695d-127">deviceInformation</span></span>|<span data-ttu-id="8695d-128">string</span><span class="sxs-lookup"><span data-stu-id="8695d-128">string</span></span>| <span data-ttu-id="8695d-129">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="8695d-129">Information about the device</span></span>|
|<span data-ttu-id="8695d-130">id</span><span class="sxs-lookup"><span data-stu-id="8695d-130">id</span></span>|<span data-ttu-id="8695d-131">string</span><span class="sxs-lookup"><span data-stu-id="8695d-131">string</span></span>| <span data-ttu-id="8695d-132">只读</span><span class="sxs-lookup"><span data-stu-id="8695d-132">Read-only</span></span>|
|<span data-ttu-id="8695d-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8695d-133">ipAddress</span></span>|<span data-ttu-id="8695d-134">string</span><span class="sxs-lookup"><span data-stu-id="8695d-134">string</span></span>| <span data-ttu-id="8695d-135">第二次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="8695d-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="8695d-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="8695d-136">isAtypicalLocation</span></span>|<span data-ttu-id="8695d-137">boolean</span><span class="sxs-lookup"><span data-stu-id="8695d-137">boolean</span></span>| <span data-ttu-id="8695d-138">如果其中一个位置对于用户来说不是典型位置</span><span class="sxs-lookup"><span data-stu-id="8695d-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="8695d-139">location</span><span class="sxs-lookup"><span data-stu-id="8695d-139">location</span></span>|<span data-ttu-id="8695d-140">string</span><span class="sxs-lookup"><span data-stu-id="8695d-140">string</span></span>| <span data-ttu-id="8695d-141">附加到第二次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="8695d-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="8695d-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="8695d-142">previousIPAddress</span></span>|<span data-ttu-id="8695d-143">string</span><span class="sxs-lookup"><span data-stu-id="8695d-143">string</span></span>| <span data-ttu-id="8695d-144">首次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="8695d-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="8695d-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="8695d-145">previousLocation</span></span>|<span data-ttu-id="8695d-146">string</span><span class="sxs-lookup"><span data-stu-id="8695d-146">string</span></span>| <span data-ttu-id="8695d-147">附加到首次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="8695d-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="8695d-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="8695d-148">previousSigninDateTime</span></span>|<span data-ttu-id="8695d-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8695d-149">dateTimeOffset</span></span>| <span data-ttu-id="8695d-150">首次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="8695d-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="8695d-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="8695d-151">riskEventDateTime</span></span>|<span data-ttu-id="8695d-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8695d-152">dateTimeOffset</span></span>| <span data-ttu-id="8695d-153">第二次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="8695d-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="8695d-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="8695d-154">riskEventStatus</span></span>|<span data-ttu-id="8695d-155">string</span><span class="sxs-lookup"><span data-stu-id="8695d-155">string</span></span>| <span data-ttu-id="8695d-156">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="8695d-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="8695d-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8695d-157">riskLevel</span></span>|<span data-ttu-id="8695d-158">string</span><span class="sxs-lookup"><span data-stu-id="8695d-158">string</span></span>| <span data-ttu-id="8695d-159">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="8695d-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="8695d-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="8695d-160">riskEventType</span></span>|<span data-ttu-id="8695d-161">string</span><span class="sxs-lookup"><span data-stu-id="8695d-161">string</span></span>| <span data-ttu-id="8695d-162">风险类型</span><span class="sxs-lookup"><span data-stu-id="8695d-162">The type of risk</span></span>|
|<span data-ttu-id="8695d-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="8695d-163">userAgent</span></span>|<span data-ttu-id="8695d-164">string</span><span class="sxs-lookup"><span data-stu-id="8695d-164">string</span></span>| <span data-ttu-id="8695d-165">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="8695d-165">The browser's user agent string</span></span>|
|<span data-ttu-id="8695d-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8695d-166">userDisplayName</span></span>|<span data-ttu-id="8695d-167">string</span><span class="sxs-lookup"><span data-stu-id="8695d-167">string</span></span>| <span data-ttu-id="8695d-168">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="8695d-168">The name of the user at risk</span></span>|
|<span data-ttu-id="8695d-169">userId</span><span class="sxs-lookup"><span data-stu-id="8695d-169">userId</span></span>|<span data-ttu-id="8695d-170">string</span><span class="sxs-lookup"><span data-stu-id="8695d-170">string</span></span>| <span data-ttu-id="8695d-171">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="8695d-171">The id of the user at risk</span></span>|
|<span data-ttu-id="8695d-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8695d-172">userPrincipalName</span></span>|<span data-ttu-id="8695d-173">string</span><span class="sxs-lookup"><span data-stu-id="8695d-173">string</span></span>| <span data-ttu-id="8695d-174">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="8695d-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="8695d-175">关系</span><span class="sxs-lookup"><span data-stu-id="8695d-175">Relationships</span></span>
| <span data-ttu-id="8695d-176">关系</span><span class="sxs-lookup"><span data-stu-id="8695d-176">Relationship</span></span> | <span data-ttu-id="8695d-177">类型</span><span class="sxs-lookup"><span data-stu-id="8695d-177">Type</span></span>   |<span data-ttu-id="8695d-178">说明</span><span class="sxs-lookup"><span data-stu-id="8695d-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8695d-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="8695d-179">impactedUser</span></span>|[<span data-ttu-id="8695d-180">user</span><span class="sxs-lookup"><span data-stu-id="8695d-180">user</span></span>](user.md)| <span data-ttu-id="8695d-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="8695d-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8695d-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8695d-183">JSON representation</span></span>

<span data-ttu-id="8695d-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8695d-184">Here is a JSON representation of the resource.</span></span>

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
