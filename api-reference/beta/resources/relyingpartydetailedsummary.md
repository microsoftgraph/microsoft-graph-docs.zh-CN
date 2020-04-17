---
title: relyingPartyDetailedSummary 资源类型
description: 表示 AD FS 中的信赖方。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 306c20c31120d2f130562993d8ebd2d7e4083c23
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543457"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="6749a-103">relyingPartyDetailedSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6749a-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="6749a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6749a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6749a-105">表示配置了 Active Directory 联合身份验证服务（AD FS）的信赖方、其聚合的使用情况，以及是否可以将信赖方配置迁移到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="6749a-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="6749a-106">方法</span><span class="sxs-lookup"><span data-stu-id="6749a-106">Methods</span></span>

| <span data-ttu-id="6749a-107">方法</span><span class="sxs-lookup"><span data-stu-id="6749a-107">Method</span></span>       | <span data-ttu-id="6749a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6749a-108">Return Type</span></span> | <span data-ttu-id="6749a-109">说明</span><span class="sxs-lookup"><span data-stu-id="6749a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6749a-110">List</span><span class="sxs-lookup"><span data-stu-id="6749a-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="6749a-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="6749a-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="6749a-112">检索**relyingPartyDetailedSummary**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6749a-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="6749a-113">属性</span><span class="sxs-lookup"><span data-stu-id="6749a-113">Properties</span></span>

| <span data-ttu-id="6749a-114">属性</span><span class="sxs-lookup"><span data-stu-id="6749a-114">Property</span></span>     | <span data-ttu-id="6749a-115">类型</span><span class="sxs-lookup"><span data-stu-id="6749a-115">Type</span></span>        | <span data-ttu-id="6749a-116">说明</span><span class="sxs-lookup"><span data-stu-id="6749a-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6749a-117">id</span><span class="sxs-lookup"><span data-stu-id="6749a-117">id</span></span>|<span data-ttu-id="6749a-118">String</span><span class="sxs-lookup"><span data-stu-id="6749a-118">String</span></span>| <span data-ttu-id="6749a-119">只读。</span><span class="sxs-lookup"><span data-stu-id="6749a-119">Read-only.</span></span> <span data-ttu-id="6749a-120">在 API 级别生成的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6749a-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="6749a-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="6749a-121">relyingPartyId</span></span>|<span data-ttu-id="6749a-122">String</span><span class="sxs-lookup"><span data-stu-id="6749a-122">String</span></span>|<span data-ttu-id="6749a-123">此标识符用于将信赖方标识为此联合身份验证服务。</span><span class="sxs-lookup"><span data-stu-id="6749a-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="6749a-124">向信赖方颁发声明时使用它。</span><span class="sxs-lookup"><span data-stu-id="6749a-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="6749a-125">服务 Id</span><span class="sxs-lookup"><span data-stu-id="6749a-125">serviceId</span></span>|<span data-ttu-id="6749a-126">String</span><span class="sxs-lookup"><span data-stu-id="6749a-126">String</span></span>|<span data-ttu-id="6749a-127">唯一标识 Active Directory 林。</span><span class="sxs-lookup"><span data-stu-id="6749a-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="6749a-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="6749a-128">migrationStatus</span></span>|<span data-ttu-id="6749a-129">string</span><span class="sxs-lookup"><span data-stu-id="6749a-129">string</span></span>| <span data-ttu-id="6749a-130">指示是否可以将应用程序移动到 Azure AD 或需要更多调查。</span><span class="sxs-lookup"><span data-stu-id="6749a-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="6749a-131">可取值为：`ready`、`needsReview`、`additionalStepsRequired`。</span><span class="sxs-lookup"><span data-stu-id="6749a-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="6749a-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="6749a-132">migrationValidationDetails</span></span>|<span data-ttu-id="6749a-133">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6749a-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="6749a-134">指定对应用程序配置详细信息进行的所有验证检查，以评估应用程序是否已准备好迁移到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="6749a-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="6749a-135">可能的名称为`AdditionalWSFedEndpointCheckResult`： `AllowedAuthenticationClassReferencesCheckResult`、 `AlwaysRequireAuthenticationCheckResult`、 `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult` `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult``NotBeforeSkewCheckResult` `RequestMFAFromClaimsProvidersCheckResult` `IssuanceTransformRulesCheckResult`、、 `SignedSamlRequestsRequiredCheckResult`、、、、、、、、、、、。 `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult` `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult`</span><span class="sxs-lookup"><span data-stu-id="6749a-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="6749a-136">可能的结果值`0`为`1`、或`2`。</span><span class="sxs-lookup"><span data-stu-id="6749a-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="6749a-137">`0`验证检查通过后， `1`验证检查失败，并且`2`在验证检查为警告时。</span><span class="sxs-lookup"><span data-stu-id="6749a-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="6749a-138">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="6749a-138">relyingPartyName</span></span>|<span data-ttu-id="6749a-139">String</span><span class="sxs-lookup"><span data-stu-id="6749a-139">String</span></span>|<span data-ttu-id="6749a-140">Internet 上的应用程序或其他实体的名称，该实体使用标识提供程序对要登录的用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6749a-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="6749a-141">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="6749a-141">failedSignInCount</span></span>|<span data-ttu-id="6749a-142">Int64</span><span class="sxs-lookup"><span data-stu-id="6749a-142">Int64</span></span>| <span data-ttu-id="6749a-143">在指定时间段内，在 Active Directory 联合身份验证服务上登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="6749a-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="6749a-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="6749a-144">replyUrls</span></span>|<span data-ttu-id="6749a-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="6749a-145">String collection</span></span>|<span data-ttu-id="6749a-146">指定信赖方预期接收令牌的位置。</span><span class="sxs-lookup"><span data-stu-id="6749a-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="6749a-147">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="6749a-147">signInSuccessRate</span></span>|<span data-ttu-id="6749a-148">双精度</span><span class="sxs-lookup"><span data-stu-id="6749a-148">Double</span></span>|<span data-ttu-id="6749a-149">在指定时间段内，Active Directory 联合身份验证服务上成功/（成功的登录失败次数）的数量。</span><span class="sxs-lookup"><span data-stu-id="6749a-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="6749a-150">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="6749a-150">successfulSignInCount</span></span>|<span data-ttu-id="6749a-151">Int64</span><span class="sxs-lookup"><span data-stu-id="6749a-151">Int64</span></span>|<span data-ttu-id="6749a-152">在 Active Directory 联合身份验证服务上成功登录的次数。</span><span class="sxs-lookup"><span data-stu-id="6749a-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="6749a-153">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="6749a-153">totalSignInCount</span></span>|<span data-ttu-id="6749a-154">Int64</span><span class="sxs-lookup"><span data-stu-id="6749a-154">Int64</span></span>|<span data-ttu-id="6749a-155">在指定时间段内，在 Active Directory 联合身份验证服务上成功的 + 失败登录登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="6749a-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="6749a-156">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="6749a-156">uniqueUserCount</span></span>|<span data-ttu-id="6749a-157">Int64</span><span class="sxs-lookup"><span data-stu-id="6749a-157">Int64</span></span>|<span data-ttu-id="6749a-158">已登录到应用程序的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="6749a-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6749a-159">关系</span><span class="sxs-lookup"><span data-stu-id="6749a-159">Relationships</span></span>

<span data-ttu-id="6749a-160">无。</span><span class="sxs-lookup"><span data-stu-id="6749a-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6749a-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6749a-161">JSON representation</span></span>

<span data-ttu-id="6749a-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6749a-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "failedSignInCount": 10,
  "id": "String (identifier)",
  "migrationStatus": "ready | needsReview | additionalStepsRequired",
  "migrationValidationDetails": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": ["String"],
  "serviceId": "String (identifier)",
  "signInSuccessRate": 90.0,
  "successfulSignInCount": 90,
  "totalSignInCount": 100,
  "uniqueUserCount": 10
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relyingPartyDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
