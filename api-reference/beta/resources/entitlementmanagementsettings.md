---
title: entitlementManagementSettings 资源类型
description: 表示 Azure AD 权利管理的租户范围设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d5cc340837f173924802196bf12c9a63f26949a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159120"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="c2909-103">entitlementManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2909-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="c2909-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2909-105">表示控制 [Azure AD 权利管理行为的设置](entitlementmanagement-root.md)。</span><span class="sxs-lookup"><span data-stu-id="c2909-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c2909-106">方法</span><span class="sxs-lookup"><span data-stu-id="c2909-106">Methods</span></span>

| <span data-ttu-id="c2909-107">方法</span><span class="sxs-lookup"><span data-stu-id="c2909-107">Method</span></span>       | <span data-ttu-id="c2909-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2909-108">Return Type</span></span> | <span data-ttu-id="c2909-109">说明</span><span class="sxs-lookup"><span data-stu-id="c2909-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c2909-110">Get</span><span class="sxs-lookup"><span data-stu-id="c2909-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="c2909-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c2909-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="c2909-112">读取 **entitlementManagementSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="c2909-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="c2909-113">更新</span><span class="sxs-lookup"><span data-stu-id="c2909-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="c2909-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c2909-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="c2909-115">更新 **entitlementManagementSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="c2909-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2909-116">属性</span><span class="sxs-lookup"><span data-stu-id="c2909-116">Properties</span></span>

| <span data-ttu-id="c2909-117">属性</span><span class="sxs-lookup"><span data-stu-id="c2909-117">Property</span></span>     | <span data-ttu-id="c2909-118">类型</span><span class="sxs-lookup"><span data-stu-id="c2909-118">Type</span></span>        | <span data-ttu-id="c2909-119">说明</span><span class="sxs-lookup"><span data-stu-id="c2909-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2909-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="c2909-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="c2909-121">String</span><span class="sxs-lookup"><span data-stu-id="c2909-121">String</span></span>|<span data-ttu-id="c2909-122">之 `None` 一 `BlockSignIn` ， 或 `BlockSignInAndDelete` 。</span><span class="sxs-lookup"><span data-stu-id="c2909-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="c2909-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="c2909-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="c2909-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c2909-124">Int64</span></span>|<span data-ttu-id="c2909-125">如果为 ，则当外部用户的帐户被删除之前，阻止其 `externalUserLifecycleAction` `BlockSignInAndDelete` 登录的天数。</span><span class="sxs-lookup"><span data-stu-id="c2909-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2909-126">关系</span><span class="sxs-lookup"><span data-stu-id="c2909-126">Relationships</span></span>

<span data-ttu-id="c2909-127">无。</span><span class="sxs-lookup"><span data-stu-id="c2909-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2909-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2909-128">JSON representation</span></span>

<span data-ttu-id="c2909-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2909-129">The following is a JSON representation of the resource.</span></span>

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


