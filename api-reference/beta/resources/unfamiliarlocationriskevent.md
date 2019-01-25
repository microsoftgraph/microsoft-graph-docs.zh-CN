---
title: unfamiliarLocationRiskEvent 资源类型
description: 风险事件检测到的 Azure Active Directory 标识保护其中帐户登录尝试从用户的新位置。 Azure AD 身份保护文档中，可以找到有关风险事件的完整信息。
localization_priority: Normal
ms.openlocfilehash: adad214c0ac58540f1115b836c2c5f26faa6c031
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507976"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="ea695-104">unfamiliarLocationRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea695-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea695-105">风险事件检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中帐户登录尝试从用户的新位置。</span><span class="sxs-lookup"><span data-stu-id="ea695-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="ea695-106">[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="ea695-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="ea695-107">方法</span><span class="sxs-lookup"><span data-stu-id="ea695-107">Methods</span></span>

| <span data-ttu-id="ea695-108">方法</span><span class="sxs-lookup"><span data-stu-id="ea695-108">Method</span></span>           | <span data-ttu-id="ea695-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea695-109">Return Type</span></span>    |<span data-ttu-id="ea695-110">说明</span><span class="sxs-lookup"><span data-stu-id="ea695-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea695-111">获取 unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ea695-111">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="ea695-112">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ea695-112">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="ea695-113">读取属性和 unfamiliarLocationRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ea695-113">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea695-114">属性</span><span class="sxs-lookup"><span data-stu-id="ea695-114">Properties</span></span>
| <span data-ttu-id="ea695-115">属性</span><span class="sxs-lookup"><span data-stu-id="ea695-115">Property</span></span>     | <span data-ttu-id="ea695-116">类型</span><span class="sxs-lookup"><span data-stu-id="ea695-116">Type</span></span>   |<span data-ttu-id="ea695-117">说明</span><span class="sxs-lookup"><span data-stu-id="ea695-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea695-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea695-118">closedDateTime</span></span>|<span data-ttu-id="ea695-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea695-119">dateTimeOffset</span></span>| <span data-ttu-id="ea695-120">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="ea695-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ea695-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea695-121">createdDateTime</span></span>|<span data-ttu-id="ea695-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea695-122">dateTimeOffset</span></span>| <span data-ttu-id="ea695-123">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="ea695-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="ea695-124">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="ea695-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ea695-125">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="ea695-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ea695-126">id</span><span class="sxs-lookup"><span data-stu-id="ea695-126">id</span></span>|<span data-ttu-id="ea695-127">string</span><span class="sxs-lookup"><span data-stu-id="ea695-127">string</span></span>| <span data-ttu-id="ea695-128">只读</span><span class="sxs-lookup"><span data-stu-id="ea695-128">Read-only</span></span>|
|<span data-ttu-id="ea695-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ea695-129">ipAddress</span></span>|<span data-ttu-id="ea695-130">string</span><span class="sxs-lookup"><span data-stu-id="ea695-130">string</span></span>| <span data-ttu-id="ea695-131">登录 IP 地址</span><span class="sxs-lookup"><span data-stu-id="ea695-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="ea695-132">location</span><span class="sxs-lookup"><span data-stu-id="ea695-132">location</span></span>|<span data-ttu-id="ea695-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ea695-133">string</span></span>| <span data-ttu-id="ea695-134">挂接到登录的 IP 地址的位置</span><span class="sxs-lookup"><span data-stu-id="ea695-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="ea695-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="ea695-135">riskEventDateTime</span></span>|<span data-ttu-id="ea695-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea695-136">dateTimeOffset</span></span>| <span data-ttu-id="ea695-137">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="ea695-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="ea695-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="ea695-138">riskEventStatus</span></span>|<span data-ttu-id="ea695-139">string</span><span class="sxs-lookup"><span data-stu-id="ea695-139">string</span></span>| <span data-ttu-id="ea695-140">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="ea695-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ea695-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ea695-141">riskLevel</span></span>|<span data-ttu-id="ea695-142">string</span><span class="sxs-lookup"><span data-stu-id="ea695-142">string</span></span>| <span data-ttu-id="ea695-143">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="ea695-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ea695-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="ea695-144">riskEventType</span></span>|<span data-ttu-id="ea695-145">string</span><span class="sxs-lookup"><span data-stu-id="ea695-145">string</span></span>| <span data-ttu-id="ea695-146">风险类型</span><span class="sxs-lookup"><span data-stu-id="ea695-146">The type of risk</span></span>|
|<span data-ttu-id="ea695-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ea695-147">userDisplayName</span></span>|<span data-ttu-id="ea695-148">string</span><span class="sxs-lookup"><span data-stu-id="ea695-148">string</span></span>| <span data-ttu-id="ea695-149">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="ea695-149">The name of the user at risk</span></span>|
|<span data-ttu-id="ea695-150">userId</span><span class="sxs-lookup"><span data-stu-id="ea695-150">userId</span></span>|<span data-ttu-id="ea695-151">string</span><span class="sxs-lookup"><span data-stu-id="ea695-151">string</span></span>| <span data-ttu-id="ea695-152">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="ea695-152">The id of the user at risk</span></span>|
|<span data-ttu-id="ea695-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ea695-153">userPrincipalName</span></span>|<span data-ttu-id="ea695-154">string</span><span class="sxs-lookup"><span data-stu-id="ea695-154">string</span></span>| <span data-ttu-id="ea695-155">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ea695-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea695-156">关系</span><span class="sxs-lookup"><span data-stu-id="ea695-156">Relationships</span></span>
| <span data-ttu-id="ea695-157">关系</span><span class="sxs-lookup"><span data-stu-id="ea695-157">Relationship</span></span> | <span data-ttu-id="ea695-158">类型</span><span class="sxs-lookup"><span data-stu-id="ea695-158">Type</span></span>   |<span data-ttu-id="ea695-159">说明</span><span class="sxs-lookup"><span data-stu-id="ea695-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea695-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="ea695-160">impactedUser</span></span>|[<span data-ttu-id="ea695-161">user</span><span class="sxs-lookup"><span data-stu-id="ea695-161">user</span></span>](user.md)| <span data-ttu-id="ea695-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ea695-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea695-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea695-164">JSON representation</span></span>

<span data-ttu-id="ea695-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea695-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/unfamiliarlocationriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
