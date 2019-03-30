---
title: riskyUsers 资源类型
description: 表示有风险的 Azure AD 用户。 Azure AD 会根据各种信号和机器学习持续评估用户风险。 此 API 提供对 Azure AD 中所有风险用户的编程访问。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003718"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="28ff9-105">riskyUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="28ff9-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28ff9-106">表示有风险的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="28ff9-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="28ff9-107">Azure AD 会根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="28ff9-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="28ff9-108">此 API 提供对 Azure AD 中所有风险用户的编程访问。</span><span class="sxs-lookup"><span data-stu-id="28ff9-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="28ff9-109">有关风险事件的详细信息, 请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="28ff9-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="28ff9-110">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="28ff9-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="28ff9-111">方法</span><span class="sxs-lookup"><span data-stu-id="28ff9-111">Methods</span></span>

| <span data-ttu-id="28ff9-112">方法</span><span class="sxs-lookup"><span data-stu-id="28ff9-112">Method</span></span>   | <span data-ttu-id="28ff9-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="28ff9-113">Return Type</span></span>|<span data-ttu-id="28ff9-114">说明</span><span class="sxs-lookup"><span data-stu-id="28ff9-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28ff9-115">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="28ff9-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="28ff9-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="28ff9-116">riskyUsers</span></span>](riskyUser.md) |<span data-ttu-id="28ff9-117">列出有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="28ff9-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="28ff9-118">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="28ff9-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="28ff9-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="28ff9-119">riskyUsers</span></span>](riskyUser.md)|<span data-ttu-id="28ff9-120">获取特定的有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="28ff9-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="28ff9-121">确认 riskyUsers 已泄露</span><span class="sxs-lookup"><span data-stu-id="28ff9-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="28ff9-122">确认有风险的用户受到威胁。</span><span class="sxs-lookup"><span data-stu-id="28ff9-122">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="28ff9-123">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="28ff9-123">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="28ff9-124">消除有风险的用户的风险。</span><span class="sxs-lookup"><span data-stu-id="28ff9-124">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="28ff9-125">属性</span><span class="sxs-lookup"><span data-stu-id="28ff9-125">Properties</span></span>

| <span data-ttu-id="28ff9-126">属性</span><span class="sxs-lookup"><span data-stu-id="28ff9-126">Property</span></span>   | <span data-ttu-id="28ff9-127">类型</span><span class="sxs-lookup"><span data-stu-id="28ff9-127">Type</span></span>|<span data-ttu-id="28ff9-128">说明</span><span class="sxs-lookup"><span data-stu-id="28ff9-128">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="28ff9-129">用户面临风险的唯一 id</span><span class="sxs-lookup"><span data-stu-id="28ff9-129">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="28ff9-130">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="28ff9-130">Indicates whether the user is deleted.</span></span> <span data-ttu-id="28ff9-131">可能的值包括`true`:、`false`</span><span class="sxs-lookup"><span data-stu-id="28ff9-131">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="28ff9-132">指示用户是否为来宾用户。</span><span class="sxs-lookup"><span data-stu-id="28ff9-132">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="28ff9-133">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="28ff9-133">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="28ff9-134">如此如果用户的标识位于租户外部, 请考虑。</span><span class="sxs-lookup"><span data-stu-id="28ff9-134">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="28ff9-135">此用户可以是在 Azure AD、MSA 或第三方标识提供程序中具有标识的 B2B 或 B2C 用户。</span><span class="sxs-lookup"><span data-stu-id="28ff9-135">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="28ff9-136">假如果用户的标识位于租户内部, 则考虑</span><span class="sxs-lookup"><span data-stu-id="28ff9-136">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="28ff9-137">指示后端正在处理用户的危险状态 wehther</span><span class="sxs-lookup"><span data-stu-id="28ff9-137">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`risk`|[<span data-ttu-id="28ff9-138">冒</span><span class="sxs-lookup"><span data-stu-id="28ff9-138">risk</span></span>](risk.md)|<span data-ttu-id="28ff9-139">有风险的用户状态</span><span class="sxs-lookup"><span data-stu-id="28ff9-139">Risky user state</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="28ff9-140">上次更新有风险的用户的日期和时间</span><span class="sxs-lookup"><span data-stu-id="28ff9-140">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="28ff9-141">有风险的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="28ff9-141">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="28ff9-142">有风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="28ff9-142">Risky user principal name</span></span>|


## <a name="json-representation"></a><span data-ttu-id="28ff9-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28ff9-143">JSON representation</span></span>

<span data-ttu-id="28ff9-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28ff9-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
