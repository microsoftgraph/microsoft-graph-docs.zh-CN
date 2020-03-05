---
title: locatedRiskEvent 资源类型
description: 基于位置数据的 Azure Active Directory 标识保护检测到的风险事件。 找到的风险事件类型包括：
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b7abb10417e7659e923eddf04990067c8b979ce9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522923"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="e49df-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e49df-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="e49df-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e49df-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49df-106">基于位置数据的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="e49df-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="e49df-107">找到的风险事件类型包括：</span><span class="sxs-lookup"><span data-stu-id="e49df-107">Located risk event types include:</span></span>
* [<span data-ttu-id="e49df-108">来自匿名 IP 地址的登录</span><span class="sxs-lookup"><span data-stu-id="e49df-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="e49df-109">来自受恶意软件感染的设备的登录</span><span class="sxs-lookup"><span data-stu-id="e49df-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="e49df-110">无法移动到非常规位置</span><span class="sxs-lookup"><span data-stu-id="e49df-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="e49df-111">来自可疑 IP 地址的登录</span><span class="sxs-lookup"><span data-stu-id="e49df-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="e49df-112">[来自不熟悉位置的登录](unfamiliarlocationriskevent.md)有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="e49df-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="e49df-113">方法</span><span class="sxs-lookup"><span data-stu-id="e49df-113">Methods</span></span>

| <span data-ttu-id="e49df-114">方法</span><span class="sxs-lookup"><span data-stu-id="e49df-114">Method</span></span>           | <span data-ttu-id="e49df-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="e49df-115">Return Type</span></span>    |<span data-ttu-id="e49df-116">说明</span><span class="sxs-lookup"><span data-stu-id="e49df-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e49df-117">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e49df-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="e49df-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e49df-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="e49df-119">读取 locatedRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e49df-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e49df-120">属性</span><span class="sxs-lookup"><span data-stu-id="e49df-120">Properties</span></span>
| <span data-ttu-id="e49df-121">属性</span><span class="sxs-lookup"><span data-stu-id="e49df-121">Property</span></span>     | <span data-ttu-id="e49df-122">类型</span><span class="sxs-lookup"><span data-stu-id="e49df-122">Type</span></span>   |<span data-ttu-id="e49df-123">说明</span><span class="sxs-lookup"><span data-stu-id="e49df-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e49df-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e49df-124">closedDateTime</span></span>|<span data-ttu-id="e49df-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49df-125">dateTimeOffset</span></span>| <span data-ttu-id="e49df-126">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="e49df-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e49df-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e49df-127">createdDateTime</span></span>|<span data-ttu-id="e49df-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49df-128">dateTimeOffset</span></span>| <span data-ttu-id="e49df-129">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e49df-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="e49df-130">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="e49df-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e49df-131">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="e49df-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e49df-132">id</span><span class="sxs-lookup"><span data-stu-id="e49df-132">id</span></span>|<span data-ttu-id="e49df-133">string</span><span class="sxs-lookup"><span data-stu-id="e49df-133">string</span></span>| <span data-ttu-id="e49df-134">只读</span><span class="sxs-lookup"><span data-stu-id="e49df-134">Read-only</span></span>|
|<span data-ttu-id="e49df-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e49df-135">ipAddress</span></span>|<span data-ttu-id="e49df-136">string</span><span class="sxs-lookup"><span data-stu-id="e49df-136">string</span></span>| <span data-ttu-id="e49df-137">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="e49df-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="e49df-138">location</span><span class="sxs-lookup"><span data-stu-id="e49df-138">location</span></span>|<span data-ttu-id="e49df-139">string</span><span class="sxs-lookup"><span data-stu-id="e49df-139">string</span></span>| <span data-ttu-id="e49df-140">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="e49df-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="e49df-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e49df-141">riskEventDateTime</span></span>|<span data-ttu-id="e49df-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e49df-142">dateTimeOffset</span></span>| <span data-ttu-id="e49df-143">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="e49df-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e49df-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e49df-144">riskEventStatus</span></span>|<span data-ttu-id="e49df-145">string</span><span class="sxs-lookup"><span data-stu-id="e49df-145">string</span></span>| <span data-ttu-id="e49df-146">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="e49df-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e49df-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e49df-147">riskLevel</span></span>|<span data-ttu-id="e49df-148">string</span><span class="sxs-lookup"><span data-stu-id="e49df-148">string</span></span>| <span data-ttu-id="e49df-149">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e49df-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e49df-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e49df-150">riskEventType</span></span>|<span data-ttu-id="e49df-151">string</span><span class="sxs-lookup"><span data-stu-id="e49df-151">string</span></span>| <span data-ttu-id="e49df-152">风险的类型</span><span class="sxs-lookup"><span data-stu-id="e49df-152">The type of risk</span></span>|
|<span data-ttu-id="e49df-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e49df-153">userDisplayName</span></span>|<span data-ttu-id="e49df-154">string</span><span class="sxs-lookup"><span data-stu-id="e49df-154">string</span></span>| <span data-ttu-id="e49df-155">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="e49df-155">The name of the user at risk</span></span>|
|<span data-ttu-id="e49df-156">userId</span><span class="sxs-lookup"><span data-stu-id="e49df-156">userId</span></span>|<span data-ttu-id="e49df-157">string</span><span class="sxs-lookup"><span data-stu-id="e49df-157">string</span></span>| <span data-ttu-id="e49df-158">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="e49df-158">The id of the user at risk</span></span>|
|<span data-ttu-id="e49df-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e49df-159">userPrincipalName</span></span>|<span data-ttu-id="e49df-160">string</span><span class="sxs-lookup"><span data-stu-id="e49df-160">string</span></span>| <span data-ttu-id="e49df-161">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e49df-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e49df-162">关系</span><span class="sxs-lookup"><span data-stu-id="e49df-162">Relationships</span></span>
| <span data-ttu-id="e49df-163">关系</span><span class="sxs-lookup"><span data-stu-id="e49df-163">Relationship</span></span> | <span data-ttu-id="e49df-164">类型</span><span class="sxs-lookup"><span data-stu-id="e49df-164">Type</span></span>   |<span data-ttu-id="e49df-165">说明</span><span class="sxs-lookup"><span data-stu-id="e49df-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e49df-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e49df-166">impactedUser</span></span>|[<span data-ttu-id="e49df-167">用户</span><span class="sxs-lookup"><span data-stu-id="e49df-167">user</span></span>](user.md)| <span data-ttu-id="e49df-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="e49df-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e49df-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e49df-170">JSON representation</span></span>

<span data-ttu-id="e49df-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e49df-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
  "@odata.type": "microsoft.graph.locatedRiskEvent"
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
