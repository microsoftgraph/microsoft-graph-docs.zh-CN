---
title: locatedRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护基于位置数据的风险事件。 位于的风险事件类型包括：
localization_priority: Normal
ms.openlocfilehash: 20fe76099c511483144b42e33fc260910debb5ed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510258"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="08f95-104">locatedRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="08f95-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f95-105">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)基于位置数据的风险事件。</span><span class="sxs-lookup"><span data-stu-id="08f95-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="08f95-106">位于的风险事件类型包括：</span><span class="sxs-lookup"><span data-stu-id="08f95-106">Located risk event types include:</span></span>
* [<span data-ttu-id="08f95-107">从匿名登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="08f95-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="08f95-108">从感染恶意软件的设备登录</span><span class="sxs-lookup"><span data-stu-id="08f95-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="08f95-109">对在典型的位置的意思出差</span><span class="sxs-lookup"><span data-stu-id="08f95-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="08f95-110">登录从可疑 IP 地址</span><span class="sxs-lookup"><span data-stu-id="08f95-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="08f95-111">[从不熟悉位置登录](unfamiliarlocationriskevent.md)[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="08f95-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="08f95-112">方法</span><span class="sxs-lookup"><span data-stu-id="08f95-112">Methods</span></span>

| <span data-ttu-id="08f95-113">方法</span><span class="sxs-lookup"><span data-stu-id="08f95-113">Method</span></span>           | <span data-ttu-id="08f95-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="08f95-114">Return Type</span></span>    |<span data-ttu-id="08f95-115">说明</span><span class="sxs-lookup"><span data-stu-id="08f95-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08f95-116">获取 locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="08f95-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="08f95-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="08f95-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="08f95-118">读取属性和 locatedRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="08f95-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08f95-119">属性</span><span class="sxs-lookup"><span data-stu-id="08f95-119">Properties</span></span>
| <span data-ttu-id="08f95-120">属性</span><span class="sxs-lookup"><span data-stu-id="08f95-120">Property</span></span>     | <span data-ttu-id="08f95-121">类型</span><span class="sxs-lookup"><span data-stu-id="08f95-121">Type</span></span>   |<span data-ttu-id="08f95-122">说明</span><span class="sxs-lookup"><span data-stu-id="08f95-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08f95-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="08f95-123">closedDateTime</span></span>|<span data-ttu-id="08f95-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f95-124">dateTimeOffset</span></span>| <span data-ttu-id="08f95-125">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="08f95-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="08f95-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08f95-126">createdDateTime</span></span>|<span data-ttu-id="08f95-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f95-127">dateTimeOffset</span></span>| <span data-ttu-id="08f95-128">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="08f95-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="08f95-129">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="08f95-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="08f95-130">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="08f95-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="08f95-131">id</span><span class="sxs-lookup"><span data-stu-id="08f95-131">id</span></span>|<span data-ttu-id="08f95-132">string</span><span class="sxs-lookup"><span data-stu-id="08f95-132">string</span></span>| <span data-ttu-id="08f95-133">只读</span><span class="sxs-lookup"><span data-stu-id="08f95-133">Read-only</span></span>|
|<span data-ttu-id="08f95-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="08f95-134">ipAddress</span></span>|<span data-ttu-id="08f95-135">string</span><span class="sxs-lookup"><span data-stu-id="08f95-135">string</span></span>| <span data-ttu-id="08f95-136">登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="08f95-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="08f95-137">location</span><span class="sxs-lookup"><span data-stu-id="08f95-137">location</span></span>|<span data-ttu-id="08f95-138">字符串</span><span class="sxs-lookup"><span data-stu-id="08f95-138">string</span></span>| <span data-ttu-id="08f95-139">挂接到登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="08f95-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="08f95-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="08f95-140">riskEventDateTime</span></span>|<span data-ttu-id="08f95-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f95-141">dateTimeOffset</span></span>| <span data-ttu-id="08f95-142">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="08f95-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="08f95-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="08f95-143">riskEventStatus</span></span>|<span data-ttu-id="08f95-144">string</span><span class="sxs-lookup"><span data-stu-id="08f95-144">string</span></span>| <span data-ttu-id="08f95-145">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="08f95-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="08f95-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="08f95-146">riskLevel</span></span>|<span data-ttu-id="08f95-147">string</span><span class="sxs-lookup"><span data-stu-id="08f95-147">string</span></span>| <span data-ttu-id="08f95-148">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="08f95-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="08f95-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="08f95-149">riskEventType</span></span>|<span data-ttu-id="08f95-150">string</span><span class="sxs-lookup"><span data-stu-id="08f95-150">string</span></span>| <span data-ttu-id="08f95-151">风险类型</span><span class="sxs-lookup"><span data-stu-id="08f95-151">The type of risk</span></span>|
|<span data-ttu-id="08f95-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="08f95-152">userDisplayName</span></span>|<span data-ttu-id="08f95-153">string</span><span class="sxs-lookup"><span data-stu-id="08f95-153">string</span></span>| <span data-ttu-id="08f95-154">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="08f95-154">The name of the user at risk</span></span>|
|<span data-ttu-id="08f95-155">userId</span><span class="sxs-lookup"><span data-stu-id="08f95-155">userId</span></span>|<span data-ttu-id="08f95-156">string</span><span class="sxs-lookup"><span data-stu-id="08f95-156">string</span></span>| <span data-ttu-id="08f95-157">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="08f95-157">The id of the user at risk</span></span>|
|<span data-ttu-id="08f95-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08f95-158">userPrincipalName</span></span>|<span data-ttu-id="08f95-159">string</span><span class="sxs-lookup"><span data-stu-id="08f95-159">string</span></span>| <span data-ttu-id="08f95-160">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="08f95-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="08f95-161">关系</span><span class="sxs-lookup"><span data-stu-id="08f95-161">Relationships</span></span>
| <span data-ttu-id="08f95-162">关系</span><span class="sxs-lookup"><span data-stu-id="08f95-162">Relationship</span></span> | <span data-ttu-id="08f95-163">类型</span><span class="sxs-lookup"><span data-stu-id="08f95-163">Type</span></span>   |<span data-ttu-id="08f95-164">说明</span><span class="sxs-lookup"><span data-stu-id="08f95-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08f95-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="08f95-165">impactedUser</span></span>|[<span data-ttu-id="08f95-166">user</span><span class="sxs-lookup"><span data-stu-id="08f95-166">user</span></span>](user.md)| <span data-ttu-id="08f95-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="08f95-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08f95-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08f95-169">JSON representation</span></span>

<span data-ttu-id="08f95-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08f95-170">Here is a JSON representation of the resource.</span></span>

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
