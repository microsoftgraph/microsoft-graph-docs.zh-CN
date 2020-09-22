---
title: anonymousIpRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的一个风险事件，其中的帐户登录尝试来自看似匿名的 IP 地址。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: e233e1995748f57a5da9eca51bf336b60d5273b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004268"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="f8cc1-104">anonymousIpRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="f8cc1-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="f8cc1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8cc1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="f8cc1-106">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="f8cc1-107">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="f8cc1-108">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的一个风险事件，其中的帐户登录尝试来自看似匿名的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="f8cc1-109">有关风险事件的完整信息，请参阅 [AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="f8cc1-110">方法</span><span class="sxs-lookup"><span data-stu-id="f8cc1-110">Methods</span></span>

| <span data-ttu-id="f8cc1-111">方法</span><span class="sxs-lookup"><span data-stu-id="f8cc1-111">Method</span></span>           | <span data-ttu-id="f8cc1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8cc1-112">Return Type</span></span>    |<span data-ttu-id="f8cc1-113">说明</span><span class="sxs-lookup"><span data-stu-id="f8cc1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8cc1-114">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f8cc1-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="f8cc1-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f8cc1-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="f8cc1-116">读取 anonymousIpRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f8cc1-117">属性</span><span class="sxs-lookup"><span data-stu-id="f8cc1-117">Properties</span></span>
| <span data-ttu-id="f8cc1-118">属性</span><span class="sxs-lookup"><span data-stu-id="f8cc1-118">Property</span></span>     | <span data-ttu-id="f8cc1-119">类型</span><span class="sxs-lookup"><span data-stu-id="f8cc1-119">Type</span></span>   |<span data-ttu-id="f8cc1-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8cc1-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8cc1-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8cc1-121">closedDateTime</span></span>|<span data-ttu-id="f8cc1-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8cc1-122">dateTimeOffset</span></span>| <span data-ttu-id="f8cc1-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="f8cc1-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f8cc1-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8cc1-124">createdDateTime</span></span>|<span data-ttu-id="f8cc1-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8cc1-125">dateTimeOffset</span></span>| <span data-ttu-id="f8cc1-126">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="f8cc1-127">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f8cc1-128">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f8cc1-129">id</span><span class="sxs-lookup"><span data-stu-id="f8cc1-129">id</span></span>|<span data-ttu-id="f8cc1-130">string</span><span class="sxs-lookup"><span data-stu-id="f8cc1-130">string</span></span>| <span data-ttu-id="f8cc1-131">只读</span><span class="sxs-lookup"><span data-stu-id="f8cc1-131">Read-only</span></span>|
|<span data-ttu-id="f8cc1-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f8cc1-132">ipAddress</span></span>|<span data-ttu-id="f8cc1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f8cc1-133">string</span></span>| <span data-ttu-id="f8cc1-134">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="f8cc1-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="f8cc1-135">location</span><span class="sxs-lookup"><span data-stu-id="f8cc1-135">location</span></span>|<span data-ttu-id="f8cc1-136">string</span><span class="sxs-lookup"><span data-stu-id="f8cc1-136">string</span></span>| <span data-ttu-id="f8cc1-137">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="f8cc1-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="f8cc1-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f8cc1-138">riskEventDateTime</span></span>|<span data-ttu-id="f8cc1-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8cc1-139">dateTimeOffset</span></span>| <span data-ttu-id="f8cc1-140">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="f8cc1-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f8cc1-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f8cc1-141">riskEventStatus</span></span>|<span data-ttu-id="f8cc1-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f8cc1-142">string</span></span>| <span data-ttu-id="f8cc1-143">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f8cc1-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f8cc1-144">riskLevel</span></span>|<span data-ttu-id="f8cc1-145">string</span><span class="sxs-lookup"><span data-stu-id="f8cc1-145">string</span></span>| <span data-ttu-id="f8cc1-146">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f8cc1-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f8cc1-147">riskEventType</span></span>|<span data-ttu-id="f8cc1-148">字符串</span><span class="sxs-lookup"><span data-stu-id="f8cc1-148">string</span></span>| <span data-ttu-id="f8cc1-149">风险的类型</span><span class="sxs-lookup"><span data-stu-id="f8cc1-149">The type of risk</span></span>|
|<span data-ttu-id="f8cc1-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f8cc1-150">userDisplayName</span></span>|<span data-ttu-id="f8cc1-151">字符串</span><span class="sxs-lookup"><span data-stu-id="f8cc1-151">string</span></span>| <span data-ttu-id="f8cc1-152">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="f8cc1-152">The name of the user at risk</span></span>|
|<span data-ttu-id="f8cc1-153">userId</span><span class="sxs-lookup"><span data-stu-id="f8cc1-153">userId</span></span>|<span data-ttu-id="f8cc1-154">string</span><span class="sxs-lookup"><span data-stu-id="f8cc1-154">string</span></span>| <span data-ttu-id="f8cc1-155">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="f8cc1-155">The id of the user at risk</span></span>|
|<span data-ttu-id="f8cc1-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8cc1-156">userPrincipalName</span></span>|<span data-ttu-id="f8cc1-157">string</span><span class="sxs-lookup"><span data-stu-id="f8cc1-157">string</span></span>| <span data-ttu-id="f8cc1-158">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f8cc1-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8cc1-159">关系</span><span class="sxs-lookup"><span data-stu-id="f8cc1-159">Relationships</span></span>
| <span data-ttu-id="f8cc1-160">关系</span><span class="sxs-lookup"><span data-stu-id="f8cc1-160">Relationship</span></span> | <span data-ttu-id="f8cc1-161">类型</span><span class="sxs-lookup"><span data-stu-id="f8cc1-161">Type</span></span>   |<span data-ttu-id="f8cc1-162">说明</span><span class="sxs-lookup"><span data-stu-id="f8cc1-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8cc1-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f8cc1-163">impactedUser</span></span>|[<span data-ttu-id="f8cc1-164">用户</span><span class="sxs-lookup"><span data-stu-id="f8cc1-164">user</span></span>](user.md)| <span data-ttu-id="f8cc1-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8cc1-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8cc1-167">JSON representation</span></span>

<span data-ttu-id="f8cc1-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8cc1-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


