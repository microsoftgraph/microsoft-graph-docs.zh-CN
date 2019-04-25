---
title: leakedCredentialsRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的某个帐户凭据已在通配符中检测到的风险事件。 有关风险事件的完整信息, 请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
ms.openlocfilehash: 0884da08195ffa2bee38c943d27b1d25aef02e49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581085"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="430de-104">leakedCredentialsRiskEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="430de-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430de-105">[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的某个帐户凭据已在通配符中检测到的风险事件。</span><span class="sxs-lookup"><span data-stu-id="430de-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="430de-106">有关风险事件的完整信息, 请参阅[Azure AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)。</span><span class="sxs-lookup"><span data-stu-id="430de-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="430de-107">方法</span><span class="sxs-lookup"><span data-stu-id="430de-107">Methods</span></span>

| <span data-ttu-id="430de-108">方法</span><span class="sxs-lookup"><span data-stu-id="430de-108">Method</span></span>           | <span data-ttu-id="430de-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="430de-109">Return Type</span></span>    |<span data-ttu-id="430de-110">说明</span><span class="sxs-lookup"><span data-stu-id="430de-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="430de-111">获取 leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="430de-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="430de-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="430de-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="430de-113">读取 leakedCredentialsRiskEvent 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="430de-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="430de-114">属性</span><span class="sxs-lookup"><span data-stu-id="430de-114">Properties</span></span>
| <span data-ttu-id="430de-115">属性</span><span class="sxs-lookup"><span data-stu-id="430de-115">Property</span></span>     | <span data-ttu-id="430de-116">类型</span><span class="sxs-lookup"><span data-stu-id="430de-116">Type</span></span>   |<span data-ttu-id="430de-117">说明</span><span class="sxs-lookup"><span data-stu-id="430de-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="430de-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="430de-118">closedDateTime</span></span>|<span data-ttu-id="430de-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430de-119">dateTimeOffset</span></span>| <span data-ttu-id="430de-120">风险事件关闭的日期和时间</span><span class="sxs-lookup"><span data-stu-id="430de-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="430de-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="430de-121">createdDateTime</span></span>|<span data-ttu-id="430de-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430de-122">dateTimeOffset</span></span>| <span data-ttu-id="430de-123">风险事件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="430de-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="430de-124">此值始终大于或等于风险事件本身的日期时间。</span><span class="sxs-lookup"><span data-stu-id="430de-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="430de-125">这是查询风险事件时用作筛选器的正确属性。</span><span class="sxs-lookup"><span data-stu-id="430de-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="430de-126">id</span><span class="sxs-lookup"><span data-stu-id="430de-126">id</span></span>|<span data-ttu-id="430de-127">string</span><span class="sxs-lookup"><span data-stu-id="430de-127">string</span></span>| <span data-ttu-id="430de-128">只读</span><span class="sxs-lookup"><span data-stu-id="430de-128">Read-only</span></span>|
|<span data-ttu-id="430de-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="430de-129">riskEventDateTime</span></span>|<span data-ttu-id="430de-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430de-130">dateTimeOffset</span></span>| <span data-ttu-id="430de-131">风险事件发生的日期和时间</span><span class="sxs-lookup"><span data-stu-id="430de-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="430de-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="430de-132">riskEventStatus</span></span>|<span data-ttu-id="430de-133">string</span><span class="sxs-lookup"><span data-stu-id="430de-133">string</span></span>| <span data-ttu-id="430de-134">可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。</span><span class="sxs-lookup"><span data-stu-id="430de-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="430de-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="430de-135">riskLevel</span></span>|<span data-ttu-id="430de-136">string</span><span class="sxs-lookup"><span data-stu-id="430de-136">string</span></span>| <span data-ttu-id="430de-137">可取值为：`low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="430de-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="430de-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="430de-138">riskEventType</span></span>|<span data-ttu-id="430de-139">string</span><span class="sxs-lookup"><span data-stu-id="430de-139">string</span></span>| <span data-ttu-id="430de-140">风险的类型</span><span class="sxs-lookup"><span data-stu-id="430de-140">The type of risk</span></span>|
|<span data-ttu-id="430de-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="430de-141">userDisplayName</span></span>|<span data-ttu-id="430de-142">string</span><span class="sxs-lookup"><span data-stu-id="430de-142">string</span></span>| <span data-ttu-id="430de-143">具有风险的用户的名称</span><span class="sxs-lookup"><span data-stu-id="430de-143">The name of the user at risk</span></span>|
|<span data-ttu-id="430de-144">userId</span><span class="sxs-lookup"><span data-stu-id="430de-144">userId</span></span>|<span data-ttu-id="430de-145">string</span><span class="sxs-lookup"><span data-stu-id="430de-145">string</span></span>| <span data-ttu-id="430de-146">用户面临风险的 id</span><span class="sxs-lookup"><span data-stu-id="430de-146">The id of the user at risk</span></span>|
|<span data-ttu-id="430de-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="430de-147">userPrincipalName</span></span>|<span data-ttu-id="430de-148">string</span><span class="sxs-lookup"><span data-stu-id="430de-148">string</span></span>| <span data-ttu-id="430de-149">用户面临风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="430de-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="430de-150">关系</span><span class="sxs-lookup"><span data-stu-id="430de-150">Relationships</span></span>
| <span data-ttu-id="430de-151">关系</span><span class="sxs-lookup"><span data-stu-id="430de-151">Relationship</span></span> | <span data-ttu-id="430de-152">类型</span><span class="sxs-lookup"><span data-stu-id="430de-152">Type</span></span>   |<span data-ttu-id="430de-153">说明</span><span class="sxs-lookup"><span data-stu-id="430de-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="430de-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="430de-154">impactedUser</span></span>|[<span data-ttu-id="430de-155">用户</span><span class="sxs-lookup"><span data-stu-id="430de-155">user</span></span>](user.md)| <span data-ttu-id="430de-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="430de-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="430de-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="430de-158">JSON representation</span></span>

<span data-ttu-id="430de-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="430de-159">Here is a JSON representation of the resource.</span></span>

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
