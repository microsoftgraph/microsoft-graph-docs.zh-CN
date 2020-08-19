---
title: anonymousIpRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的一个风险事件，其中的帐户登录尝试来自看似匿名的 IP 地址。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 41d4109cb14053621baebd8383c522ad7e0ae3c0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807562"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="537e9-104">anonymousIpRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="537e9-104">anonymousIpRiskEvent resource type</span></span>

<span data-ttu-id="537e9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="537e9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="537e9-106">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="537e9-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="537e9-107">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="537e9-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="537e9-108">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的一个风险事件，其中的帐户登录尝试来自看似匿名的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="537e9-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="537e9-109">有关风险事件的完整信息，请参阅 [AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="537e9-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="537e9-110">方法</span><span class="sxs-lookup"><span data-stu-id="537e9-110">Methods</span></span>

| <span data-ttu-id="537e9-111">方法</span><span class="sxs-lookup"><span data-stu-id="537e9-111">Method</span></span>           | <span data-ttu-id="537e9-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="537e9-112">Return Type</span></span>    |<span data-ttu-id="537e9-113">说明</span><span class="sxs-lookup"><span data-stu-id="537e9-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="537e9-114">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="537e9-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="537e9-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="537e9-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="537e9-116">读取 anonymousIpRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="537e9-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="537e9-117">属性</span><span class="sxs-lookup"><span data-stu-id="537e9-117">Properties</span></span>
| <span data-ttu-id="537e9-118">属性</span><span class="sxs-lookup"><span data-stu-id="537e9-118">Property</span></span>     | <span data-ttu-id="537e9-119">类型</span><span class="sxs-lookup"><span data-stu-id="537e9-119">Type</span></span>   |<span data-ttu-id="537e9-120">说明</span><span class="sxs-lookup"><span data-stu-id="537e9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="537e9-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="537e9-121">closedDateTime</span></span>|<span data-ttu-id="537e9-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537e9-122">dateTimeOffset</span></span>| <span data-ttu-id="537e9-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="537e9-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="537e9-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="537e9-124">createdDateTime</span></span>|<span data-ttu-id="537e9-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537e9-125">dateTimeOffset</span></span>| <span data-ttu-id="537e9-126">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="537e9-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="537e9-127">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="537e9-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="537e9-128">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="537e9-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="537e9-129">id</span><span class="sxs-lookup"><span data-stu-id="537e9-129">id</span></span>|<span data-ttu-id="537e9-130">string</span><span class="sxs-lookup"><span data-stu-id="537e9-130">string</span></span>| <span data-ttu-id="537e9-131">只读</span><span class="sxs-lookup"><span data-stu-id="537e9-131">Read-only</span></span>|
|<span data-ttu-id="537e9-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="537e9-132">ipAddress</span></span>|<span data-ttu-id="537e9-133">string</span><span class="sxs-lookup"><span data-stu-id="537e9-133">string</span></span>| <span data-ttu-id="537e9-134">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="537e9-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="537e9-135">location</span><span class="sxs-lookup"><span data-stu-id="537e9-135">location</span></span>|<span data-ttu-id="537e9-136">string</span><span class="sxs-lookup"><span data-stu-id="537e9-136">string</span></span>| <span data-ttu-id="537e9-137">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="537e9-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="537e9-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="537e9-138">riskEventDateTime</span></span>|<span data-ttu-id="537e9-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537e9-139">dateTimeOffset</span></span>| <span data-ttu-id="537e9-140">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="537e9-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="537e9-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="537e9-141">riskEventStatus</span></span>|<span data-ttu-id="537e9-142">string</span><span class="sxs-lookup"><span data-stu-id="537e9-142">string</span></span>| <span data-ttu-id="537e9-143">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="537e9-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="537e9-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="537e9-144">riskLevel</span></span>|<span data-ttu-id="537e9-145">string</span><span class="sxs-lookup"><span data-stu-id="537e9-145">string</span></span>| <span data-ttu-id="537e9-146">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="537e9-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="537e9-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="537e9-147">riskEventType</span></span>|<span data-ttu-id="537e9-148">string</span><span class="sxs-lookup"><span data-stu-id="537e9-148">string</span></span>| <span data-ttu-id="537e9-149">风险的类型</span><span class="sxs-lookup"><span data-stu-id="537e9-149">The type of risk</span></span>|
|<span data-ttu-id="537e9-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="537e9-150">userDisplayName</span></span>|<span data-ttu-id="537e9-151">string</span><span class="sxs-lookup"><span data-stu-id="537e9-151">string</span></span>| <span data-ttu-id="537e9-152">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="537e9-152">The name of the user at risk</span></span>|
|<span data-ttu-id="537e9-153">userId</span><span class="sxs-lookup"><span data-stu-id="537e9-153">userId</span></span>|<span data-ttu-id="537e9-154">string</span><span class="sxs-lookup"><span data-stu-id="537e9-154">string</span></span>| <span data-ttu-id="537e9-155">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="537e9-155">The id of the user at risk</span></span>|
|<span data-ttu-id="537e9-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="537e9-156">userPrincipalName</span></span>|<span data-ttu-id="537e9-157">string</span><span class="sxs-lookup"><span data-stu-id="537e9-157">string</span></span>| <span data-ttu-id="537e9-158">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="537e9-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="537e9-159">关系</span><span class="sxs-lookup"><span data-stu-id="537e9-159">Relationships</span></span>
| <span data-ttu-id="537e9-160">关系</span><span class="sxs-lookup"><span data-stu-id="537e9-160">Relationship</span></span> | <span data-ttu-id="537e9-161">类型</span><span class="sxs-lookup"><span data-stu-id="537e9-161">Type</span></span>   |<span data-ttu-id="537e9-162">说明</span><span class="sxs-lookup"><span data-stu-id="537e9-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="537e9-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="537e9-163">impactedUser</span></span>|[<span data-ttu-id="537e9-164">user</span><span class="sxs-lookup"><span data-stu-id="537e9-164">user</span></span>](user.md)| <span data-ttu-id="537e9-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="537e9-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="537e9-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="537e9-167">JSON representation</span></span>

<span data-ttu-id="537e9-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="537e9-168">Here is a JSON representation of the resource.</span></span>

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
