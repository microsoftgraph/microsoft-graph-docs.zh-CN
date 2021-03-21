---
title: relyingPartyDetailedSummary 资源类型
description: 表示 AD FS 中的信赖方。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6e840c47ed5170f95929d686fe9ff94be54ea1ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962110"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="1c8c5-103">relyingPartyDetailedSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c8c5-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="1c8c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c8c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c8c5-105">表示使用 Active Directory 联合身份验证服务 (AD FS) 配置的信赖方、其聚合使用情况，以及信赖方配置是否可以迁移到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="1c8c5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1c8c5-106">Methods</span></span>

| <span data-ttu-id="1c8c5-107">方法</span><span class="sxs-lookup"><span data-stu-id="1c8c5-107">Method</span></span>       | <span data-ttu-id="1c8c5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c8c5-108">Return Type</span></span> | <span data-ttu-id="1c8c5-109">Description</span><span class="sxs-lookup"><span data-stu-id="1c8c5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1c8c5-110">List</span><span class="sxs-lookup"><span data-stu-id="1c8c5-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="1c8c5-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="1c8c5-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="1c8c5-112">检索 **relyingPartyDetailedSummary 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="1c8c5-113">属性</span><span class="sxs-lookup"><span data-stu-id="1c8c5-113">Properties</span></span>

| <span data-ttu-id="1c8c5-114">属性</span><span class="sxs-lookup"><span data-stu-id="1c8c5-114">Property</span></span>     | <span data-ttu-id="1c8c5-115">类型</span><span class="sxs-lookup"><span data-stu-id="1c8c5-115">Type</span></span>        | <span data-ttu-id="1c8c5-116">说明</span><span class="sxs-lookup"><span data-stu-id="1c8c5-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c8c5-117">id</span><span class="sxs-lookup"><span data-stu-id="1c8c5-117">id</span></span>|<span data-ttu-id="1c8c5-118">String</span><span class="sxs-lookup"><span data-stu-id="1c8c5-118">String</span></span>| <span data-ttu-id="1c8c5-119">只读。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-119">Read-only.</span></span> <span data-ttu-id="1c8c5-120">在 API 级别生成的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="1c8c5-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="1c8c5-121">relyingPartyId</span></span>|<span data-ttu-id="1c8c5-122">String</span><span class="sxs-lookup"><span data-stu-id="1c8c5-122">String</span></span>|<span data-ttu-id="1c8c5-123">此标识符用于标识此联合身份验证服务的信赖方。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="1c8c5-124">向信赖方发出声明时，会使用声明。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="1c8c5-125">服务 Id</span><span class="sxs-lookup"><span data-stu-id="1c8c5-125">serviceId</span></span>|<span data-ttu-id="1c8c5-126">String</span><span class="sxs-lookup"><span data-stu-id="1c8c5-126">String</span></span>|<span data-ttu-id="1c8c5-127">唯一标识 Active Directory 林。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="1c8c5-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="1c8c5-128">migrationStatus</span></span>|<span data-ttu-id="1c8c5-129">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="1c8c5-129">migrationStatus</span></span>| <span data-ttu-id="1c8c5-130">指示应用程序是否可以移动到 Azure AD 或需要更多调查。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="1c8c5-131">可取值为：`ready`、`needsReview`、`additionalStepsRequired`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1c8c5-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="1c8c5-132">migrationValidationDetails</span></span>|<span data-ttu-id="1c8c5-133">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c8c5-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="1c8c5-134">指定在应用程序配置详细信息上完成的所有验证检查，以评估应用程序是否已准备好移动到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span>|
|<span data-ttu-id="1c8c5-135">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="1c8c5-135">relyingPartyName</span></span>|<span data-ttu-id="1c8c5-136">String</span><span class="sxs-lookup"><span data-stu-id="1c8c5-136">String</span></span>|<span data-ttu-id="1c8c5-137">Internet 上使用标识提供程序对要登录的用户进行身份验证的应用程序或其他实体的名称。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-137">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="1c8c5-138">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="1c8c5-138">failedSignInCount</span></span>|<span data-ttu-id="1c8c5-139">Int64</span><span class="sxs-lookup"><span data-stu-id="1c8c5-139">Int64</span></span>| <span data-ttu-id="1c8c5-140">指定时段内 Active Directory 联合身份验证服务上的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-140">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="1c8c5-141">replyUrls</span><span class="sxs-lookup"><span data-stu-id="1c8c5-141">replyUrls</span></span>|<span data-ttu-id="1c8c5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1c8c5-142">String collection</span></span>|<span data-ttu-id="1c8c5-143">指定信赖方期望接收令牌的地方。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-143">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="1c8c5-144">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="1c8c5-144">signInSuccessRate</span></span>|<span data-ttu-id="1c8c5-145">双精度</span><span class="sxs-lookup"><span data-stu-id="1c8c5-145">Double</span></span>|<span data-ttu-id="1c8c5-146">在指定的 (Active Directory 联合身份验证服务上成功登录数) 登录失败次数 + 失败次数。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-146">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="1c8c5-147">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="1c8c5-147">successfulSignInCount</span></span>|<span data-ttu-id="1c8c5-148">Int64</span><span class="sxs-lookup"><span data-stu-id="1c8c5-148">Int64</span></span>|<span data-ttu-id="1c8c5-149">Active Directory 联合身份验证服务上成功登录的数量。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-149">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="1c8c5-150">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="1c8c5-150">totalSignInCount</span></span>|<span data-ttu-id="1c8c5-151">Int64</span><span class="sxs-lookup"><span data-stu-id="1c8c5-151">Int64</span></span>|<span data-ttu-id="1c8c5-152">指定时段内 Active Directory 联合身份验证服务的成功登录数 + 登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-152">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="1c8c5-153">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="1c8c5-153">uniqueUserCount</span></span>|<span data-ttu-id="1c8c5-154">Int64</span><span class="sxs-lookup"><span data-stu-id="1c8c5-154">Int64</span></span>|<span data-ttu-id="1c8c5-155">已登录到应用程序的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-155">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c8c5-156">关系</span><span class="sxs-lookup"><span data-stu-id="1c8c5-156">Relationships</span></span>

<span data-ttu-id="1c8c5-157">无。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c8c5-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c8c5-158">JSON representation</span></span>

<span data-ttu-id="1c8c5-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c8c5-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
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


