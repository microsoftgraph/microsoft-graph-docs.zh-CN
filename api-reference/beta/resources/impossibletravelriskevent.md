---
title: impossibleTravelRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件，其中两个帐户登录从用户的非典型位置发生，并且在登录之间的持续时间之间无法进行移动。有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 72492c3542733c194ee4d5560b473cb7a67387c7
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404184"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="44450-103">impossibleTravelRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="44450-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="44450-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44450-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="44450-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="44450-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="44450-106">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="44450-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="44450-107">[Azure Active Directory 标识保护](/azure/active-directory/identity-protection/overview-identity-protection)检测到的风险事件，其中两个帐户登录从用户的非典型位置发生，并且在登录之间的持续时间之间无法进行移动。有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="44450-107">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="44450-108">方法</span><span class="sxs-lookup"><span data-stu-id="44450-108">Methods</span></span>

| <span data-ttu-id="44450-109">方法</span><span class="sxs-lookup"><span data-stu-id="44450-109">Method</span></span>           | <span data-ttu-id="44450-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="44450-110">Return Type</span></span>    |<span data-ttu-id="44450-111">说明</span><span class="sxs-lookup"><span data-stu-id="44450-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44450-112">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44450-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="44450-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="44450-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="44450-114">读取 impossibleTravelRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44450-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44450-115">属性</span><span class="sxs-lookup"><span data-stu-id="44450-115">Properties</span></span>
| <span data-ttu-id="44450-116">属性</span><span class="sxs-lookup"><span data-stu-id="44450-116">Property</span></span>     | <span data-ttu-id="44450-117">类型</span><span class="sxs-lookup"><span data-stu-id="44450-117">Type</span></span>   |<span data-ttu-id="44450-118">说明</span><span class="sxs-lookup"><span data-stu-id="44450-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44450-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="44450-119">closedDateTime</span></span>|<span data-ttu-id="44450-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44450-120">dateTimeOffset</span></span>| <span data-ttu-id="44450-121">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="44450-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="44450-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44450-122">createdDateTime</span></span>|<span data-ttu-id="44450-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44450-123">dateTimeOffset</span></span>| <span data-ttu-id="44450-124">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="44450-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="44450-125">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="44450-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="44450-126">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="44450-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="44450-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="44450-127">deviceInformation</span></span>|<span data-ttu-id="44450-128">string</span><span class="sxs-lookup"><span data-stu-id="44450-128">string</span></span>| <span data-ttu-id="44450-129">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="44450-129">Information about the device</span></span>|
|<span data-ttu-id="44450-130">id</span><span class="sxs-lookup"><span data-stu-id="44450-130">id</span></span>|<span data-ttu-id="44450-131">string</span><span class="sxs-lookup"><span data-stu-id="44450-131">string</span></span>| <span data-ttu-id="44450-132">只读</span><span class="sxs-lookup"><span data-stu-id="44450-132">Read-only</span></span>|
|<span data-ttu-id="44450-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="44450-133">ipAddress</span></span>|<span data-ttu-id="44450-134">string</span><span class="sxs-lookup"><span data-stu-id="44450-134">string</span></span>| <span data-ttu-id="44450-135">第二次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="44450-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="44450-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="44450-136">isAtypicalLocation</span></span>|<span data-ttu-id="44450-137">boolean</span><span class="sxs-lookup"><span data-stu-id="44450-137">boolean</span></span>| <span data-ttu-id="44450-138">如果其中一个位置对用户是典型的</span><span class="sxs-lookup"><span data-stu-id="44450-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="44450-139">location</span><span class="sxs-lookup"><span data-stu-id="44450-139">location</span></span>|<span data-ttu-id="44450-140">string</span><span class="sxs-lookup"><span data-stu-id="44450-140">string</span></span>| <span data-ttu-id="44450-141">连接到第二次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="44450-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="44450-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="44450-142">previousIPAddress</span></span>|<span data-ttu-id="44450-143">string</span><span class="sxs-lookup"><span data-stu-id="44450-143">string</span></span>| <span data-ttu-id="44450-144">第一次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="44450-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="44450-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="44450-145">previousLocation</span></span>|<span data-ttu-id="44450-146">string</span><span class="sxs-lookup"><span data-stu-id="44450-146">string</span></span>| <span data-ttu-id="44450-147">第一次登录的 IP 地址所连接的位置</span><span class="sxs-lookup"><span data-stu-id="44450-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="44450-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="44450-148">previousSigninDateTime</span></span>|<span data-ttu-id="44450-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44450-149">dateTimeOffset</span></span>| <span data-ttu-id="44450-150">首次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="44450-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="44450-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="44450-151">riskEventDateTime</span></span>|<span data-ttu-id="44450-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44450-152">dateTimeOffset</span></span>| <span data-ttu-id="44450-153">第二次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="44450-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="44450-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="44450-154">riskEventStatus</span></span>|<span data-ttu-id="44450-155">string</span><span class="sxs-lookup"><span data-stu-id="44450-155">string</span></span>| <span data-ttu-id="44450-156">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="44450-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="44450-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="44450-157">riskLevel</span></span>|<span data-ttu-id="44450-158">string</span><span class="sxs-lookup"><span data-stu-id="44450-158">string</span></span>| <span data-ttu-id="44450-159">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="44450-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="44450-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="44450-160">riskEventType</span></span>|<span data-ttu-id="44450-161">string</span><span class="sxs-lookup"><span data-stu-id="44450-161">string</span></span>| <span data-ttu-id="44450-162">风险的类型</span><span class="sxs-lookup"><span data-stu-id="44450-162">The type of risk</span></span>|
|<span data-ttu-id="44450-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="44450-163">userAgent</span></span>|<span data-ttu-id="44450-164">string</span><span class="sxs-lookup"><span data-stu-id="44450-164">string</span></span>| <span data-ttu-id="44450-165">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="44450-165">The browser's user agent string</span></span>|
|<span data-ttu-id="44450-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="44450-166">userDisplayName</span></span>|<span data-ttu-id="44450-167">string</span><span class="sxs-lookup"><span data-stu-id="44450-167">string</span></span>| <span data-ttu-id="44450-168">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="44450-168">The name of the user at risk</span></span>|
|<span data-ttu-id="44450-169">userId</span><span class="sxs-lookup"><span data-stu-id="44450-169">userId</span></span>|<span data-ttu-id="44450-170">string</span><span class="sxs-lookup"><span data-stu-id="44450-170">string</span></span>| <span data-ttu-id="44450-171">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="44450-171">The id of the user at risk</span></span>|
|<span data-ttu-id="44450-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44450-172">userPrincipalName</span></span>|<span data-ttu-id="44450-173">string</span><span class="sxs-lookup"><span data-stu-id="44450-173">string</span></span>| <span data-ttu-id="44450-174">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="44450-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="44450-175">关系</span><span class="sxs-lookup"><span data-stu-id="44450-175">Relationships</span></span>
| <span data-ttu-id="44450-176">关系</span><span class="sxs-lookup"><span data-stu-id="44450-176">Relationship</span></span> | <span data-ttu-id="44450-177">类型</span><span class="sxs-lookup"><span data-stu-id="44450-177">Type</span></span>   |<span data-ttu-id="44450-178">说明</span><span class="sxs-lookup"><span data-stu-id="44450-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44450-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="44450-179">impactedUser</span></span>|[<span data-ttu-id="44450-180">用户</span><span class="sxs-lookup"><span data-stu-id="44450-180">user</span></span>](user.md)| <span data-ttu-id="44450-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="44450-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44450-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44450-183">JSON representation</span></span>

<span data-ttu-id="44450-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44450-184">Here is a JSON representation of the resource.</span></span>

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