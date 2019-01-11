---
title: unfamiliarLocationRiskEvent 资源类型
description: 风险事件检测到的 Azure Active Directory 标识保护其中帐户登录尝试从用户的新位置。 Azure AD 身份保护文档中，可以找到有关风险事件的完整信息。
localization_priority: Normal
ms.openlocfilehash: 130d68bfb23bdb23b6a9de81fa988d38db1d8c10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868738"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="e863d-104">unfamiliarLocationRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e863d-104">unfamiliarLocationRiskEvent resource type</span></span>

> <span data-ttu-id="e863d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e863d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e863d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e863d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e863d-107">风险事件检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中帐户登录尝试从用户的新位置。</span><span class="sxs-lookup"><span data-stu-id="e863d-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="e863d-108">[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="e863d-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="e863d-109">方法</span><span class="sxs-lookup"><span data-stu-id="e863d-109">Methods</span></span>

| <span data-ttu-id="e863d-110">方法</span><span class="sxs-lookup"><span data-stu-id="e863d-110">Method</span></span>           | <span data-ttu-id="e863d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e863d-111">Return Type</span></span>    |<span data-ttu-id="e863d-112">说明</span><span class="sxs-lookup"><span data-stu-id="e863d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e863d-113">获取 unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e863d-113">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="e863d-114">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e863d-114">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="e863d-115">读取属性和 unfamiliarLocationRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e863d-115">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e863d-116">属性</span><span class="sxs-lookup"><span data-stu-id="e863d-116">Properties</span></span>
| <span data-ttu-id="e863d-117">属性</span><span class="sxs-lookup"><span data-stu-id="e863d-117">Property</span></span>     | <span data-ttu-id="e863d-118">类型</span><span class="sxs-lookup"><span data-stu-id="e863d-118">Type</span></span>   |<span data-ttu-id="e863d-119">Description</span><span class="sxs-lookup"><span data-stu-id="e863d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e863d-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e863d-120">closedDateTime</span></span>|<span data-ttu-id="e863d-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e863d-121">dateTimeOffset</span></span>| <span data-ttu-id="e863d-122">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="e863d-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e863d-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e863d-123">createdDateTime</span></span>|<span data-ttu-id="e863d-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e863d-124">dateTimeOffset</span></span>| <span data-ttu-id="e863d-125">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="e863d-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="e863d-126">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="e863d-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e863d-127">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="e863d-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e863d-128">id</span><span class="sxs-lookup"><span data-stu-id="e863d-128">id</span></span>|<span data-ttu-id="e863d-129">string</span><span class="sxs-lookup"><span data-stu-id="e863d-129">string</span></span>| <span data-ttu-id="e863d-130">只读</span><span class="sxs-lookup"><span data-stu-id="e863d-130">Read-only</span></span>|
|<span data-ttu-id="e863d-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e863d-131">ipAddress</span></span>|<span data-ttu-id="e863d-132">string</span><span class="sxs-lookup"><span data-stu-id="e863d-132">string</span></span>| <span data-ttu-id="e863d-133">登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="e863d-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="e863d-134">location</span><span class="sxs-lookup"><span data-stu-id="e863d-134">location</span></span>|<span data-ttu-id="e863d-135">string</span><span class="sxs-lookup"><span data-stu-id="e863d-135">string</span></span>| <span data-ttu-id="e863d-136">挂接到登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="e863d-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="e863d-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e863d-137">riskEventDateTime</span></span>|<span data-ttu-id="e863d-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e863d-138">dateTimeOffset</span></span>| <span data-ttu-id="e863d-139">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="e863d-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e863d-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e863d-140">riskEventStatus</span></span>|<span data-ttu-id="e863d-141">string</span><span class="sxs-lookup"><span data-stu-id="e863d-141">string</span></span>| <span data-ttu-id="e863d-142">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="e863d-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e863d-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e863d-143">riskLevel</span></span>|<span data-ttu-id="e863d-144">string</span><span class="sxs-lookup"><span data-stu-id="e863d-144">string</span></span>| <span data-ttu-id="e863d-145">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e863d-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e863d-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e863d-146">riskEventType</span></span>|<span data-ttu-id="e863d-147">string</span><span class="sxs-lookup"><span data-stu-id="e863d-147">string</span></span>| <span data-ttu-id="e863d-148">风险类型</span><span class="sxs-lookup"><span data-stu-id="e863d-148">The type of risk</span></span>|
|<span data-ttu-id="e863d-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e863d-149">userDisplayName</span></span>|<span data-ttu-id="e863d-150">string</span><span class="sxs-lookup"><span data-stu-id="e863d-150">string</span></span>| <span data-ttu-id="e863d-151">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="e863d-151">The name of the user at risk</span></span>|
|<span data-ttu-id="e863d-152">userId</span><span class="sxs-lookup"><span data-stu-id="e863d-152">userId</span></span>|<span data-ttu-id="e863d-153">string</span><span class="sxs-lookup"><span data-stu-id="e863d-153">string</span></span>| <span data-ttu-id="e863d-154">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="e863d-154">The id of the user at risk</span></span>|
|<span data-ttu-id="e863d-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e863d-155">userPrincipalName</span></span>|<span data-ttu-id="e863d-156">string</span><span class="sxs-lookup"><span data-stu-id="e863d-156">string</span></span>| <span data-ttu-id="e863d-157">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e863d-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e863d-158">Relationships</span><span class="sxs-lookup"><span data-stu-id="e863d-158">Relationships</span></span>
| <span data-ttu-id="e863d-159">关系</span><span class="sxs-lookup"><span data-stu-id="e863d-159">Relationship</span></span> | <span data-ttu-id="e863d-160">类型</span><span class="sxs-lookup"><span data-stu-id="e863d-160">Type</span></span>   |<span data-ttu-id="e863d-161">Description</span><span class="sxs-lookup"><span data-stu-id="e863d-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e863d-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e863d-162">impactedUser</span></span>|[<span data-ttu-id="e863d-163">用户</span><span class="sxs-lookup"><span data-stu-id="e863d-163">user</span></span>](user.md)| <span data-ttu-id="e863d-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e863d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e863d-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e863d-166">JSON representation</span></span>

<span data-ttu-id="e863d-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e863d-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
