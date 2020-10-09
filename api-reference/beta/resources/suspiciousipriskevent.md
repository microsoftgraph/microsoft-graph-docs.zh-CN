---
title: suspiciousIpRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的、从可疑 IP 地址尝试登录帐户的风险事件。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 68952fb80906a90c62798422d3fc302336311cab
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406058"
---
# <a name="suspiciousipriskevent-resource-type-deprecated"></a><span data-ttu-id="6fc39-104">suspiciousIpRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="6fc39-104">suspiciousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="6fc39-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc39-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="6fc39-106">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="6fc39-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="6fc39-107">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="6fc39-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="6fc39-108">[Azure Active Directory 标识保护](/azure/active-directory/identity-protection/overview-identity-protection)检测到的、从可疑 IP 地址尝试登录帐户的风险事件。</span><span class="sxs-lookup"><span data-stu-id="6fc39-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="6fc39-109">有关风险事件的完整信息，请参阅 [AZURE AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="6fc39-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="6fc39-110">方法</span><span class="sxs-lookup"><span data-stu-id="6fc39-110">Methods</span></span>

| <span data-ttu-id="6fc39-111">方法</span><span class="sxs-lookup"><span data-stu-id="6fc39-111">Method</span></span>           | <span data-ttu-id="6fc39-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fc39-112">Return Type</span></span>    |<span data-ttu-id="6fc39-113">说明</span><span class="sxs-lookup"><span data-stu-id="6fc39-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6fc39-114">获取 suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="6fc39-114">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="6fc39-115">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="6fc39-115">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="6fc39-116">读取 suspiciousIpRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fc39-116">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fc39-117">属性</span><span class="sxs-lookup"><span data-stu-id="6fc39-117">Properties</span></span>
| <span data-ttu-id="6fc39-118">属性</span><span class="sxs-lookup"><span data-stu-id="6fc39-118">Property</span></span>     | <span data-ttu-id="6fc39-119">类型</span><span class="sxs-lookup"><span data-stu-id="6fc39-119">Type</span></span>   |<span data-ttu-id="6fc39-120">说明</span><span class="sxs-lookup"><span data-stu-id="6fc39-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fc39-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc39-121">closedDateTime</span></span>|<span data-ttu-id="6fc39-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc39-122">dateTimeOffset</span></span>| <span data-ttu-id="6fc39-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="6fc39-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="6fc39-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc39-124">createdDateTime</span></span>|<span data-ttu-id="6fc39-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc39-125">dateTimeOffset</span></span>| <span data-ttu-id="6fc39-126">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6fc39-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="6fc39-127">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="6fc39-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="6fc39-128">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="6fc39-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="6fc39-129">id</span><span class="sxs-lookup"><span data-stu-id="6fc39-129">id</span></span>|<span data-ttu-id="6fc39-130">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-130">string</span></span>| <span data-ttu-id="6fc39-131">只读</span><span class="sxs-lookup"><span data-stu-id="6fc39-131">Read-only</span></span>|
|<span data-ttu-id="6fc39-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6fc39-132">ipAddress</span></span>|<span data-ttu-id="6fc39-133">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-133">string</span></span>| <span data-ttu-id="6fc39-134">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="6fc39-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="6fc39-135">location</span><span class="sxs-lookup"><span data-stu-id="6fc39-135">location</span></span>|<span data-ttu-id="6fc39-136">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-136">string</span></span>| <span data-ttu-id="6fc39-137">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="6fc39-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="6fc39-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc39-138">riskEventDateTime</span></span>|<span data-ttu-id="6fc39-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc39-139">dateTimeOffset</span></span>| <span data-ttu-id="6fc39-140">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="6fc39-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="6fc39-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="6fc39-141">riskEventStatus</span></span>|<span data-ttu-id="6fc39-142">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-142">string</span></span>| <span data-ttu-id="6fc39-143">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="6fc39-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="6fc39-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="6fc39-144">riskLevel</span></span>|<span data-ttu-id="6fc39-145">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-145">string</span></span>| <span data-ttu-id="6fc39-146">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="6fc39-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="6fc39-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="6fc39-147">riskEventType</span></span>|<span data-ttu-id="6fc39-148">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-148">string</span></span>| <span data-ttu-id="6fc39-149">风险的类型</span><span class="sxs-lookup"><span data-stu-id="6fc39-149">The type of risk</span></span>|
|<span data-ttu-id="6fc39-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6fc39-150">userDisplayName</span></span>|<span data-ttu-id="6fc39-151">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-151">string</span></span>| <span data-ttu-id="6fc39-152">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="6fc39-152">The name of the user at risk</span></span>|
|<span data-ttu-id="6fc39-153">userId</span><span class="sxs-lookup"><span data-stu-id="6fc39-153">userId</span></span>|<span data-ttu-id="6fc39-154">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-154">string</span></span>| <span data-ttu-id="6fc39-155">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="6fc39-155">The id of the user at risk</span></span>|
|<span data-ttu-id="6fc39-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6fc39-156">userPrincipalName</span></span>|<span data-ttu-id="6fc39-157">string</span><span class="sxs-lookup"><span data-stu-id="6fc39-157">string</span></span>| <span data-ttu-id="6fc39-158">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6fc39-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fc39-159">关系</span><span class="sxs-lookup"><span data-stu-id="6fc39-159">Relationships</span></span>
| <span data-ttu-id="6fc39-160">关系</span><span class="sxs-lookup"><span data-stu-id="6fc39-160">Relationship</span></span> | <span data-ttu-id="6fc39-161">类型</span><span class="sxs-lookup"><span data-stu-id="6fc39-161">Type</span></span>   |<span data-ttu-id="6fc39-162">说明</span><span class="sxs-lookup"><span data-stu-id="6fc39-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fc39-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="6fc39-163">impactedUser</span></span>|[<span data-ttu-id="6fc39-164">用户</span><span class="sxs-lookup"><span data-stu-id="6fc39-164">user</span></span>](user.md)| <span data-ttu-id="6fc39-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="6fc39-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc39-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fc39-167">JSON representation</span></span>

<span data-ttu-id="6fc39-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc39-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->