---
title: locatedRiskEvent 资源类型
description: Azure Active Directory Identity Protection 根据位置数据检测到的风险事件。 定位的风险事件类型包括：
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: c53c503132a0b280c8b7fb02c99816d2ee7a5f03
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51490989"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="c9d08-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9d08-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="c9d08-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d08-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d08-106">Azure [Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) 根据位置数据检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="c9d08-106">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) that is based on location data.</span></span> <span data-ttu-id="c9d08-107">定位的风险事件类型包括：</span><span class="sxs-lookup"><span data-stu-id="c9d08-107">Located risk event types include:</span></span>
* [<span data-ttu-id="c9d08-108">从匿名 IP 地址登录</span><span class="sxs-lookup"><span data-stu-id="c9d08-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="c9d08-109">来自感染了恶意软件的设备登录</span><span class="sxs-lookup"><span data-stu-id="c9d08-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="c9d08-110">不可能到达非典型位置</span><span class="sxs-lookup"><span data-stu-id="c9d08-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="c9d08-111">从可疑 IP 地址登录</span><span class="sxs-lookup"><span data-stu-id="c9d08-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="c9d08-112">[从不熟悉的位置登录](unfamiliarlocationriskevent.md) 有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="c9d08-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="c9d08-113">方法</span><span class="sxs-lookup"><span data-stu-id="c9d08-113">Methods</span></span>

| <span data-ttu-id="c9d08-114">方法</span><span class="sxs-lookup"><span data-stu-id="c9d08-114">Method</span></span>           | <span data-ttu-id="c9d08-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9d08-115">Return Type</span></span>    |<span data-ttu-id="c9d08-116">说明</span><span class="sxs-lookup"><span data-stu-id="c9d08-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9d08-117">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c9d08-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="c9d08-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c9d08-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="c9d08-119">读取 locatedRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9d08-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9d08-120">属性</span><span class="sxs-lookup"><span data-stu-id="c9d08-120">Properties</span></span>
| <span data-ttu-id="c9d08-121">属性</span><span class="sxs-lookup"><span data-stu-id="c9d08-121">Property</span></span>     | <span data-ttu-id="c9d08-122">类型</span><span class="sxs-lookup"><span data-stu-id="c9d08-122">Type</span></span>   |<span data-ttu-id="c9d08-123">说明</span><span class="sxs-lookup"><span data-stu-id="c9d08-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d08-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d08-124">closedDateTime</span></span>|<span data-ttu-id="c9d08-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9d08-125">dateTimeOffset</span></span>| <span data-ttu-id="c9d08-126">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c9d08-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c9d08-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d08-127">createdDateTime</span></span>|<span data-ttu-id="c9d08-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9d08-128">dateTimeOffset</span></span>| <span data-ttu-id="c9d08-129">创建风险事件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c9d08-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="c9d08-130">这始终大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="c9d08-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c9d08-131">这是在查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="c9d08-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c9d08-132">id</span><span class="sxs-lookup"><span data-stu-id="c9d08-132">id</span></span>|<span data-ttu-id="c9d08-133">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-133">string</span></span>| <span data-ttu-id="c9d08-134">只读</span><span class="sxs-lookup"><span data-stu-id="c9d08-134">Read-only</span></span>|
|<span data-ttu-id="c9d08-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c9d08-135">ipAddress</span></span>|<span data-ttu-id="c9d08-136">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-136">string</span></span>| <span data-ttu-id="c9d08-137">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="c9d08-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="c9d08-138">location</span><span class="sxs-lookup"><span data-stu-id="c9d08-138">location</span></span>|<span data-ttu-id="c9d08-139">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-139">string</span></span>| <span data-ttu-id="c9d08-140">附加到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="c9d08-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="c9d08-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d08-141">riskEventDateTime</span></span>|<span data-ttu-id="c9d08-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9d08-142">dateTimeOffset</span></span>| <span data-ttu-id="c9d08-143">发生风险事件的日期和时间</span><span class="sxs-lookup"><span data-stu-id="c9d08-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c9d08-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c9d08-144">riskEventStatus</span></span>|<span data-ttu-id="c9d08-145">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-145">string</span></span>| <span data-ttu-id="c9d08-146">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="c9d08-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c9d08-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c9d08-147">riskLevel</span></span>|<span data-ttu-id="c9d08-148">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-148">string</span></span>| <span data-ttu-id="c9d08-149">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c9d08-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c9d08-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c9d08-150">riskEventType</span></span>|<span data-ttu-id="c9d08-151">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-151">string</span></span>| <span data-ttu-id="c9d08-152">风险类型</span><span class="sxs-lookup"><span data-stu-id="c9d08-152">The type of risk</span></span>|
|<span data-ttu-id="c9d08-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c9d08-153">userDisplayName</span></span>|<span data-ttu-id="c9d08-154">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-154">string</span></span>| <span data-ttu-id="c9d08-155">处于风险中的用户的名称</span><span class="sxs-lookup"><span data-stu-id="c9d08-155">The name of the user at risk</span></span>|
|<span data-ttu-id="c9d08-156">userId</span><span class="sxs-lookup"><span data-stu-id="c9d08-156">userId</span></span>|<span data-ttu-id="c9d08-157">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-157">string</span></span>| <span data-ttu-id="c9d08-158">处于风险中的用户的 ID</span><span class="sxs-lookup"><span data-stu-id="c9d08-158">The id of the user at risk</span></span>|
|<span data-ttu-id="c9d08-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c9d08-159">userPrincipalName</span></span>|<span data-ttu-id="c9d08-160">string</span><span class="sxs-lookup"><span data-stu-id="c9d08-160">string</span></span>| <span data-ttu-id="c9d08-161">处于风险中的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c9d08-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9d08-162">关系</span><span class="sxs-lookup"><span data-stu-id="c9d08-162">Relationships</span></span>
| <span data-ttu-id="c9d08-163">关系</span><span class="sxs-lookup"><span data-stu-id="c9d08-163">Relationship</span></span> | <span data-ttu-id="c9d08-164">类型</span><span class="sxs-lookup"><span data-stu-id="c9d08-164">Type</span></span>   |<span data-ttu-id="c9d08-165">说明</span><span class="sxs-lookup"><span data-stu-id="c9d08-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d08-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c9d08-166">impactedUser</span></span>|[<span data-ttu-id="c9d08-167">用户</span><span class="sxs-lookup"><span data-stu-id="c9d08-167">user</span></span>](user.md)| <span data-ttu-id="c9d08-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="c9d08-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9d08-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9d08-170">JSON representation</span></span>

<span data-ttu-id="c9d08-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9d08-171">Here is a JSON representation of the resource.</span></span>

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