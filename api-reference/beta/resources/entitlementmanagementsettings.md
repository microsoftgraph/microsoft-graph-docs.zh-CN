---
title: entitlementManagementSettings 资源类型
description: 表示 Azure AD 权限管理的租户范围的设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f34740bd5e16bb001cd3618edf4c4b669155f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052881"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="4cfa9-103">entitlementManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cfa9-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="4cfa9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cfa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cfa9-105">表示控制 [AZURE AD 权限管理](entitlementmanagement-root.md)行为的设置。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4cfa9-106">方法</span><span class="sxs-lookup"><span data-stu-id="4cfa9-106">Methods</span></span>

| <span data-ttu-id="4cfa9-107">方法</span><span class="sxs-lookup"><span data-stu-id="4cfa9-107">Method</span></span>       | <span data-ttu-id="4cfa9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4cfa9-108">Return Type</span></span> | <span data-ttu-id="4cfa9-109">说明</span><span class="sxs-lookup"><span data-stu-id="4cfa9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4cfa9-110">获取</span><span class="sxs-lookup"><span data-stu-id="4cfa9-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="4cfa9-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="4cfa9-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="4cfa9-112">读取 **entitlementManagementSettings** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="4cfa9-113">更新</span><span class="sxs-lookup"><span data-stu-id="4cfa9-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="4cfa9-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="4cfa9-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="4cfa9-115">更新 **entitlementManagementSettings** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4cfa9-116">属性</span><span class="sxs-lookup"><span data-stu-id="4cfa9-116">Properties</span></span>

| <span data-ttu-id="4cfa9-117">属性</span><span class="sxs-lookup"><span data-stu-id="4cfa9-117">Property</span></span>     | <span data-ttu-id="4cfa9-118">类型</span><span class="sxs-lookup"><span data-stu-id="4cfa9-118">Type</span></span>        | <span data-ttu-id="4cfa9-119">说明</span><span class="sxs-lookup"><span data-stu-id="4cfa9-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4cfa9-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="4cfa9-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="4cfa9-121">String</span><span class="sxs-lookup"><span data-stu-id="4cfa9-121">String</span></span>|<span data-ttu-id="4cfa9-122">`None`、、或中的一个 `BlockSignIn` `BlockSignInAndDelete` 。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="4cfa9-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="4cfa9-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="4cfa9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4cfa9-124">Int64</span></span>|<span data-ttu-id="4cfa9-125">如果 `externalUserLifecycleAction` 为 `BlockSignInAndDelete` ，则在删除外部用户的帐户之前，阻止外部用户登录的天数。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cfa9-126">关系</span><span class="sxs-lookup"><span data-stu-id="4cfa9-126">Relationships</span></span>

<span data-ttu-id="4cfa9-127">无。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cfa9-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cfa9-128">JSON representation</span></span>

<span data-ttu-id="4cfa9-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cfa9-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "baseType": "",
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


