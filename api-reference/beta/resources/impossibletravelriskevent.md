---
title: impossibleTravelRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件, 其中两个帐户登录从用户的非典型位置发生, 并且在登录之间的持续时间之间无法进行移动。有关详细信息, 请参阅可在 Azure AD Identity Protection 文档中找到风险事件。
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548325"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="4b035-103">impossibleTravelRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b035-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b035-104">[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件, 其中两个帐户登录从用户的非典型位置发生, 并且在登录之间的持续时间之间无法进行移动。完成有关风险事件的信息可以在[Azure AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中找到。</span><span class="sxs-lookup"><span data-stu-id="4b035-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="4b035-105">方法</span><span class="sxs-lookup"><span data-stu-id="4b035-105">Methods</span></span>

| <span data-ttu-id="4b035-106">方法</span><span class="sxs-lookup"><span data-stu-id="4b035-106">Method</span></span>           | <span data-ttu-id="4b035-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b035-107">Return Type</span></span>    |<span data-ttu-id="4b035-108">说明</span><span class="sxs-lookup"><span data-stu-id="4b035-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b035-109">获取 impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4b035-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="4b035-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="4b035-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="4b035-111">读取 impossibleTravelRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b035-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b035-112">属性</span><span class="sxs-lookup"><span data-stu-id="4b035-112">Properties</span></span>
| <span data-ttu-id="4b035-113">属性</span><span class="sxs-lookup"><span data-stu-id="4b035-113">Property</span></span>     | <span data-ttu-id="4b035-114">类型</span><span class="sxs-lookup"><span data-stu-id="4b035-114">Type</span></span>   |<span data-ttu-id="4b035-115">说明</span><span class="sxs-lookup"><span data-stu-id="4b035-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b035-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b035-116">closedDateTime</span></span>|<span data-ttu-id="4b035-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b035-117">dateTimeOffset</span></span>| <span data-ttu-id="4b035-118">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="4b035-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="4b035-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b035-119">createdDateTime</span></span>|<span data-ttu-id="4b035-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b035-120">dateTimeOffset</span></span>| <span data-ttu-id="4b035-121">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4b035-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="4b035-122">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="4b035-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="4b035-123">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="4b035-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="4b035-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="4b035-124">deviceInformation</span></span>|<span data-ttu-id="4b035-125">string</span><span class="sxs-lookup"><span data-stu-id="4b035-125">string</span></span>| <span data-ttu-id="4b035-126">有关设备的信息</span><span class="sxs-lookup"><span data-stu-id="4b035-126">Information about the device</span></span>|
|<span data-ttu-id="4b035-127">id</span><span class="sxs-lookup"><span data-stu-id="4b035-127">id</span></span>|<span data-ttu-id="4b035-128">string</span><span class="sxs-lookup"><span data-stu-id="4b035-128">string</span></span>| <span data-ttu-id="4b035-129">只读</span><span class="sxs-lookup"><span data-stu-id="4b035-129">Read-only</span></span>|
|<span data-ttu-id="4b035-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4b035-130">ipAddress</span></span>|<span data-ttu-id="4b035-131">string</span><span class="sxs-lookup"><span data-stu-id="4b035-131">string</span></span>| <span data-ttu-id="4b035-132">第二次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="4b035-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="4b035-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="4b035-133">isAtypicalLocation</span></span>|<span data-ttu-id="4b035-134">布尔</span><span class="sxs-lookup"><span data-stu-id="4b035-134">boolean</span></span>| <span data-ttu-id="4b035-135">如果其中一个位置对用户是典型的</span><span class="sxs-lookup"><span data-stu-id="4b035-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="4b035-136">location</span><span class="sxs-lookup"><span data-stu-id="4b035-136">location</span></span>|<span data-ttu-id="4b035-137">string</span><span class="sxs-lookup"><span data-stu-id="4b035-137">string</span></span>| <span data-ttu-id="4b035-138">连接到第二次登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="4b035-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="4b035-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="4b035-139">previousIPAddress</span></span>|<span data-ttu-id="4b035-140">string</span><span class="sxs-lookup"><span data-stu-id="4b035-140">string</span></span>| <span data-ttu-id="4b035-141">第一次登录的 IP 地址</span><span class="sxs-lookup"><span data-stu-id="4b035-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="4b035-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="4b035-142">previousLocation</span></span>|<span data-ttu-id="4b035-143">string</span><span class="sxs-lookup"><span data-stu-id="4b035-143">string</span></span>| <span data-ttu-id="4b035-144">第一次登录的 IP 地址所连接的位置</span><span class="sxs-lookup"><span data-stu-id="4b035-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="4b035-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="4b035-145">previousSigninDateTime</span></span>|<span data-ttu-id="4b035-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b035-146">dateTimeOffset</span></span>| <span data-ttu-id="4b035-147">首次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="4b035-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="4b035-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="4b035-148">riskEventDateTime</span></span>|<span data-ttu-id="4b035-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b035-149">dateTimeOffset</span></span>| <span data-ttu-id="4b035-150">第二次登录的日期和时间</span><span class="sxs-lookup"><span data-stu-id="4b035-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="4b035-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="4b035-151">riskEventStatus</span></span>|<span data-ttu-id="4b035-152">string</span><span class="sxs-lookup"><span data-stu-id="4b035-152">string</span></span>| <span data-ttu-id="4b035-153">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="4b035-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="4b035-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="4b035-154">riskLevel</span></span>|<span data-ttu-id="4b035-155">string</span><span class="sxs-lookup"><span data-stu-id="4b035-155">string</span></span>| <span data-ttu-id="4b035-156">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="4b035-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="4b035-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="4b035-157">riskEventType</span></span>|<span data-ttu-id="4b035-158">string</span><span class="sxs-lookup"><span data-stu-id="4b035-158">string</span></span>| <span data-ttu-id="4b035-159">风险的类型</span><span class="sxs-lookup"><span data-stu-id="4b035-159">The type of risk</span></span>|
|<span data-ttu-id="4b035-160">userAgent</span><span class="sxs-lookup"><span data-stu-id="4b035-160">userAgent</span></span>|<span data-ttu-id="4b035-161">string</span><span class="sxs-lookup"><span data-stu-id="4b035-161">string</span></span>| <span data-ttu-id="4b035-162">浏览器的用户代理字符串</span><span class="sxs-lookup"><span data-stu-id="4b035-162">The browser's user agent string</span></span>|
|<span data-ttu-id="4b035-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4b035-163">userDisplayName</span></span>|<span data-ttu-id="4b035-164">string</span><span class="sxs-lookup"><span data-stu-id="4b035-164">string</span></span>| <span data-ttu-id="4b035-165">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="4b035-165">The name of the user at risk</span></span>|
|<span data-ttu-id="4b035-166">userId</span><span class="sxs-lookup"><span data-stu-id="4b035-166">userId</span></span>|<span data-ttu-id="4b035-167">string</span><span class="sxs-lookup"><span data-stu-id="4b035-167">string</span></span>| <span data-ttu-id="4b035-168">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="4b035-168">The id of the user at risk</span></span>|
|<span data-ttu-id="4b035-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b035-169">userPrincipalName</span></span>|<span data-ttu-id="4b035-170">string</span><span class="sxs-lookup"><span data-stu-id="4b035-170">string</span></span>| <span data-ttu-id="4b035-171">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4b035-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b035-172">关系</span><span class="sxs-lookup"><span data-stu-id="4b035-172">Relationships</span></span>
| <span data-ttu-id="4b035-173">关系</span><span class="sxs-lookup"><span data-stu-id="4b035-173">Relationship</span></span> | <span data-ttu-id="4b035-174">类型</span><span class="sxs-lookup"><span data-stu-id="4b035-174">Type</span></span>   |<span data-ttu-id="4b035-175">说明</span><span class="sxs-lookup"><span data-stu-id="4b035-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b035-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="4b035-176">impactedUser</span></span>|[<span data-ttu-id="4b035-177">user</span><span class="sxs-lookup"><span data-stu-id="4b035-177">user</span></span>](user.md)| <span data-ttu-id="4b035-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4b035-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b035-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b035-180">JSON representation</span></span>

<span data-ttu-id="4b035-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b035-181">Here is a JSON representation of the resource.</span></span>

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
