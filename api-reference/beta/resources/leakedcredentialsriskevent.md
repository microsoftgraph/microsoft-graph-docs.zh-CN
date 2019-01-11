---
title: leakedCredentialsRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护其中已帐户的凭据检测到的风险事件。 Azure AD 身份保护文档中，可以找到有关风险事件的完整信息。
localization_priority: Normal
ms.openlocfilehash: 7a8f2a8cf72b713fab30887fcc4d81b8a88e71ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815979"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="556ca-104">leakedCredentialsRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="556ca-104">leakedCredentialsRiskEvent resource type</span></span>

> <span data-ttu-id="556ca-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="556ca-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="556ca-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="556ca-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="556ca-107">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中已帐户的凭据检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="556ca-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="556ca-108">[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="556ca-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="556ca-109">方法</span><span class="sxs-lookup"><span data-stu-id="556ca-109">Methods</span></span>

| <span data-ttu-id="556ca-110">方法</span><span class="sxs-lookup"><span data-stu-id="556ca-110">Method</span></span>           | <span data-ttu-id="556ca-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="556ca-111">Return Type</span></span>    |<span data-ttu-id="556ca-112">说明</span><span class="sxs-lookup"><span data-stu-id="556ca-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="556ca-113">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="556ca-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="556ca-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="556ca-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="556ca-115">读取属性和 leakedCredentialsRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="556ca-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="556ca-116">属性</span><span class="sxs-lookup"><span data-stu-id="556ca-116">Properties</span></span>
| <span data-ttu-id="556ca-117">属性</span><span class="sxs-lookup"><span data-stu-id="556ca-117">Property</span></span>     | <span data-ttu-id="556ca-118">类型</span><span class="sxs-lookup"><span data-stu-id="556ca-118">Type</span></span>   |<span data-ttu-id="556ca-119">Description</span><span class="sxs-lookup"><span data-stu-id="556ca-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="556ca-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="556ca-120">closedDateTime</span></span>|<span data-ttu-id="556ca-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="556ca-121">dateTimeOffset</span></span>| <span data-ttu-id="556ca-122">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="556ca-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="556ca-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="556ca-123">createdDateTime</span></span>|<span data-ttu-id="556ca-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="556ca-124">dateTimeOffset</span></span>| <span data-ttu-id="556ca-125">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="556ca-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="556ca-126">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="556ca-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="556ca-127">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="556ca-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="556ca-128">id</span><span class="sxs-lookup"><span data-stu-id="556ca-128">id</span></span>|<span data-ttu-id="556ca-129">string</span><span class="sxs-lookup"><span data-stu-id="556ca-129">string</span></span>| <span data-ttu-id="556ca-130">只读</span><span class="sxs-lookup"><span data-stu-id="556ca-130">Read-only</span></span>|
|<span data-ttu-id="556ca-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="556ca-131">riskEventDateTime</span></span>|<span data-ttu-id="556ca-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="556ca-132">dateTimeOffset</span></span>| <span data-ttu-id="556ca-133">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="556ca-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="556ca-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="556ca-134">riskEventStatus</span></span>|<span data-ttu-id="556ca-135">string</span><span class="sxs-lookup"><span data-stu-id="556ca-135">string</span></span>| <span data-ttu-id="556ca-136">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="556ca-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="556ca-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="556ca-137">riskLevel</span></span>|<span data-ttu-id="556ca-138">string</span><span class="sxs-lookup"><span data-stu-id="556ca-138">string</span></span>| <span data-ttu-id="556ca-139">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="556ca-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="556ca-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="556ca-140">riskEventType</span></span>|<span data-ttu-id="556ca-141">string</span><span class="sxs-lookup"><span data-stu-id="556ca-141">string</span></span>| <span data-ttu-id="556ca-142">风险类型</span><span class="sxs-lookup"><span data-stu-id="556ca-142">The type of risk</span></span>|
|<span data-ttu-id="556ca-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="556ca-143">userDisplayName</span></span>|<span data-ttu-id="556ca-144">string</span><span class="sxs-lookup"><span data-stu-id="556ca-144">string</span></span>| <span data-ttu-id="556ca-145">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="556ca-145">The name of the user at risk</span></span>|
|<span data-ttu-id="556ca-146">userId</span><span class="sxs-lookup"><span data-stu-id="556ca-146">userId</span></span>|<span data-ttu-id="556ca-147">string</span><span class="sxs-lookup"><span data-stu-id="556ca-147">string</span></span>| <span data-ttu-id="556ca-148">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="556ca-148">The id of the user at risk</span></span>|
|<span data-ttu-id="556ca-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="556ca-149">userPrincipalName</span></span>|<span data-ttu-id="556ca-150">string</span><span class="sxs-lookup"><span data-stu-id="556ca-150">string</span></span>| <span data-ttu-id="556ca-151">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="556ca-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="556ca-152">Relationships</span><span class="sxs-lookup"><span data-stu-id="556ca-152">Relationships</span></span>
| <span data-ttu-id="556ca-153">关系</span><span class="sxs-lookup"><span data-stu-id="556ca-153">Relationship</span></span> | <span data-ttu-id="556ca-154">类型</span><span class="sxs-lookup"><span data-stu-id="556ca-154">Type</span></span>   |<span data-ttu-id="556ca-155">Description</span><span class="sxs-lookup"><span data-stu-id="556ca-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="556ca-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="556ca-156">impactedUser</span></span>|[<span data-ttu-id="556ca-157">用户</span><span class="sxs-lookup"><span data-stu-id="556ca-157">user</span></span>](user.md)| <span data-ttu-id="556ca-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="556ca-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="556ca-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="556ca-160">JSON representation</span></span>

<span data-ttu-id="556ca-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="556ca-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
