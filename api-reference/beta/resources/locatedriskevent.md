---
title: locatedRiskEvent 资源类型
description: 基于位置数据的 Azure Active Directory 标识保护检测到的风险事件。 找到的风险事件类型包括：
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 461f20233e92edca48b9dd51fa417b33ab9f386c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404670"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="50049-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="50049-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="50049-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50049-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50049-106">基于位置数据的 [Azure Active Directory 标识保护](/azure/active-directory/identity-protection/overview-identity-protection) 检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="50049-106">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) that is based on location data.</span></span> <span data-ttu-id="50049-107">找到的风险事件类型包括：</span><span class="sxs-lookup"><span data-stu-id="50049-107">Located risk event types include:</span></span>
* [<span data-ttu-id="50049-108">来自匿名 IP 地址的登录</span><span class="sxs-lookup"><span data-stu-id="50049-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="50049-109">来自受恶意软件感染的设备的登录</span><span class="sxs-lookup"><span data-stu-id="50049-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="50049-110">无法移动到非常规位置</span><span class="sxs-lookup"><span data-stu-id="50049-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="50049-111">来自可疑 IP 地址的登录</span><span class="sxs-lookup"><span data-stu-id="50049-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="50049-112">[来自不熟悉位置的登录](unfamiliarlocationriskevent.md) 有关风险事件的完整信息，请参阅 [AZURE AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。</span><span class="sxs-lookup"><span data-stu-id="50049-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="50049-113">方法</span><span class="sxs-lookup"><span data-stu-id="50049-113">Methods</span></span>

| <span data-ttu-id="50049-114">方法</span><span class="sxs-lookup"><span data-stu-id="50049-114">Method</span></span>           | <span data-ttu-id="50049-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="50049-115">Return Type</span></span>    |<span data-ttu-id="50049-116">说明</span><span class="sxs-lookup"><span data-stu-id="50049-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50049-117">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="50049-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="50049-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="50049-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="50049-119">读取 locatedRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50049-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50049-120">属性</span><span class="sxs-lookup"><span data-stu-id="50049-120">Properties</span></span>
| <span data-ttu-id="50049-121">属性</span><span class="sxs-lookup"><span data-stu-id="50049-121">Property</span></span>     | <span data-ttu-id="50049-122">类型</span><span class="sxs-lookup"><span data-stu-id="50049-122">Type</span></span>   |<span data-ttu-id="50049-123">说明</span><span class="sxs-lookup"><span data-stu-id="50049-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50049-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="50049-124">closedDateTime</span></span>|<span data-ttu-id="50049-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50049-125">dateTimeOffset</span></span>| <span data-ttu-id="50049-126">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="50049-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="50049-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50049-127">createdDateTime</span></span>|<span data-ttu-id="50049-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50049-128">dateTimeOffset</span></span>| <span data-ttu-id="50049-129">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="50049-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="50049-130">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="50049-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="50049-131">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="50049-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="50049-132">id</span><span class="sxs-lookup"><span data-stu-id="50049-132">id</span></span>|<span data-ttu-id="50049-133">string</span><span class="sxs-lookup"><span data-stu-id="50049-133">string</span></span>| <span data-ttu-id="50049-134">只读</span><span class="sxs-lookup"><span data-stu-id="50049-134">Read-only</span></span>|
|<span data-ttu-id="50049-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="50049-135">ipAddress</span></span>|<span data-ttu-id="50049-136">string</span><span class="sxs-lookup"><span data-stu-id="50049-136">string</span></span>| <span data-ttu-id="50049-137">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="50049-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="50049-138">location</span><span class="sxs-lookup"><span data-stu-id="50049-138">location</span></span>|<span data-ttu-id="50049-139">string</span><span class="sxs-lookup"><span data-stu-id="50049-139">string</span></span>| <span data-ttu-id="50049-140">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="50049-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="50049-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="50049-141">riskEventDateTime</span></span>|<span data-ttu-id="50049-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50049-142">dateTimeOffset</span></span>| <span data-ttu-id="50049-143">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="50049-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="50049-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="50049-144">riskEventStatus</span></span>|<span data-ttu-id="50049-145">string</span><span class="sxs-lookup"><span data-stu-id="50049-145">string</span></span>| <span data-ttu-id="50049-146">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="50049-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="50049-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="50049-147">riskLevel</span></span>|<span data-ttu-id="50049-148">string</span><span class="sxs-lookup"><span data-stu-id="50049-148">string</span></span>| <span data-ttu-id="50049-149">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="50049-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="50049-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="50049-150">riskEventType</span></span>|<span data-ttu-id="50049-151">string</span><span class="sxs-lookup"><span data-stu-id="50049-151">string</span></span>| <span data-ttu-id="50049-152">风险的类型</span><span class="sxs-lookup"><span data-stu-id="50049-152">The type of risk</span></span>|
|<span data-ttu-id="50049-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="50049-153">userDisplayName</span></span>|<span data-ttu-id="50049-154">string</span><span class="sxs-lookup"><span data-stu-id="50049-154">string</span></span>| <span data-ttu-id="50049-155">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="50049-155">The name of the user at risk</span></span>|
|<span data-ttu-id="50049-156">userId</span><span class="sxs-lookup"><span data-stu-id="50049-156">userId</span></span>|<span data-ttu-id="50049-157">string</span><span class="sxs-lookup"><span data-stu-id="50049-157">string</span></span>| <span data-ttu-id="50049-158">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="50049-158">The id of the user at risk</span></span>|
|<span data-ttu-id="50049-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50049-159">userPrincipalName</span></span>|<span data-ttu-id="50049-160">string</span><span class="sxs-lookup"><span data-stu-id="50049-160">string</span></span>| <span data-ttu-id="50049-161">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="50049-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="50049-162">关系</span><span class="sxs-lookup"><span data-stu-id="50049-162">Relationships</span></span>
| <span data-ttu-id="50049-163">关系</span><span class="sxs-lookup"><span data-stu-id="50049-163">Relationship</span></span> | <span data-ttu-id="50049-164">类型</span><span class="sxs-lookup"><span data-stu-id="50049-164">Type</span></span>   |<span data-ttu-id="50049-165">说明</span><span class="sxs-lookup"><span data-stu-id="50049-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50049-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="50049-166">impactedUser</span></span>|[<span data-ttu-id="50049-167">用户</span><span class="sxs-lookup"><span data-stu-id="50049-167">user</span></span>](user.md)| <span data-ttu-id="50049-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="50049-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50049-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50049-170">JSON representation</span></span>

<span data-ttu-id="50049-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50049-171">Here is a JSON representation of the resource.</span></span>

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