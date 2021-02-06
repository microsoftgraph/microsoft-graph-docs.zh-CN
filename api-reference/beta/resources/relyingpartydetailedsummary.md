---
title: relyingPartyDetailedSummary 资源类型
description: 表示 AD FS 中的信赖方。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c1c0195302c4b01e39a6223797567c750807e9f6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136225"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="929b7-103">relyingPartyDetailedSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="929b7-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="929b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="929b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="929b7-105">表示使用 Active Directory 联合身份验证服务 (AD FS) 配置的信赖方、其聚合使用情况，以及信赖方配置是否可以迁移到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="929b7-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="929b7-106">方法</span><span class="sxs-lookup"><span data-stu-id="929b7-106">Methods</span></span>

| <span data-ttu-id="929b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="929b7-107">Method</span></span>       | <span data-ttu-id="929b7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="929b7-108">Return Type</span></span> | <span data-ttu-id="929b7-109">Description</span><span class="sxs-lookup"><span data-stu-id="929b7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="929b7-110">List</span><span class="sxs-lookup"><span data-stu-id="929b7-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="929b7-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="929b7-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="929b7-112">检索 **relyyPartyDetailedSummary 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="929b7-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="929b7-113">属性</span><span class="sxs-lookup"><span data-stu-id="929b7-113">Properties</span></span>

| <span data-ttu-id="929b7-114">属性</span><span class="sxs-lookup"><span data-stu-id="929b7-114">Property</span></span>     | <span data-ttu-id="929b7-115">类型</span><span class="sxs-lookup"><span data-stu-id="929b7-115">Type</span></span>        | <span data-ttu-id="929b7-116">说明</span><span class="sxs-lookup"><span data-stu-id="929b7-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="929b7-117">id</span><span class="sxs-lookup"><span data-stu-id="929b7-117">id</span></span>|<span data-ttu-id="929b7-118">字符串</span><span class="sxs-lookup"><span data-stu-id="929b7-118">String</span></span>| <span data-ttu-id="929b7-119">只读。</span><span class="sxs-lookup"><span data-stu-id="929b7-119">Read-only.</span></span> <span data-ttu-id="929b7-120">在 API 级别生成的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="929b7-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="929b7-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="929b7-121">relyingPartyId</span></span>|<span data-ttu-id="929b7-122">字符串</span><span class="sxs-lookup"><span data-stu-id="929b7-122">String</span></span>|<span data-ttu-id="929b7-123">此标识符用于标识此联合身份验证服务的信赖方。</span><span class="sxs-lookup"><span data-stu-id="929b7-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="929b7-124">它用于向信赖方发出声明。</span><span class="sxs-lookup"><span data-stu-id="929b7-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="929b7-125">服务 Id</span><span class="sxs-lookup"><span data-stu-id="929b7-125">serviceId</span></span>|<span data-ttu-id="929b7-126">字符串</span><span class="sxs-lookup"><span data-stu-id="929b7-126">String</span></span>|<span data-ttu-id="929b7-127">唯一标识 Active Directory 林。</span><span class="sxs-lookup"><span data-stu-id="929b7-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="929b7-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="929b7-128">migrationStatus</span></span>|<span data-ttu-id="929b7-129">string</span><span class="sxs-lookup"><span data-stu-id="929b7-129">string</span></span>| <span data-ttu-id="929b7-130">指示应用程序是否可以移动到 Azure AD 或需要进行更多调查。</span><span class="sxs-lookup"><span data-stu-id="929b7-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="929b7-131">可取值为：`ready`、`needsReview`、`additionalStepsRequired`。</span><span class="sxs-lookup"><span data-stu-id="929b7-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="929b7-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="929b7-132">migrationValidationDetails</span></span>|<span data-ttu-id="929b7-133">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="929b7-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="929b7-134">指定对应用程序配置详细信息执行的所有验证检查，以评估应用程序是否已准备好移动到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="929b7-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="929b7-135">可能的名称是： `AdditionalWSFedEndpointCheckResult` ， ， ， ， ， ， ， ，  `AllowedAuthenticationClassReferencesCheckResult` ， `AlwaysRequireAuthenticationCheckResult`   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` 。</span><span class="sxs-lookup"><span data-stu-id="929b7-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="929b7-136">可能的结果值为 `0` ， `1` 或 `2` 。</span><span class="sxs-lookup"><span data-stu-id="929b7-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="929b7-137">`0` 验证检查通过时、 `1` 验证检查失败时以及验证 `2` 检查为警告时。</span><span class="sxs-lookup"><span data-stu-id="929b7-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="929b7-138">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="929b7-138">relyingPartyName</span></span>|<span data-ttu-id="929b7-139">字符串</span><span class="sxs-lookup"><span data-stu-id="929b7-139">String</span></span>|<span data-ttu-id="929b7-140">Internet 上使用标识提供程序对想要登录的用户进行身份验证的应用程序或其他实体的名称。</span><span class="sxs-lookup"><span data-stu-id="929b7-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="929b7-141">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="929b7-141">failedSignInCount</span></span>|<span data-ttu-id="929b7-142">Int64</span><span class="sxs-lookup"><span data-stu-id="929b7-142">Int64</span></span>| <span data-ttu-id="929b7-143">指定时段内 Active Directory 联合身份验证服务登录失败的数量。</span><span class="sxs-lookup"><span data-stu-id="929b7-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="929b7-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="929b7-144">replyUrls</span></span>|<span data-ttu-id="929b7-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="929b7-145">String collection</span></span>|<span data-ttu-id="929b7-146">指定信赖方希望在何处接收令牌。</span><span class="sxs-lookup"><span data-stu-id="929b7-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="929b7-147">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="929b7-147">signInSuccessRate</span></span>|<span data-ttu-id="929b7-148">双精度</span><span class="sxs-lookup"><span data-stu-id="929b7-148">Double</span></span>|<span data-ttu-id="929b7-149">在指定的 (Active Directory 联合身份验证服务上成功登录) 成功登录数 + 失败登录数。</span><span class="sxs-lookup"><span data-stu-id="929b7-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="929b7-150">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="929b7-150">successfulSignInCount</span></span>|<span data-ttu-id="929b7-151">Int64</span><span class="sxs-lookup"><span data-stu-id="929b7-151">Int64</span></span>|<span data-ttu-id="929b7-152">Active Directory 联合身份验证服务上成功登录的数量。</span><span class="sxs-lookup"><span data-stu-id="929b7-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="929b7-153">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="929b7-153">totalSignInCount</span></span>|<span data-ttu-id="929b7-154">Int64</span><span class="sxs-lookup"><span data-stu-id="929b7-154">Int64</span></span>|<span data-ttu-id="929b7-155">指定时段内 Active Directory 联合身份验证服务上登录成功 + 失败登录失败的数量。</span><span class="sxs-lookup"><span data-stu-id="929b7-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="929b7-156">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="929b7-156">uniqueUserCount</span></span>|<span data-ttu-id="929b7-157">Int64</span><span class="sxs-lookup"><span data-stu-id="929b7-157">Int64</span></span>|<span data-ttu-id="929b7-158">已登录到应用程序的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="929b7-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="929b7-159">关系</span><span class="sxs-lookup"><span data-stu-id="929b7-159">Relationships</span></span>

<span data-ttu-id="929b7-160">无。</span><span class="sxs-lookup"><span data-stu-id="929b7-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="929b7-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="929b7-161">JSON representation</span></span>

<span data-ttu-id="929b7-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="929b7-162">The following is a JSON representation of the resource.</span></span>

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


