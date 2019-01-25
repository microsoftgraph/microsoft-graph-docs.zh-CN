---
title: leakedCredentialsRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护其中已帐户的凭据检测到的风险事件。 Azure AD 身份保护文档中，可以找到有关风险事件的完整信息。
localization_priority: Normal
ms.openlocfilehash: 0884da08195ffa2bee38c943d27b1d25aef02e49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510986"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="de901-104">leakedCredentialsRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="de901-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de901-105">检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中已帐户的凭据检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="de901-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="de901-106">[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。</span><span class="sxs-lookup"><span data-stu-id="de901-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="de901-107">方法</span><span class="sxs-lookup"><span data-stu-id="de901-107">Methods</span></span>

| <span data-ttu-id="de901-108">方法</span><span class="sxs-lookup"><span data-stu-id="de901-108">Method</span></span>           | <span data-ttu-id="de901-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="de901-109">Return Type</span></span>    |<span data-ttu-id="de901-110">说明</span><span class="sxs-lookup"><span data-stu-id="de901-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de901-111">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="de901-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="de901-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="de901-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="de901-113">读取属性和 leakedCredentialsRiskEvent 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="de901-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de901-114">属性</span><span class="sxs-lookup"><span data-stu-id="de901-114">Properties</span></span>
| <span data-ttu-id="de901-115">属性</span><span class="sxs-lookup"><span data-stu-id="de901-115">Property</span></span>     | <span data-ttu-id="de901-116">类型</span><span class="sxs-lookup"><span data-stu-id="de901-116">Type</span></span>   |<span data-ttu-id="de901-117">说明</span><span class="sxs-lookup"><span data-stu-id="de901-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de901-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="de901-118">closedDateTime</span></span>|<span data-ttu-id="de901-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de901-119">dateTimeOffset</span></span>| <span data-ttu-id="de901-120">日期和时间的风险事件已关闭</span><span class="sxs-lookup"><span data-stu-id="de901-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="de901-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de901-121">createdDateTime</span></span>|<span data-ttu-id="de901-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de901-122">dateTimeOffset</span></span>| <span data-ttu-id="de901-123">日期和时间的风险事件的创建。</span><span class="sxs-lookup"><span data-stu-id="de901-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="de901-124">始终是大于或等于风险事件本身的 datetime。</span><span class="sxs-lookup"><span data-stu-id="de901-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="de901-125">这是正确的属性，以用作筛选器时查询风险事件。</span><span class="sxs-lookup"><span data-stu-id="de901-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="de901-126">id</span><span class="sxs-lookup"><span data-stu-id="de901-126">id</span></span>|<span data-ttu-id="de901-127">string</span><span class="sxs-lookup"><span data-stu-id="de901-127">string</span></span>| <span data-ttu-id="de901-128">只读</span><span class="sxs-lookup"><span data-stu-id="de901-128">Read-only</span></span>|
|<span data-ttu-id="de901-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="de901-129">riskEventDateTime</span></span>|<span data-ttu-id="de901-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de901-130">dateTimeOffset</span></span>| <span data-ttu-id="de901-131">日期和风险事件发生的时间</span><span class="sxs-lookup"><span data-stu-id="de901-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="de901-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="de901-132">riskEventStatus</span></span>|<span data-ttu-id="de901-133">string</span><span class="sxs-lookup"><span data-stu-id="de901-133">string</span></span>| <span data-ttu-id="de901-134">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="de901-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="de901-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="de901-135">riskLevel</span></span>|<span data-ttu-id="de901-136">string</span><span class="sxs-lookup"><span data-stu-id="de901-136">string</span></span>| <span data-ttu-id="de901-137">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="de901-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="de901-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="de901-138">riskEventType</span></span>|<span data-ttu-id="de901-139">string</span><span class="sxs-lookup"><span data-stu-id="de901-139">string</span></span>| <span data-ttu-id="de901-140">风险类型</span><span class="sxs-lookup"><span data-stu-id="de901-140">The type of risk</span></span>|
|<span data-ttu-id="de901-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="de901-141">userDisplayName</span></span>|<span data-ttu-id="de901-142">string</span><span class="sxs-lookup"><span data-stu-id="de901-142">string</span></span>| <span data-ttu-id="de901-143">风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="de901-143">The name of the user at risk</span></span>|
|<span data-ttu-id="de901-144">userId</span><span class="sxs-lookup"><span data-stu-id="de901-144">userId</span></span>|<span data-ttu-id="de901-145">string</span><span class="sxs-lookup"><span data-stu-id="de901-145">string</span></span>| <span data-ttu-id="de901-146">风险的用户 id</span><span class="sxs-lookup"><span data-stu-id="de901-146">The id of the user at risk</span></span>|
|<span data-ttu-id="de901-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de901-147">userPrincipalName</span></span>|<span data-ttu-id="de901-148">string</span><span class="sxs-lookup"><span data-stu-id="de901-148">string</span></span>| <span data-ttu-id="de901-149">风险的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="de901-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="de901-150">关系</span><span class="sxs-lookup"><span data-stu-id="de901-150">Relationships</span></span>
| <span data-ttu-id="de901-151">关系</span><span class="sxs-lookup"><span data-stu-id="de901-151">Relationship</span></span> | <span data-ttu-id="de901-152">类型</span><span class="sxs-lookup"><span data-stu-id="de901-152">Type</span></span>   |<span data-ttu-id="de901-153">说明</span><span class="sxs-lookup"><span data-stu-id="de901-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de901-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="de901-154">impactedUser</span></span>|[<span data-ttu-id="de901-155">user</span><span class="sxs-lookup"><span data-stu-id="de901-155">user</span></span>](user.md)| <span data-ttu-id="de901-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="de901-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de901-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de901-158">JSON representation</span></span>

<span data-ttu-id="de901-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de901-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/leakedcredentialsriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
