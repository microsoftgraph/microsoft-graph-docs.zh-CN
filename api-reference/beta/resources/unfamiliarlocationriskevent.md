---
title: unfamiliarLocationRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的一个风险事件，其中的帐户登录尝试来自该用户的新位置。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 72a114fb42d24bd61aef3bff5cd3fba8d2de93a0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866509"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="f45cc-104">unfamiliarLocationRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="f45cc-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="f45cc-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="f45cc-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="f45cc-106">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="f45cc-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="f45cc-107">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的一个风险事件，其中的帐户登录尝试来自该用户的新位置。</span><span class="sxs-lookup"><span data-stu-id="f45cc-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="f45cc-108">有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="f45cc-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="f45cc-109">方法</span><span class="sxs-lookup"><span data-stu-id="f45cc-109">Methods</span></span>

| <span data-ttu-id="f45cc-110">方法</span><span class="sxs-lookup"><span data-stu-id="f45cc-110">Method</span></span>           | <span data-ttu-id="f45cc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f45cc-111">Return Type</span></span>    |<span data-ttu-id="f45cc-112">说明</span><span class="sxs-lookup"><span data-stu-id="f45cc-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f45cc-113">获取 unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f45cc-113">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="f45cc-114">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f45cc-114">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="f45cc-115">读取 unfamiliarLocationRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f45cc-115">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f45cc-116">属性</span><span class="sxs-lookup"><span data-stu-id="f45cc-116">Properties</span></span>
| <span data-ttu-id="f45cc-117">属性</span><span class="sxs-lookup"><span data-stu-id="f45cc-117">Property</span></span>     | <span data-ttu-id="f45cc-118">类型</span><span class="sxs-lookup"><span data-stu-id="f45cc-118">Type</span></span>   |<span data-ttu-id="f45cc-119">说明</span><span class="sxs-lookup"><span data-stu-id="f45cc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f45cc-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f45cc-120">closedDateTime</span></span>|<span data-ttu-id="f45cc-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45cc-121">dateTimeOffset</span></span>| <span data-ttu-id="f45cc-122">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="f45cc-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f45cc-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f45cc-123">createdDateTime</span></span>|<span data-ttu-id="f45cc-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45cc-124">dateTimeOffset</span></span>| <span data-ttu-id="f45cc-125">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f45cc-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="f45cc-126">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="f45cc-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f45cc-127">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="f45cc-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f45cc-128">id</span><span class="sxs-lookup"><span data-stu-id="f45cc-128">id</span></span>|<span data-ttu-id="f45cc-129">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-129">string</span></span>| <span data-ttu-id="f45cc-130">只读</span><span class="sxs-lookup"><span data-stu-id="f45cc-130">Read-only</span></span>|
|<span data-ttu-id="f45cc-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f45cc-131">ipAddress</span></span>|<span data-ttu-id="f45cc-132">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-132">string</span></span>| <span data-ttu-id="f45cc-133">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="f45cc-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="f45cc-134">location</span><span class="sxs-lookup"><span data-stu-id="f45cc-134">location</span></span>|<span data-ttu-id="f45cc-135">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-135">string</span></span>| <span data-ttu-id="f45cc-136">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="f45cc-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="f45cc-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f45cc-137">riskEventDateTime</span></span>|<span data-ttu-id="f45cc-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45cc-138">dateTimeOffset</span></span>| <span data-ttu-id="f45cc-139">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="f45cc-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f45cc-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f45cc-140">riskEventStatus</span></span>|<span data-ttu-id="f45cc-141">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-141">string</span></span>| <span data-ttu-id="f45cc-142">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="f45cc-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f45cc-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f45cc-143">riskLevel</span></span>|<span data-ttu-id="f45cc-144">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-144">string</span></span>| <span data-ttu-id="f45cc-145">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f45cc-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f45cc-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f45cc-146">riskEventType</span></span>|<span data-ttu-id="f45cc-147">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-147">string</span></span>| <span data-ttu-id="f45cc-148">风险的类型</span><span class="sxs-lookup"><span data-stu-id="f45cc-148">The type of risk</span></span>|
|<span data-ttu-id="f45cc-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f45cc-149">userDisplayName</span></span>|<span data-ttu-id="f45cc-150">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-150">string</span></span>| <span data-ttu-id="f45cc-151">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="f45cc-151">The name of the user at risk</span></span>|
|<span data-ttu-id="f45cc-152">userId</span><span class="sxs-lookup"><span data-stu-id="f45cc-152">userId</span></span>|<span data-ttu-id="f45cc-153">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-153">string</span></span>| <span data-ttu-id="f45cc-154">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="f45cc-154">The id of the user at risk</span></span>|
|<span data-ttu-id="f45cc-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f45cc-155">userPrincipalName</span></span>|<span data-ttu-id="f45cc-156">string</span><span class="sxs-lookup"><span data-stu-id="f45cc-156">string</span></span>| <span data-ttu-id="f45cc-157">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f45cc-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f45cc-158">关系</span><span class="sxs-lookup"><span data-stu-id="f45cc-158">Relationships</span></span>
| <span data-ttu-id="f45cc-159">关系</span><span class="sxs-lookup"><span data-stu-id="f45cc-159">Relationship</span></span> | <span data-ttu-id="f45cc-160">类型</span><span class="sxs-lookup"><span data-stu-id="f45cc-160">Type</span></span>   |<span data-ttu-id="f45cc-161">说明</span><span class="sxs-lookup"><span data-stu-id="f45cc-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f45cc-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f45cc-162">impactedUser</span></span>|[<span data-ttu-id="f45cc-163">user</span><span class="sxs-lookup"><span data-stu-id="f45cc-163">user</span></span>](user.md)| <span data-ttu-id="f45cc-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="f45cc-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f45cc-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f45cc-166">JSON representation</span></span>

<span data-ttu-id="f45cc-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f45cc-167">Here is a JSON representation of the resource.</span></span>

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
