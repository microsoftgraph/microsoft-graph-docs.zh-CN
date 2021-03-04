---
title: entitlementManagementSettings 资源类型
description: 表示 Azure AD 权利管理的租户范围设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4b6ee584e671e070955eb7c065c59cb8481c375
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440351"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="50d13-103">entitlementManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="50d13-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="50d13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d13-105">表示控制 [Azure AD 权利管理行为的设置](entitlementmanagement-root.md)。</span><span class="sxs-lookup"><span data-stu-id="50d13-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="50d13-106">Methods</span><span class="sxs-lookup"><span data-stu-id="50d13-106">Methods</span></span>

| <span data-ttu-id="50d13-107">方法</span><span class="sxs-lookup"><span data-stu-id="50d13-107">Method</span></span>       | <span data-ttu-id="50d13-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="50d13-108">Return Type</span></span> | <span data-ttu-id="50d13-109">说明</span><span class="sxs-lookup"><span data-stu-id="50d13-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="50d13-110">获取</span><span class="sxs-lookup"><span data-stu-id="50d13-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="50d13-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="50d13-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="50d13-112">读取 **entitlementManagementSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="50d13-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="50d13-113">更新</span><span class="sxs-lookup"><span data-stu-id="50d13-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="50d13-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="50d13-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="50d13-115">更新 **entitlementManagementSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="50d13-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="50d13-116">属性</span><span class="sxs-lookup"><span data-stu-id="50d13-116">Properties</span></span>

| <span data-ttu-id="50d13-117">属性</span><span class="sxs-lookup"><span data-stu-id="50d13-117">Property</span></span>     | <span data-ttu-id="50d13-118">类型</span><span class="sxs-lookup"><span data-stu-id="50d13-118">Type</span></span>        | <span data-ttu-id="50d13-119">说明</span><span class="sxs-lookup"><span data-stu-id="50d13-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50d13-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="50d13-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="50d13-121">String</span><span class="sxs-lookup"><span data-stu-id="50d13-121">String</span></span>|<span data-ttu-id="50d13-122">之一 `None` `BlockSignIn` ， 或 `BlockSignInAndDelete` 。</span><span class="sxs-lookup"><span data-stu-id="50d13-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="50d13-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="50d13-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="50d13-124">Int64</span><span class="sxs-lookup"><span data-stu-id="50d13-124">Int64</span></span>|<span data-ttu-id="50d13-125">如果为 ，则删除外部用户的帐户之前阻止其 `externalUserLifecycleAction` `BlockSignInAndDelete` 登录的天数。</span><span class="sxs-lookup"><span data-stu-id="50d13-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50d13-126">关系</span><span class="sxs-lookup"><span data-stu-id="50d13-126">Relationships</span></span>

<span data-ttu-id="50d13-127">无。</span><span class="sxs-lookup"><span data-stu-id="50d13-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50d13-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50d13-128">JSON representation</span></span>

<span data-ttu-id="50d13-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50d13-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


