---
title: unfamiliarLocationRiskEvent 资源类型
description: Azure Active Directory Identity Protection 检测到的风险事件，其中帐户从该用户的新位置尝试登录。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: e2d34106de3e0b72303f103edcc6a798b5790b47
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442724"
---
# <a name="unfamiliarlocationriskevent-resource-type-deprecated"></a><span data-ttu-id="c679a-104">已弃 (的 unfamiliarLocationRiskEvent 资源) </span><span class="sxs-lookup"><span data-stu-id="c679a-104">unfamiliarLocationRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="c679a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c679a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="c679a-106">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="c679a-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="c679a-107">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="c679a-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="c679a-108">Azure [Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) 检测到的风险事件，其中帐户从该用户的新位置尝试登录。</span><span class="sxs-lookup"><span data-stu-id="c679a-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="c679a-109">有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="c679a-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="c679a-110">Methods</span><span class="sxs-lookup"><span data-stu-id="c679a-110">Methods</span></span>

| <span data-ttu-id="c679a-111">方法</span><span class="sxs-lookup"><span data-stu-id="c679a-111">Method</span></span>           | <span data-ttu-id="c679a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c679a-112">Return Type</span></span>    |<span data-ttu-id="c679a-113">说明</span><span class="sxs-lookup"><span data-stu-id="c679a-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c679a-114">获取 unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c679a-114">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="c679a-115">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c679a-115">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="c679a-116">读取 unfamiliarLocationRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c679a-116">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c679a-117">属性</span><span class="sxs-lookup"><span data-stu-id="c679a-117">Properties</span></span>
| <span data-ttu-id="c679a-118">属性</span><span class="sxs-lookup"><span data-stu-id="c679a-118">Property</span></span>     | <span data-ttu-id="c679a-119">类型</span><span class="sxs-lookup"><span data-stu-id="c679a-119">Type</span></span>   |<span data-ttu-id="c679a-120">说明</span><span class="sxs-lookup"><span data-stu-id="c679a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c679a-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c679a-121">closedDateTime</span></span>|<span data-ttu-id="c679a-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c679a-122">dateTimeOffset</span></span>| <span data-ttu-id="c679a-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c679a-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c679a-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c679a-124">createdDateTime</span></span>|<span data-ttu-id="c679a-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c679a-125">dateTimeOffset</span></span>| <span data-ttu-id="c679a-126">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c679a-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="c679a-127">这始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c679a-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c679a-128">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="c679a-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c679a-129">id</span><span class="sxs-lookup"><span data-stu-id="c679a-129">id</span></span>|<span data-ttu-id="c679a-130">string</span><span class="sxs-lookup"><span data-stu-id="c679a-130">string</span></span>| <span data-ttu-id="c679a-131">只读</span><span class="sxs-lookup"><span data-stu-id="c679a-131">Read-only</span></span>|
|<span data-ttu-id="c679a-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c679a-132">ipAddress</span></span>|<span data-ttu-id="c679a-133">string</span><span class="sxs-lookup"><span data-stu-id="c679a-133">string</span></span>| <span data-ttu-id="c679a-134">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="c679a-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="c679a-135">location</span><span class="sxs-lookup"><span data-stu-id="c679a-135">location</span></span>|<span data-ttu-id="c679a-136">string</span><span class="sxs-lookup"><span data-stu-id="c679a-136">string</span></span>| <span data-ttu-id="c679a-137">附加到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="c679a-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="c679a-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c679a-138">riskEventDateTime</span></span>|<span data-ttu-id="c679a-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c679a-139">dateTimeOffset</span></span>| <span data-ttu-id="c679a-140">发生风险事件的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c679a-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c679a-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c679a-141">riskEventStatus</span></span>|<span data-ttu-id="c679a-142">string</span><span class="sxs-lookup"><span data-stu-id="c679a-142">string</span></span>| <span data-ttu-id="c679a-143">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="c679a-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c679a-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c679a-144">riskLevel</span></span>|<span data-ttu-id="c679a-145">string</span><span class="sxs-lookup"><span data-stu-id="c679a-145">string</span></span>| <span data-ttu-id="c679a-146">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c679a-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c679a-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c679a-147">riskEventType</span></span>|<span data-ttu-id="c679a-148">string</span><span class="sxs-lookup"><span data-stu-id="c679a-148">string</span></span>| <span data-ttu-id="c679a-149">风险类型</span><span class="sxs-lookup"><span data-stu-id="c679a-149">The type of risk</span></span>|
|<span data-ttu-id="c679a-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c679a-150">userDisplayName</span></span>|<span data-ttu-id="c679a-151">string</span><span class="sxs-lookup"><span data-stu-id="c679a-151">string</span></span>| <span data-ttu-id="c679a-152">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="c679a-152">The name of the user at risk</span></span>|
|<span data-ttu-id="c679a-153">userId</span><span class="sxs-lookup"><span data-stu-id="c679a-153">userId</span></span>|<span data-ttu-id="c679a-154">string</span><span class="sxs-lookup"><span data-stu-id="c679a-154">string</span></span>| <span data-ttu-id="c679a-155">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="c679a-155">The id of the user at risk</span></span>|
|<span data-ttu-id="c679a-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c679a-156">userPrincipalName</span></span>|<span data-ttu-id="c679a-157">string</span><span class="sxs-lookup"><span data-stu-id="c679a-157">string</span></span>| <span data-ttu-id="c679a-158">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c679a-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c679a-159">关系</span><span class="sxs-lookup"><span data-stu-id="c679a-159">Relationships</span></span>
| <span data-ttu-id="c679a-160">关系</span><span class="sxs-lookup"><span data-stu-id="c679a-160">Relationship</span></span> | <span data-ttu-id="c679a-161">类型</span><span class="sxs-lookup"><span data-stu-id="c679a-161">Type</span></span>   |<span data-ttu-id="c679a-162">说明</span><span class="sxs-lookup"><span data-stu-id="c679a-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c679a-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c679a-163">impactedUser</span></span>|[<span data-ttu-id="c679a-164">user</span><span class="sxs-lookup"><span data-stu-id="c679a-164">user</span></span>](user.md)| <span data-ttu-id="c679a-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="c679a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c679a-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c679a-167">JSON representation</span></span>

<span data-ttu-id="c679a-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c679a-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
