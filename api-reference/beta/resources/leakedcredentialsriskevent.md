---
title: leakedCredentialsRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的某个帐户凭据已在通配符中检测到的风险事件。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4f12131d1dafcd8bc33d026ef4c56d220eae2799
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870213"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="d1c7b-104">leakedCredentialsRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1c7b-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="d1c7b-105">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="d1c7b-106">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="d1c7b-107">[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的某个帐户凭据已在通配符中检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="d1c7b-108">有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="d1c7b-109">方法</span><span class="sxs-lookup"><span data-stu-id="d1c7b-109">Methods</span></span>

| <span data-ttu-id="d1c7b-110">方法</span><span class="sxs-lookup"><span data-stu-id="d1c7b-110">Method</span></span>           | <span data-ttu-id="d1c7b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1c7b-111">Return Type</span></span>    |<span data-ttu-id="d1c7b-112">说明</span><span class="sxs-lookup"><span data-stu-id="d1c7b-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1c7b-113">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d1c7b-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="d1c7b-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d1c7b-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="d1c7b-115">读取 leakedCredentialsRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1c7b-116">属性</span><span class="sxs-lookup"><span data-stu-id="d1c7b-116">Properties</span></span>
| <span data-ttu-id="d1c7b-117">属性</span><span class="sxs-lookup"><span data-stu-id="d1c7b-117">Property</span></span>     | <span data-ttu-id="d1c7b-118">类型</span><span class="sxs-lookup"><span data-stu-id="d1c7b-118">Type</span></span>   |<span data-ttu-id="d1c7b-119">说明</span><span class="sxs-lookup"><span data-stu-id="d1c7b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1c7b-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1c7b-120">closedDateTime</span></span>|<span data-ttu-id="d1c7b-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1c7b-121">dateTimeOffset</span></span>| <span data-ttu-id="d1c7b-122">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="d1c7b-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="d1c7b-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1c7b-123">createdDateTime</span></span>|<span data-ttu-id="d1c7b-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1c7b-124">dateTimeOffset</span></span>| <span data-ttu-id="d1c7b-125">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="d1c7b-126">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="d1c7b-127">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="d1c7b-128">id</span><span class="sxs-lookup"><span data-stu-id="d1c7b-128">id</span></span>|<span data-ttu-id="d1c7b-129">字符串</span><span class="sxs-lookup"><span data-stu-id="d1c7b-129">string</span></span>| <span data-ttu-id="d1c7b-130">只读</span><span class="sxs-lookup"><span data-stu-id="d1c7b-130">Read-only</span></span>|
|<span data-ttu-id="d1c7b-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="d1c7b-131">riskEventDateTime</span></span>|<span data-ttu-id="d1c7b-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1c7b-132">dateTimeOffset</span></span>| <span data-ttu-id="d1c7b-133">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="d1c7b-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="d1c7b-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="d1c7b-134">riskEventStatus</span></span>|<span data-ttu-id="d1c7b-135">string</span><span class="sxs-lookup"><span data-stu-id="d1c7b-135">string</span></span>| <span data-ttu-id="d1c7b-136">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="d1c7b-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d1c7b-137">riskLevel</span></span>|<span data-ttu-id="d1c7b-138">string</span><span class="sxs-lookup"><span data-stu-id="d1c7b-138">string</span></span>| <span data-ttu-id="d1c7b-139">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="d1c7b-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="d1c7b-140">riskEventType</span></span>|<span data-ttu-id="d1c7b-141">string</span><span class="sxs-lookup"><span data-stu-id="d1c7b-141">string</span></span>| <span data-ttu-id="d1c7b-142">风险的类型</span><span class="sxs-lookup"><span data-stu-id="d1c7b-142">The type of risk</span></span>|
|<span data-ttu-id="d1c7b-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d1c7b-143">userDisplayName</span></span>|<span data-ttu-id="d1c7b-144">string</span><span class="sxs-lookup"><span data-stu-id="d1c7b-144">string</span></span>| <span data-ttu-id="d1c7b-145">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="d1c7b-145">The name of the user at risk</span></span>|
|<span data-ttu-id="d1c7b-146">userId</span><span class="sxs-lookup"><span data-stu-id="d1c7b-146">userId</span></span>|<span data-ttu-id="d1c7b-147">string</span><span class="sxs-lookup"><span data-stu-id="d1c7b-147">string</span></span>| <span data-ttu-id="d1c7b-148">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="d1c7b-148">The id of the user at risk</span></span>|
|<span data-ttu-id="d1c7b-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d1c7b-149">userPrincipalName</span></span>|<span data-ttu-id="d1c7b-150">string</span><span class="sxs-lookup"><span data-stu-id="d1c7b-150">string</span></span>| <span data-ttu-id="d1c7b-151">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d1c7b-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1c7b-152">关系</span><span class="sxs-lookup"><span data-stu-id="d1c7b-152">Relationships</span></span>
| <span data-ttu-id="d1c7b-153">关系</span><span class="sxs-lookup"><span data-stu-id="d1c7b-153">Relationship</span></span> | <span data-ttu-id="d1c7b-154">类型</span><span class="sxs-lookup"><span data-stu-id="d1c7b-154">Type</span></span>   |<span data-ttu-id="d1c7b-155">说明</span><span class="sxs-lookup"><span data-stu-id="d1c7b-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1c7b-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="d1c7b-156">impactedUser</span></span>|[<span data-ttu-id="d1c7b-157">user</span><span class="sxs-lookup"><span data-stu-id="d1c7b-157">user</span></span>](user.md)| <span data-ttu-id="d1c7b-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1c7b-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1c7b-160">JSON representation</span></span>

<span data-ttu-id="d1c7b-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1c7b-161">Here is a JSON representation of the resource.</span></span>

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
