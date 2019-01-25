---
title: suspiciousIpRiskEvent 资源类型
description: 风险事件检测到的 Azure Active Directory 标识保护其中帐户登录尝试从可疑的 IP 地址。 Azure AD 身份保护文档中，可以找到有关风险事件的完整信息。
localization_priority: Normal
ms.openlocfilehash: e144e1f631941076b5cee7cee20d90062564012a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515809"
---
# <a name="suspiciousipriskevent-resource-type"></a><span data-ttu-id="70710-104">suspiciousIpRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="70710-104">suspiciousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70710-105">风险事件检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中帐户登录尝试从可疑的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="70710-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="70710-106">[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="70710-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="70710-107">方法</span><span class="sxs-lookup"><span data-stu-id="70710-107">Methods</span></span>

| <span data-ttu-id="70710-108">方法</span><span class="sxs-lookup"><span data-stu-id="70710-108">Method</span></span>           | <span data-ttu-id="70710-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="70710-109">Return Type</span></span>    |<span data-ttu-id="70710-110">说明</span><span class="sxs-lookup"><span data-stu-id="70710-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70710-111">获取 suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="70710-111">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="70710-112">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="70710-112">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="70710-113">读取属性和 suspiciousIpRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="70710-113">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70710-114">属性</span><span class="sxs-lookup"><span data-stu-id="70710-114">Properties</span></span>
| <span data-ttu-id="70710-115">属性</span><span class="sxs-lookup"><span data-stu-id="70710-115">Property</span></span>     | <span data-ttu-id="70710-116">类型</span><span class="sxs-lookup"><span data-stu-id="70710-116">Type</span></span>   |<span data-ttu-id="70710-117">说明</span><span class="sxs-lookup"><span data-stu-id="70710-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70710-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="70710-118">closedDateTime</span></span>|<span data-ttu-id="70710-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70710-119">dateTimeOffset</span></span>| <span data-ttu-id="70710-120">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="70710-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="70710-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70710-121">createdDateTime</span></span>|<span data-ttu-id="70710-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70710-122">dateTimeOffset</span></span>| <span data-ttu-id="70710-123">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="70710-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="70710-124">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="70710-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="70710-125">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="70710-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="70710-126">id</span><span class="sxs-lookup"><span data-stu-id="70710-126">id</span></span>|<span data-ttu-id="70710-127">string</span><span class="sxs-lookup"><span data-stu-id="70710-127">string</span></span>| <span data-ttu-id="70710-128">只读</span><span class="sxs-lookup"><span data-stu-id="70710-128">Read-only</span></span>|
|<span data-ttu-id="70710-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="70710-129">ipAddress</span></span>|<span data-ttu-id="70710-130">string</span><span class="sxs-lookup"><span data-stu-id="70710-130">string</span></span>| <span data-ttu-id="70710-131">登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="70710-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="70710-132">location</span><span class="sxs-lookup"><span data-stu-id="70710-132">location</span></span>|<span data-ttu-id="70710-133">字符串</span><span class="sxs-lookup"><span data-stu-id="70710-133">string</span></span>| <span data-ttu-id="70710-134">挂接到登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="70710-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="70710-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="70710-135">riskEventDateTime</span></span>|<span data-ttu-id="70710-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70710-136">dateTimeOffset</span></span>| <span data-ttu-id="70710-137">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="70710-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="70710-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="70710-138">riskEventStatus</span></span>|<span data-ttu-id="70710-139">string</span><span class="sxs-lookup"><span data-stu-id="70710-139">string</span></span>| <span data-ttu-id="70710-140">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="70710-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="70710-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="70710-141">riskLevel</span></span>|<span data-ttu-id="70710-142">string</span><span class="sxs-lookup"><span data-stu-id="70710-142">string</span></span>| <span data-ttu-id="70710-143">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="70710-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="70710-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="70710-144">riskEventType</span></span>|<span data-ttu-id="70710-145">string</span><span class="sxs-lookup"><span data-stu-id="70710-145">string</span></span>| <span data-ttu-id="70710-146">风险类型</span><span class="sxs-lookup"><span data-stu-id="70710-146">The type of risk</span></span>|
|<span data-ttu-id="70710-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="70710-147">userDisplayName</span></span>|<span data-ttu-id="70710-148">string</span><span class="sxs-lookup"><span data-stu-id="70710-148">string</span></span>| <span data-ttu-id="70710-149">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="70710-149">The name of the user at risk</span></span>|
|<span data-ttu-id="70710-150">userId</span><span class="sxs-lookup"><span data-stu-id="70710-150">userId</span></span>|<span data-ttu-id="70710-151">string</span><span class="sxs-lookup"><span data-stu-id="70710-151">string</span></span>| <span data-ttu-id="70710-152">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="70710-152">The id of the user at risk</span></span>|
|<span data-ttu-id="70710-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70710-153">userPrincipalName</span></span>|<span data-ttu-id="70710-154">string</span><span class="sxs-lookup"><span data-stu-id="70710-154">string</span></span>| <span data-ttu-id="70710-155">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="70710-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="70710-156">关系</span><span class="sxs-lookup"><span data-stu-id="70710-156">Relationships</span></span>
| <span data-ttu-id="70710-157">关系</span><span class="sxs-lookup"><span data-stu-id="70710-157">Relationship</span></span> | <span data-ttu-id="70710-158">类型</span><span class="sxs-lookup"><span data-stu-id="70710-158">Type</span></span>   |<span data-ttu-id="70710-159">说明</span><span class="sxs-lookup"><span data-stu-id="70710-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70710-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="70710-160">impactedUser</span></span>|[<span data-ttu-id="70710-161">user</span><span class="sxs-lookup"><span data-stu-id="70710-161">user</span></span>](user.md)| <span data-ttu-id="70710-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="70710-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70710-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70710-164">JSON representation</span></span>

<span data-ttu-id="70710-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70710-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
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
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/suspiciousipriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
