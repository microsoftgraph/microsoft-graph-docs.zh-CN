---
title: leakedCredentialsRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的某个帐户凭据已在通配符中检测到的风险事件。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 750ee984ca1329b6abd4f21f9b0e10da5db14c6b
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312143"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="c5090-104">leakedCredentialsRiskEvent 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="c5090-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="c5090-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5090-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="c5090-106">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="c5090-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="c5090-107">有关详细信息，请参阅 [弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="c5090-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="c5090-108">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的某个帐户凭据已在通配符中检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="c5090-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="c5090-109">有关风险事件的完整信息，请参阅 [AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="c5090-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="c5090-110">方法</span><span class="sxs-lookup"><span data-stu-id="c5090-110">Methods</span></span>

| <span data-ttu-id="c5090-111">方法</span><span class="sxs-lookup"><span data-stu-id="c5090-111">Method</span></span>           | <span data-ttu-id="c5090-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5090-112">Return Type</span></span>    |<span data-ttu-id="c5090-113">说明</span><span class="sxs-lookup"><span data-stu-id="c5090-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5090-114">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c5090-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="c5090-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c5090-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="c5090-116">读取 leakedCredentialsRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5090-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5090-117">属性</span><span class="sxs-lookup"><span data-stu-id="c5090-117">Properties</span></span>
| <span data-ttu-id="c5090-118">属性</span><span class="sxs-lookup"><span data-stu-id="c5090-118">Property</span></span>     | <span data-ttu-id="c5090-119">类型</span><span class="sxs-lookup"><span data-stu-id="c5090-119">Type</span></span>   |<span data-ttu-id="c5090-120">说明</span><span class="sxs-lookup"><span data-stu-id="c5090-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5090-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5090-121">closedDateTime</span></span>|<span data-ttu-id="c5090-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5090-122">dateTimeOffset</span></span>| <span data-ttu-id="c5090-123">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c5090-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c5090-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5090-124">createdDateTime</span></span>|<span data-ttu-id="c5090-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5090-125">dateTimeOffset</span></span>| <span data-ttu-id="c5090-126">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c5090-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="c5090-127">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c5090-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c5090-128">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="c5090-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c5090-129">id</span><span class="sxs-lookup"><span data-stu-id="c5090-129">id</span></span>|<span data-ttu-id="c5090-130">string</span><span class="sxs-lookup"><span data-stu-id="c5090-130">string</span></span>| <span data-ttu-id="c5090-131">只读</span><span class="sxs-lookup"><span data-stu-id="c5090-131">Read-only</span></span>|
|<span data-ttu-id="c5090-132">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c5090-132">riskEventDateTime</span></span>|<span data-ttu-id="c5090-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5090-133">dateTimeOffset</span></span>| <span data-ttu-id="c5090-134">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c5090-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c5090-135">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c5090-135">riskEventStatus</span></span>|<span data-ttu-id="c5090-136">string</span><span class="sxs-lookup"><span data-stu-id="c5090-136">string</span></span>| <span data-ttu-id="c5090-137">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="c5090-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c5090-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c5090-138">riskLevel</span></span>|<span data-ttu-id="c5090-139">string</span><span class="sxs-lookup"><span data-stu-id="c5090-139">string</span></span>| <span data-ttu-id="c5090-140">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c5090-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c5090-141">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c5090-141">riskEventType</span></span>|<span data-ttu-id="c5090-142">string</span><span class="sxs-lookup"><span data-stu-id="c5090-142">string</span></span>| <span data-ttu-id="c5090-143">风险的类型</span><span class="sxs-lookup"><span data-stu-id="c5090-143">The type of risk</span></span>|
|<span data-ttu-id="c5090-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c5090-144">userDisplayName</span></span>|<span data-ttu-id="c5090-145">string</span><span class="sxs-lookup"><span data-stu-id="c5090-145">string</span></span>| <span data-ttu-id="c5090-146">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="c5090-146">The name of the user at risk</span></span>|
|<span data-ttu-id="c5090-147">userId</span><span class="sxs-lookup"><span data-stu-id="c5090-147">userId</span></span>|<span data-ttu-id="c5090-148">string</span><span class="sxs-lookup"><span data-stu-id="c5090-148">string</span></span>| <span data-ttu-id="c5090-149">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="c5090-149">The id of the user at risk</span></span>|
|<span data-ttu-id="c5090-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c5090-150">userPrincipalName</span></span>|<span data-ttu-id="c5090-151">string</span><span class="sxs-lookup"><span data-stu-id="c5090-151">string</span></span>| <span data-ttu-id="c5090-152">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c5090-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5090-153">关系</span><span class="sxs-lookup"><span data-stu-id="c5090-153">Relationships</span></span>
| <span data-ttu-id="c5090-154">关系</span><span class="sxs-lookup"><span data-stu-id="c5090-154">Relationship</span></span> | <span data-ttu-id="c5090-155">类型</span><span class="sxs-lookup"><span data-stu-id="c5090-155">Type</span></span>   |<span data-ttu-id="c5090-156">说明</span><span class="sxs-lookup"><span data-stu-id="c5090-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5090-157">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c5090-157">impactedUser</span></span>|[<span data-ttu-id="c5090-158">user</span><span class="sxs-lookup"><span data-stu-id="c5090-158">user</span></span>](user.md)| <span data-ttu-id="c5090-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="c5090-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5090-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5090-161">JSON representation</span></span>

<span data-ttu-id="c5090-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5090-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
