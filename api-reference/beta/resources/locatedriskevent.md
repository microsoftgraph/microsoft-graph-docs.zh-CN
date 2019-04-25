---
title: locatedRiskEvent 资源类型
description: '基于位置数据的 Azure Active Directory 标识保护检测到的风险事件。 找到的风险事件类型包括:'
localization_priority: Normal
ms.openlocfilehash: 20fe76099c511483144b42e33fc260910debb5ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578146"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="4702c-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="4702c-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4702c-105">基于位置数据的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="4702c-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="4702c-106">找到的风险事件类型包括:</span><span class="sxs-lookup"><span data-stu-id="4702c-106">Located risk event types include:</span></span>
* [<span data-ttu-id="4702c-107">来自匿名 IP 地址的登录</span><span class="sxs-lookup"><span data-stu-id="4702c-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="4702c-108">来自受恶意软件感染的设备的登录</span><span class="sxs-lookup"><span data-stu-id="4702c-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="4702c-109">无法移动到非常规位置</span><span class="sxs-lookup"><span data-stu-id="4702c-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="4702c-110">来自可疑 IP 地址的登录</span><span class="sxs-lookup"><span data-stu-id="4702c-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="4702c-111">[来自不熟悉位置的登录](unfamiliarlocationriskevent.md)有关风险事件的完整信息, 请参阅[Azure AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="4702c-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="4702c-112">方法</span><span class="sxs-lookup"><span data-stu-id="4702c-112">Methods</span></span>

| <span data-ttu-id="4702c-113">方法</span><span class="sxs-lookup"><span data-stu-id="4702c-113">Method</span></span>           | <span data-ttu-id="4702c-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="4702c-114">Return Type</span></span>    |<span data-ttu-id="4702c-115">说明</span><span class="sxs-lookup"><span data-stu-id="4702c-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4702c-116">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4702c-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="4702c-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4702c-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="4702c-118">读取 locatedRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4702c-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4702c-119">属性</span><span class="sxs-lookup"><span data-stu-id="4702c-119">Properties</span></span>
| <span data-ttu-id="4702c-120">属性</span><span class="sxs-lookup"><span data-stu-id="4702c-120">Property</span></span>     | <span data-ttu-id="4702c-121">类型</span><span class="sxs-lookup"><span data-stu-id="4702c-121">Type</span></span>   |<span data-ttu-id="4702c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4702c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4702c-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="4702c-123">closedDateTime</span></span>|<span data-ttu-id="4702c-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4702c-124">dateTimeOffset</span></span>| <span data-ttu-id="4702c-125">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="4702c-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="4702c-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4702c-126">createdDateTime</span></span>|<span data-ttu-id="4702c-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4702c-127">dateTimeOffset</span></span>| <span data-ttu-id="4702c-128">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4702c-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="4702c-129">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="4702c-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="4702c-130">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="4702c-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="4702c-131">id</span><span class="sxs-lookup"><span data-stu-id="4702c-131">id</span></span>|<span data-ttu-id="4702c-132">string</span><span class="sxs-lookup"><span data-stu-id="4702c-132">string</span></span>| <span data-ttu-id="4702c-133">只读</span><span class="sxs-lookup"><span data-stu-id="4702c-133">Read-only</span></span>|
|<span data-ttu-id="4702c-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4702c-134">ipAddress</span></span>|<span data-ttu-id="4702c-135">string</span><span class="sxs-lookup"><span data-stu-id="4702c-135">string</span></span>| <span data-ttu-id="4702c-136">登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="4702c-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="4702c-137">location</span><span class="sxs-lookup"><span data-stu-id="4702c-137">location</span></span>|<span data-ttu-id="4702c-138">string</span><span class="sxs-lookup"><span data-stu-id="4702c-138">string</span></span>| <span data-ttu-id="4702c-139">连接到登录 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="4702c-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="4702c-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="4702c-140">riskEventDateTime</span></span>|<span data-ttu-id="4702c-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4702c-141">dateTimeOffset</span></span>| <span data-ttu-id="4702c-142">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="4702c-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="4702c-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="4702c-143">riskEventStatus</span></span>|<span data-ttu-id="4702c-144">string</span><span class="sxs-lookup"><span data-stu-id="4702c-144">string</span></span>| <span data-ttu-id="4702c-145">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="4702c-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="4702c-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="4702c-146">riskLevel</span></span>|<span data-ttu-id="4702c-147">string</span><span class="sxs-lookup"><span data-stu-id="4702c-147">string</span></span>| <span data-ttu-id="4702c-148">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="4702c-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="4702c-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="4702c-149">riskEventType</span></span>|<span data-ttu-id="4702c-150">string</span><span class="sxs-lookup"><span data-stu-id="4702c-150">string</span></span>| <span data-ttu-id="4702c-151">风险的类型</span><span class="sxs-lookup"><span data-stu-id="4702c-151">The type of risk</span></span>|
|<span data-ttu-id="4702c-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4702c-152">userDisplayName</span></span>|<span data-ttu-id="4702c-153">string</span><span class="sxs-lookup"><span data-stu-id="4702c-153">string</span></span>| <span data-ttu-id="4702c-154">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="4702c-154">The name of the user at risk</span></span>|
|<span data-ttu-id="4702c-155">userId</span><span class="sxs-lookup"><span data-stu-id="4702c-155">userId</span></span>|<span data-ttu-id="4702c-156">string</span><span class="sxs-lookup"><span data-stu-id="4702c-156">string</span></span>| <span data-ttu-id="4702c-157">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="4702c-157">The id of the user at risk</span></span>|
|<span data-ttu-id="4702c-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4702c-158">userPrincipalName</span></span>|<span data-ttu-id="4702c-159">string</span><span class="sxs-lookup"><span data-stu-id="4702c-159">string</span></span>| <span data-ttu-id="4702c-160">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4702c-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="4702c-161">关系</span><span class="sxs-lookup"><span data-stu-id="4702c-161">Relationships</span></span>
| <span data-ttu-id="4702c-162">关系</span><span class="sxs-lookup"><span data-stu-id="4702c-162">Relationship</span></span> | <span data-ttu-id="4702c-163">类型</span><span class="sxs-lookup"><span data-stu-id="4702c-163">Type</span></span>   |<span data-ttu-id="4702c-164">说明</span><span class="sxs-lookup"><span data-stu-id="4702c-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4702c-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="4702c-165">impactedUser</span></span>|[<span data-ttu-id="4702c-166">用户</span><span class="sxs-lookup"><span data-stu-id="4702c-166">user</span></span>](user.md)| <span data-ttu-id="4702c-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4702c-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4702c-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4702c-169">JSON representation</span></span>

<span data-ttu-id="4702c-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4702c-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/locatedriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
