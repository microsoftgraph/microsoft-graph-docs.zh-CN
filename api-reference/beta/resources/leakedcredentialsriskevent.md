---
title: leakedCredentialsRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的某个帐户凭据已在通配符中检测到的风险事件。 有关风险事件的完整信息, 请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
ms.openlocfilehash: 1fbba14c25678b0e847c18648970a9fb551bee48
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345328"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="b05ab-104">leakedCredentialsRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b05ab-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b05ab-105">[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的某个帐户凭据已在通配符中检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="b05ab-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="b05ab-106">有关风险事件的完整信息, 请参阅[Azure AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="b05ab-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="b05ab-107">方法</span><span class="sxs-lookup"><span data-stu-id="b05ab-107">Methods</span></span>

| <span data-ttu-id="b05ab-108">方法</span><span class="sxs-lookup"><span data-stu-id="b05ab-108">Method</span></span>           | <span data-ttu-id="b05ab-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b05ab-109">Return Type</span></span>    |<span data-ttu-id="b05ab-110">说明</span><span class="sxs-lookup"><span data-stu-id="b05ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b05ab-111">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="b05ab-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="b05ab-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="b05ab-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="b05ab-113">读取 leakedCredentialsRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b05ab-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b05ab-114">属性</span><span class="sxs-lookup"><span data-stu-id="b05ab-114">Properties</span></span>
| <span data-ttu-id="b05ab-115">属性</span><span class="sxs-lookup"><span data-stu-id="b05ab-115">Property</span></span>     | <span data-ttu-id="b05ab-116">类型</span><span class="sxs-lookup"><span data-stu-id="b05ab-116">Type</span></span>   |<span data-ttu-id="b05ab-117">说明</span><span class="sxs-lookup"><span data-stu-id="b05ab-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b05ab-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="b05ab-118">closedDateTime</span></span>|<span data-ttu-id="b05ab-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b05ab-119">dateTimeOffset</span></span>| <span data-ttu-id="b05ab-120">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b05ab-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="b05ab-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b05ab-121">createdDateTime</span></span>|<span data-ttu-id="b05ab-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b05ab-122">dateTimeOffset</span></span>| <span data-ttu-id="b05ab-123">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b05ab-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="b05ab-124">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="b05ab-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="b05ab-125">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="b05ab-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="b05ab-126">id</span><span class="sxs-lookup"><span data-stu-id="b05ab-126">id</span></span>|<span data-ttu-id="b05ab-127">字符串</span><span class="sxs-lookup"><span data-stu-id="b05ab-127">string</span></span>| <span data-ttu-id="b05ab-128">只读</span><span class="sxs-lookup"><span data-stu-id="b05ab-128">Read-only</span></span>|
|<span data-ttu-id="b05ab-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="b05ab-129">riskEventDateTime</span></span>|<span data-ttu-id="b05ab-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b05ab-130">dateTimeOffset</span></span>| <span data-ttu-id="b05ab-131">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b05ab-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="b05ab-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="b05ab-132">riskEventStatus</span></span>|<span data-ttu-id="b05ab-133">string</span><span class="sxs-lookup"><span data-stu-id="b05ab-133">string</span></span>| <span data-ttu-id="b05ab-134">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="b05ab-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="b05ab-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b05ab-135">riskLevel</span></span>|<span data-ttu-id="b05ab-136">string</span><span class="sxs-lookup"><span data-stu-id="b05ab-136">string</span></span>| <span data-ttu-id="b05ab-137">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="b05ab-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="b05ab-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="b05ab-138">riskEventType</span></span>|<span data-ttu-id="b05ab-139">string</span><span class="sxs-lookup"><span data-stu-id="b05ab-139">string</span></span>| <span data-ttu-id="b05ab-140">风险的类型</span><span class="sxs-lookup"><span data-stu-id="b05ab-140">The type of risk</span></span>|
|<span data-ttu-id="b05ab-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b05ab-141">userDisplayName</span></span>|<span data-ttu-id="b05ab-142">string</span><span class="sxs-lookup"><span data-stu-id="b05ab-142">string</span></span>| <span data-ttu-id="b05ab-143">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="b05ab-143">The name of the user at risk</span></span>|
|<span data-ttu-id="b05ab-144">userId</span><span class="sxs-lookup"><span data-stu-id="b05ab-144">userId</span></span>|<span data-ttu-id="b05ab-145">string</span><span class="sxs-lookup"><span data-stu-id="b05ab-145">string</span></span>| <span data-ttu-id="b05ab-146">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="b05ab-146">The id of the user at risk</span></span>|
|<span data-ttu-id="b05ab-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b05ab-147">userPrincipalName</span></span>|<span data-ttu-id="b05ab-148">string</span><span class="sxs-lookup"><span data-stu-id="b05ab-148">string</span></span>| <span data-ttu-id="b05ab-149">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b05ab-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="b05ab-150">关系</span><span class="sxs-lookup"><span data-stu-id="b05ab-150">Relationships</span></span>
| <span data-ttu-id="b05ab-151">关系</span><span class="sxs-lookup"><span data-stu-id="b05ab-151">Relationship</span></span> | <span data-ttu-id="b05ab-152">类型</span><span class="sxs-lookup"><span data-stu-id="b05ab-152">Type</span></span>   |<span data-ttu-id="b05ab-153">说明</span><span class="sxs-lookup"><span data-stu-id="b05ab-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b05ab-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="b05ab-154">impactedUser</span></span>|[<span data-ttu-id="b05ab-155">用户</span><span class="sxs-lookup"><span data-stu-id="b05ab-155">user</span></span>](user.md)| <span data-ttu-id="b05ab-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="b05ab-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b05ab-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b05ab-158">JSON representation</span></span>

<span data-ttu-id="b05ab-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b05ab-159">Here is a JSON representation of the resource.</span></span>

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
