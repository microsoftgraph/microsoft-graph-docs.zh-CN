---
title: anonymousIpRiskEvent 资源类型
description: Identity Protection 检测到的风险Azure Active Directory，其中帐户从看起来是匿名的 IP 地址尝试登录。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: d4acf5d9b3d5d05a2769178657b397b22f1cb3f2
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547546"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="58744-104">anonymousIpRiskEvent 资源类型 (已弃) </span><span class="sxs-lookup"><span data-stu-id="58744-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="58744-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58744-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="58744-106">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="58744-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="58744-107">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="58744-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="58744-108">由 Azure Active Directory [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)检测到的风险事件，其中帐户从看起来是匿名的 IP 地址尝试登录。</span><span class="sxs-lookup"><span data-stu-id="58744-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="58744-109">有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="58744-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="58744-110">方法</span><span class="sxs-lookup"><span data-stu-id="58744-110">Methods</span></span>

| <span data-ttu-id="58744-111">方法</span><span class="sxs-lookup"><span data-stu-id="58744-111">Method</span></span>           | <span data-ttu-id="58744-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="58744-112">Return Type</span></span>    |<span data-ttu-id="58744-113">说明</span><span class="sxs-lookup"><span data-stu-id="58744-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58744-114">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58744-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="58744-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="58744-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="58744-116">读取 anonymousIpRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58744-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58744-117">属性</span><span class="sxs-lookup"><span data-stu-id="58744-117">Properties</span></span>
| <span data-ttu-id="58744-118">属性</span><span class="sxs-lookup"><span data-stu-id="58744-118">Property</span></span>     | <span data-ttu-id="58744-119">类型</span><span class="sxs-lookup"><span data-stu-id="58744-119">Type</span></span>   |<span data-ttu-id="58744-120">说明</span><span class="sxs-lookup"><span data-stu-id="58744-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58744-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="58744-121">closedDateTime</span></span>|<span data-ttu-id="58744-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58744-122">dateTimeOffset</span></span>| <span data-ttu-id="58744-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="58744-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="58744-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58744-124">createdDateTime</span></span>|<span data-ttu-id="58744-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58744-125">dateTimeOffset</span></span>| <span data-ttu-id="58744-126">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="58744-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="58744-127">这始终大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="58744-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="58744-128">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="58744-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="58744-129">id</span><span class="sxs-lookup"><span data-stu-id="58744-129">id</span></span>|<span data-ttu-id="58744-130">string</span><span class="sxs-lookup"><span data-stu-id="58744-130">string</span></span>| <span data-ttu-id="58744-131">只读</span><span class="sxs-lookup"><span data-stu-id="58744-131">Read-only</span></span>|
|<span data-ttu-id="58744-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="58744-132">ipAddress</span></span>|<span data-ttu-id="58744-133">string</span><span class="sxs-lookup"><span data-stu-id="58744-133">string</span></span>| <span data-ttu-id="58744-134">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="58744-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="58744-135">location</span><span class="sxs-lookup"><span data-stu-id="58744-135">location</span></span>|<span data-ttu-id="58744-136">string</span><span class="sxs-lookup"><span data-stu-id="58744-136">string</span></span>| <span data-ttu-id="58744-137">附加到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="58744-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="58744-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="58744-138">riskEventDateTime</span></span>|<span data-ttu-id="58744-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58744-139">dateTimeOffset</span></span>| <span data-ttu-id="58744-140">发生风险事件的日期和时间</span><span class="sxs-lookup"><span data-stu-id="58744-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="58744-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="58744-141">riskEventStatus</span></span>|<span data-ttu-id="58744-142">string</span><span class="sxs-lookup"><span data-stu-id="58744-142">string</span></span>| <span data-ttu-id="58744-143">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="58744-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="58744-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="58744-144">riskLevel</span></span>|<span data-ttu-id="58744-145">string</span><span class="sxs-lookup"><span data-stu-id="58744-145">string</span></span>| <span data-ttu-id="58744-146">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="58744-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="58744-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="58744-147">riskEventType</span></span>|<span data-ttu-id="58744-148">string</span><span class="sxs-lookup"><span data-stu-id="58744-148">string</span></span>| <span data-ttu-id="58744-149">风险类型</span><span class="sxs-lookup"><span data-stu-id="58744-149">The type of risk</span></span>|
|<span data-ttu-id="58744-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="58744-150">userDisplayName</span></span>|<span data-ttu-id="58744-151">string</span><span class="sxs-lookup"><span data-stu-id="58744-151">string</span></span>| <span data-ttu-id="58744-152">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="58744-152">The name of the user at risk</span></span>|
|<span data-ttu-id="58744-153">userId</span><span class="sxs-lookup"><span data-stu-id="58744-153">userId</span></span>|<span data-ttu-id="58744-154">string</span><span class="sxs-lookup"><span data-stu-id="58744-154">string</span></span>| <span data-ttu-id="58744-155">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="58744-155">The id of the user at risk</span></span>|
|<span data-ttu-id="58744-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58744-156">userPrincipalName</span></span>|<span data-ttu-id="58744-157">string</span><span class="sxs-lookup"><span data-stu-id="58744-157">string</span></span>| <span data-ttu-id="58744-158">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="58744-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="58744-159">关系</span><span class="sxs-lookup"><span data-stu-id="58744-159">Relationships</span></span>
| <span data-ttu-id="58744-160">关系</span><span class="sxs-lookup"><span data-stu-id="58744-160">Relationship</span></span> | <span data-ttu-id="58744-161">类型</span><span class="sxs-lookup"><span data-stu-id="58744-161">Type</span></span>   |<span data-ttu-id="58744-162">说明</span><span class="sxs-lookup"><span data-stu-id="58744-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58744-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="58744-163">impactedUser</span></span>|[<span data-ttu-id="58744-164">user</span><span class="sxs-lookup"><span data-stu-id="58744-164">user</span></span>](user.md)| <span data-ttu-id="58744-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="58744-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58744-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58744-167">JSON representation</span></span>

<span data-ttu-id="58744-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58744-168">Here is a JSON representation of the resource.</span></span>

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
