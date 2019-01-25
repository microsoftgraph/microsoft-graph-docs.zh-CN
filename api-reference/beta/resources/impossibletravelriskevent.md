---
title: impossibleTravelRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护其中两个帐户登录发生从用户在典型的位置，并将不可能要登录宏的完整信息之间的工期中的位置之间的差旅风险事件Azure AD 身份保护文档中找不到风险事件。
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529381"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="ba028-103">impossibleTravelRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba028-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba028-104">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中两个帐户登录发生从用户在典型的位置，并将不可能要登录宏完成之间的工期中的位置之间的差旅风险事件[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的信息。</span><span class="sxs-lookup"><span data-stu-id="ba028-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="ba028-105">方法</span><span class="sxs-lookup"><span data-stu-id="ba028-105">Methods</span></span>

| <span data-ttu-id="ba028-106">方法</span><span class="sxs-lookup"><span data-stu-id="ba028-106">Method</span></span>           | <span data-ttu-id="ba028-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba028-107">Return Type</span></span>    |<span data-ttu-id="ba028-108">说明</span><span class="sxs-lookup"><span data-stu-id="ba028-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba028-109">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ba028-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="ba028-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ba028-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="ba028-111">读取属性和 impossibleTravelRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ba028-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba028-112">属性</span><span class="sxs-lookup"><span data-stu-id="ba028-112">Properties</span></span>
| <span data-ttu-id="ba028-113">属性</span><span class="sxs-lookup"><span data-stu-id="ba028-113">Property</span></span>     | <span data-ttu-id="ba028-114">类型</span><span class="sxs-lookup"><span data-stu-id="ba028-114">Type</span></span>   |<span data-ttu-id="ba028-115">说明</span><span class="sxs-lookup"><span data-stu-id="ba028-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba028-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba028-116">closedDateTime</span></span>|<span data-ttu-id="ba028-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba028-117">dateTimeOffset</span></span>| <span data-ttu-id="ba028-118">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="ba028-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ba028-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba028-119">createdDateTime</span></span>|<span data-ttu-id="ba028-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba028-120">dateTimeOffset</span></span>| <span data-ttu-id="ba028-121">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="ba028-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="ba028-122">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="ba028-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ba028-123">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="ba028-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ba028-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="ba028-124">deviceInformation</span></span>|<span data-ttu-id="ba028-125">string</span><span class="sxs-lookup"><span data-stu-id="ba028-125">string</span></span>| <span data-ttu-id="ba028-126">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="ba028-126">Information about the device</span></span>|
|<span data-ttu-id="ba028-127">id</span><span class="sxs-lookup"><span data-stu-id="ba028-127">id</span></span>|<span data-ttu-id="ba028-128">string</span><span class="sxs-lookup"><span data-stu-id="ba028-128">string</span></span>| <span data-ttu-id="ba028-129">只读</span><span class="sxs-lookup"><span data-stu-id="ba028-129">Read-only</span></span>|
|<span data-ttu-id="ba028-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ba028-130">ipAddress</span></span>|<span data-ttu-id="ba028-131">string</span><span class="sxs-lookup"><span data-stu-id="ba028-131">string</span></span>| <span data-ttu-id="ba028-132">IP 地址的第二个登录</span><span class="sxs-lookup"><span data-stu-id="ba028-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="ba028-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="ba028-133">isAtypicalLocation</span></span>|<span data-ttu-id="ba028-134">布尔</span><span class="sxs-lookup"><span data-stu-id="ba028-134">boolean</span></span>| <span data-ttu-id="ba028-135">如果在位置之一是用户在典型</span><span class="sxs-lookup"><span data-stu-id="ba028-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="ba028-136">location</span><span class="sxs-lookup"><span data-stu-id="ba028-136">location</span></span>|<span data-ttu-id="ba028-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ba028-137">string</span></span>| <span data-ttu-id="ba028-138">挂接到第二个登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="ba028-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="ba028-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="ba028-139">previousIPAddress</span></span>|<span data-ttu-id="ba028-140">string</span><span class="sxs-lookup"><span data-stu-id="ba028-140">string</span></span>| <span data-ttu-id="ba028-141">首次登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="ba028-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="ba028-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="ba028-142">previousLocation</span></span>|<span data-ttu-id="ba028-143">string</span><span class="sxs-lookup"><span data-stu-id="ba028-143">string</span></span>| <span data-ttu-id="ba028-144">挂接到首次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="ba028-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="ba028-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="ba028-145">previousSigninDateTime</span></span>|<span data-ttu-id="ba028-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba028-146">dateTimeOffset</span></span>| <span data-ttu-id="ba028-147">日期和时间的首次登录</span><span class="sxs-lookup"><span data-stu-id="ba028-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="ba028-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="ba028-148">riskEventDateTime</span></span>|<span data-ttu-id="ba028-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba028-149">dateTimeOffset</span></span>| <span data-ttu-id="ba028-150">日期和时间的第二个登录</span><span class="sxs-lookup"><span data-stu-id="ba028-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="ba028-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="ba028-151">riskEventStatus</span></span>|<span data-ttu-id="ba028-152">string</span><span class="sxs-lookup"><span data-stu-id="ba028-152">string</span></span>| <span data-ttu-id="ba028-153">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="ba028-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ba028-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ba028-154">riskLevel</span></span>|<span data-ttu-id="ba028-155">string</span><span class="sxs-lookup"><span data-stu-id="ba028-155">string</span></span>| <span data-ttu-id="ba028-156">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ba028-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ba028-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="ba028-157">riskEventType</span></span>|<span data-ttu-id="ba028-158">string</span><span class="sxs-lookup"><span data-stu-id="ba028-158">string</span></span>| <span data-ttu-id="ba028-159">风险类型</span><span class="sxs-lookup"><span data-stu-id="ba028-159">The type of risk</span></span>|
|<span data-ttu-id="ba028-160">UserAgent</span><span class="sxs-lookup"><span data-stu-id="ba028-160">userAgent</span></span>|<span data-ttu-id="ba028-161">string</span><span class="sxs-lookup"><span data-stu-id="ba028-161">string</span></span>| <span data-ttu-id="ba028-162">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="ba028-162">The browser's user agent string</span></span>|
|<span data-ttu-id="ba028-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba028-163">userDisplayName</span></span>|<span data-ttu-id="ba028-164">string</span><span class="sxs-lookup"><span data-stu-id="ba028-164">string</span></span>| <span data-ttu-id="ba028-165">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="ba028-165">The name of the user at risk</span></span>|
|<span data-ttu-id="ba028-166">userId</span><span class="sxs-lookup"><span data-stu-id="ba028-166">userId</span></span>|<span data-ttu-id="ba028-167">string</span><span class="sxs-lookup"><span data-stu-id="ba028-167">string</span></span>| <span data-ttu-id="ba028-168">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="ba028-168">The id of the user at risk</span></span>|
|<span data-ttu-id="ba028-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ba028-169">userPrincipalName</span></span>|<span data-ttu-id="ba028-170">string</span><span class="sxs-lookup"><span data-stu-id="ba028-170">string</span></span>| <span data-ttu-id="ba028-171">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ba028-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba028-172">关系</span><span class="sxs-lookup"><span data-stu-id="ba028-172">Relationships</span></span>
| <span data-ttu-id="ba028-173">关系</span><span class="sxs-lookup"><span data-stu-id="ba028-173">Relationship</span></span> | <span data-ttu-id="ba028-174">类型</span><span class="sxs-lookup"><span data-stu-id="ba028-174">Type</span></span>   |<span data-ttu-id="ba028-175">说明</span><span class="sxs-lookup"><span data-stu-id="ba028-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba028-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="ba028-176">impactedUser</span></span>|[<span data-ttu-id="ba028-177">user</span><span class="sxs-lookup"><span data-stu-id="ba028-177">user</span></span>](user.md)| <span data-ttu-id="ba028-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ba028-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba028-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba028-180">JSON representation</span></span>

<span data-ttu-id="ba028-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba028-181">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
