---
title: anonymousIpRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的一个风险事件, 其中的帐户登录尝试来自看似匿名的 IP 地址。 有关风险事件的完整信息, 请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5016aac704feb35383dc34e58f3ed06657733edf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013387"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="b159e-104">anonymousIpRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b159e-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b159e-105">[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的一个风险事件, 其中的帐户登录尝试来自看似匿名的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b159e-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="b159e-106">有关风险事件的完整信息, 请参阅[AZURE AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="b159e-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="b159e-107">方法</span><span class="sxs-lookup"><span data-stu-id="b159e-107">Methods</span></span>

| <span data-ttu-id="b159e-108">方法</span><span class="sxs-lookup"><span data-stu-id="b159e-108">Method</span></span>           | <span data-ttu-id="b159e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b159e-109">Return Type</span></span>    |<span data-ttu-id="b159e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b159e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b159e-111">获取 anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="b159e-111">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="b159e-112">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="b159e-112">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="b159e-113">读取 anonymousIpRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b159e-113">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b159e-114">属性</span><span class="sxs-lookup"><span data-stu-id="b159e-114">Properties</span></span>
| <span data-ttu-id="b159e-115">属性</span><span class="sxs-lookup"><span data-stu-id="b159e-115">Property</span></span>     | <span data-ttu-id="b159e-116">类型</span><span class="sxs-lookup"><span data-stu-id="b159e-116">Type</span></span>   |<span data-ttu-id="b159e-117">说明</span><span class="sxs-lookup"><span data-stu-id="b159e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b159e-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="b159e-118">closedDateTime</span></span>|<span data-ttu-id="b159e-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b159e-119">dateTimeOffset</span></span>| <span data-ttu-id="b159e-120">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b159e-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="b159e-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b159e-121">createdDateTime</span></span>|<span data-ttu-id="b159e-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b159e-122">dateTimeOffset</span></span>| <span data-ttu-id="b159e-123">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b159e-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="b159e-124">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="b159e-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="b159e-125">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="b159e-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="b159e-126">id</span><span class="sxs-lookup"><span data-stu-id="b159e-126">id</span></span>|<span data-ttu-id="b159e-127">string</span><span class="sxs-lookup"><span data-stu-id="b159e-127">string</span></span>| <span data-ttu-id="b159e-128">只读</span><span class="sxs-lookup"><span data-stu-id="b159e-128">Read-only</span></span>|
|<span data-ttu-id="b159e-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b159e-129">ipAddress</span></span>|<span data-ttu-id="b159e-130">string</span><span class="sxs-lookup"><span data-stu-id="b159e-130">string</span></span>| <span data-ttu-id="b159e-131">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="b159e-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="b159e-132">location</span><span class="sxs-lookup"><span data-stu-id="b159e-132">location</span></span>|<span data-ttu-id="b159e-133">string</span><span class="sxs-lookup"><span data-stu-id="b159e-133">string</span></span>| <span data-ttu-id="b159e-134">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="b159e-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="b159e-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="b159e-135">riskEventDateTime</span></span>|<span data-ttu-id="b159e-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b159e-136">dateTimeOffset</span></span>| <span data-ttu-id="b159e-137">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="b159e-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="b159e-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="b159e-138">riskEventStatus</span></span>|<span data-ttu-id="b159e-139">string</span><span class="sxs-lookup"><span data-stu-id="b159e-139">string</span></span>| <span data-ttu-id="b159e-140">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="b159e-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="b159e-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b159e-141">riskLevel</span></span>|<span data-ttu-id="b159e-142">string</span><span class="sxs-lookup"><span data-stu-id="b159e-142">string</span></span>| <span data-ttu-id="b159e-143">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="b159e-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="b159e-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="b159e-144">riskEventType</span></span>|<span data-ttu-id="b159e-145">string</span><span class="sxs-lookup"><span data-stu-id="b159e-145">string</span></span>| <span data-ttu-id="b159e-146">风险的类型</span><span class="sxs-lookup"><span data-stu-id="b159e-146">The type of risk</span></span>|
|<span data-ttu-id="b159e-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b159e-147">userDisplayName</span></span>|<span data-ttu-id="b159e-148">string</span><span class="sxs-lookup"><span data-stu-id="b159e-148">string</span></span>| <span data-ttu-id="b159e-149">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="b159e-149">The name of the user at risk</span></span>|
|<span data-ttu-id="b159e-150">userId</span><span class="sxs-lookup"><span data-stu-id="b159e-150">userId</span></span>|<span data-ttu-id="b159e-151">string</span><span class="sxs-lookup"><span data-stu-id="b159e-151">string</span></span>| <span data-ttu-id="b159e-152">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="b159e-152">The id of the user at risk</span></span>|
|<span data-ttu-id="b159e-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b159e-153">userPrincipalName</span></span>|<span data-ttu-id="b159e-154">string</span><span class="sxs-lookup"><span data-stu-id="b159e-154">string</span></span>| <span data-ttu-id="b159e-155">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b159e-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="b159e-156">关系</span><span class="sxs-lookup"><span data-stu-id="b159e-156">Relationships</span></span>
| <span data-ttu-id="b159e-157">关系</span><span class="sxs-lookup"><span data-stu-id="b159e-157">Relationship</span></span> | <span data-ttu-id="b159e-158">类型</span><span class="sxs-lookup"><span data-stu-id="b159e-158">Type</span></span>   |<span data-ttu-id="b159e-159">说明</span><span class="sxs-lookup"><span data-stu-id="b159e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b159e-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="b159e-160">impactedUser</span></span>|[<span data-ttu-id="b159e-161">用户</span><span class="sxs-lookup"><span data-stu-id="b159e-161">user</span></span>](user.md)| <span data-ttu-id="b159e-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="b159e-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b159e-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b159e-164">JSON representation</span></span>

<span data-ttu-id="b159e-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b159e-165">Here is a JSON representation of the resource.</span></span>

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
