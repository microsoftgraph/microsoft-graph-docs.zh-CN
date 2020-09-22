---
title: unfamiliarLocationRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的一个风险事件，其中的帐户登录尝试来自该用户的新位置。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: ec1b9a0921326f9ebd8ff6f72b9ec584b1080462
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075395"
---
# <a name="unfamiliarlocationriskevent-resource-type-deprecated"></a><span data-ttu-id="bf868-104">unfamiliarLocationRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="bf868-104">unfamiliarLocationRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="bf868-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf868-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="bf868-106">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="bf868-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="bf868-107">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="bf868-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="bf868-108">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的一个风险事件，其中的帐户登录尝试来自该用户的新位置。</span><span class="sxs-lookup"><span data-stu-id="bf868-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="bf868-109">有关风险事件的完整信息，请参阅 [AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="bf868-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="bf868-110">方法</span><span class="sxs-lookup"><span data-stu-id="bf868-110">Methods</span></span>

| <span data-ttu-id="bf868-111">方法</span><span class="sxs-lookup"><span data-stu-id="bf868-111">Method</span></span>           | <span data-ttu-id="bf868-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf868-112">Return Type</span></span>    |<span data-ttu-id="bf868-113">说明</span><span class="sxs-lookup"><span data-stu-id="bf868-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf868-114">获取 unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="bf868-114">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="bf868-115">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="bf868-115">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="bf868-116">读取 unfamiliarLocationRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf868-116">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf868-117">属性</span><span class="sxs-lookup"><span data-stu-id="bf868-117">Properties</span></span>
| <span data-ttu-id="bf868-118">属性</span><span class="sxs-lookup"><span data-stu-id="bf868-118">Property</span></span>     | <span data-ttu-id="bf868-119">类型</span><span class="sxs-lookup"><span data-stu-id="bf868-119">Type</span></span>   |<span data-ttu-id="bf868-120">说明</span><span class="sxs-lookup"><span data-stu-id="bf868-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf868-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf868-121">closedDateTime</span></span>|<span data-ttu-id="bf868-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf868-122">dateTimeOffset</span></span>| <span data-ttu-id="bf868-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="bf868-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="bf868-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf868-124">createdDateTime</span></span>|<span data-ttu-id="bf868-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf868-125">dateTimeOffset</span></span>| <span data-ttu-id="bf868-126">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bf868-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="bf868-127">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="bf868-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="bf868-128">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="bf868-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="bf868-129">id</span><span class="sxs-lookup"><span data-stu-id="bf868-129">id</span></span>|<span data-ttu-id="bf868-130">string</span><span class="sxs-lookup"><span data-stu-id="bf868-130">string</span></span>| <span data-ttu-id="bf868-131">只读</span><span class="sxs-lookup"><span data-stu-id="bf868-131">Read-only</span></span>|
|<span data-ttu-id="bf868-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="bf868-132">ipAddress</span></span>|<span data-ttu-id="bf868-133">string</span><span class="sxs-lookup"><span data-stu-id="bf868-133">string</span></span>| <span data-ttu-id="bf868-134">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="bf868-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="bf868-135">location</span><span class="sxs-lookup"><span data-stu-id="bf868-135">location</span></span>|<span data-ttu-id="bf868-136">string</span><span class="sxs-lookup"><span data-stu-id="bf868-136">string</span></span>| <span data-ttu-id="bf868-137">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="bf868-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="bf868-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="bf868-138">riskEventDateTime</span></span>|<span data-ttu-id="bf868-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf868-139">dateTimeOffset</span></span>| <span data-ttu-id="bf868-140">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="bf868-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="bf868-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="bf868-141">riskEventStatus</span></span>|<span data-ttu-id="bf868-142">string</span><span class="sxs-lookup"><span data-stu-id="bf868-142">string</span></span>| <span data-ttu-id="bf868-143">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="bf868-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="bf868-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="bf868-144">riskLevel</span></span>|<span data-ttu-id="bf868-145">string</span><span class="sxs-lookup"><span data-stu-id="bf868-145">string</span></span>| <span data-ttu-id="bf868-146">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="bf868-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="bf868-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="bf868-147">riskEventType</span></span>|<span data-ttu-id="bf868-148">string</span><span class="sxs-lookup"><span data-stu-id="bf868-148">string</span></span>| <span data-ttu-id="bf868-149">风险的类型</span><span class="sxs-lookup"><span data-stu-id="bf868-149">The type of risk</span></span>|
|<span data-ttu-id="bf868-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf868-150">userDisplayName</span></span>|<span data-ttu-id="bf868-151">string</span><span class="sxs-lookup"><span data-stu-id="bf868-151">string</span></span>| <span data-ttu-id="bf868-152">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="bf868-152">The name of the user at risk</span></span>|
|<span data-ttu-id="bf868-153">userId</span><span class="sxs-lookup"><span data-stu-id="bf868-153">userId</span></span>|<span data-ttu-id="bf868-154">string</span><span class="sxs-lookup"><span data-stu-id="bf868-154">string</span></span>| <span data-ttu-id="bf868-155">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="bf868-155">The id of the user at risk</span></span>|
|<span data-ttu-id="bf868-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bf868-156">userPrincipalName</span></span>|<span data-ttu-id="bf868-157">string</span><span class="sxs-lookup"><span data-stu-id="bf868-157">string</span></span>| <span data-ttu-id="bf868-158">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="bf868-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf868-159">关系</span><span class="sxs-lookup"><span data-stu-id="bf868-159">Relationships</span></span>
| <span data-ttu-id="bf868-160">关系</span><span class="sxs-lookup"><span data-stu-id="bf868-160">Relationship</span></span> | <span data-ttu-id="bf868-161">类型</span><span class="sxs-lookup"><span data-stu-id="bf868-161">Type</span></span>   |<span data-ttu-id="bf868-162">说明</span><span class="sxs-lookup"><span data-stu-id="bf868-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf868-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="bf868-163">impactedUser</span></span>|[<span data-ttu-id="bf868-164">user</span><span class="sxs-lookup"><span data-stu-id="bf868-164">user</span></span>](user.md)| <span data-ttu-id="bf868-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="bf868-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf868-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf868-167">JSON representation</span></span>

<span data-ttu-id="bf868-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf868-168">Here is a JSON representation of the resource.</span></span>

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


