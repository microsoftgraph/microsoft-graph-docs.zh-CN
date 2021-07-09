---
title: entitlementManagementSettings 资源类型
description: 表示 Azure AD 权利管理的租户范围设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d34a04d0f8eb3bdff16befd43870b75d473a8d0c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350976"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="532be-103">entitlementManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="532be-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="532be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="532be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="532be-105">表示控制 [Azure AD 权利管理行为的设置](entitlementmanagement-root.md)。</span><span class="sxs-lookup"><span data-stu-id="532be-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>  <span data-ttu-id="532be-106">此资源不包括目录创建者设置;若要查看或更改目录创建者角色成员身份，请使用角色 [分配](unifiedroleassignment.md) API 和权利管理 RBAC 提供程序。</span><span class="sxs-lookup"><span data-stu-id="532be-106">This resource does not include the catalog creators setting; to view or change the catalog creators role membership, use the [role assignments](unifiedroleassignment.md) API with the entitlement management RBAC provider.</span></span>

## <a name="methods"></a><span data-ttu-id="532be-107">方法</span><span class="sxs-lookup"><span data-stu-id="532be-107">Methods</span></span>

| <span data-ttu-id="532be-108">方法</span><span class="sxs-lookup"><span data-stu-id="532be-108">Method</span></span>       | <span data-ttu-id="532be-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="532be-109">Return Type</span></span> | <span data-ttu-id="532be-110">说明</span><span class="sxs-lookup"><span data-stu-id="532be-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="532be-111">Get</span><span class="sxs-lookup"><span data-stu-id="532be-111">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="532be-112">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="532be-112">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="532be-113">读取 **entitlementManagementSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="532be-113">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="532be-114">更新</span><span class="sxs-lookup"><span data-stu-id="532be-114">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="532be-115">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="532be-115">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="532be-116">更新 **entitlementManagementSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="532be-116">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="532be-117">属性</span><span class="sxs-lookup"><span data-stu-id="532be-117">Properties</span></span>

| <span data-ttu-id="532be-118">属性</span><span class="sxs-lookup"><span data-stu-id="532be-118">Property</span></span>     | <span data-ttu-id="532be-119">类型</span><span class="sxs-lookup"><span data-stu-id="532be-119">Type</span></span>        | <span data-ttu-id="532be-120">说明</span><span class="sxs-lookup"><span data-stu-id="532be-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="532be-121">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="532be-121">externalUserLifecycleAction</span></span>|<span data-ttu-id="532be-122">字符串</span><span class="sxs-lookup"><span data-stu-id="532be-122">String</span></span>|<span data-ttu-id="532be-123">、 `None` `BlockSignIn` 或 `BlockSignInAndDelete` 之一。</span><span class="sxs-lookup"><span data-stu-id="532be-123">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="532be-124">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="532be-124">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="532be-125">Int64</span><span class="sxs-lookup"><span data-stu-id="532be-125">Int64</span></span>|<span data-ttu-id="532be-126">如果 **externalUserLifecycleAction** 为 ，则外部用户在删除其帐户之前被阻止 `BlockSignInAndDelete` 登录的天数。</span><span class="sxs-lookup"><span data-stu-id="532be-126">If **externalUserLifecycleAction** is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="532be-127">关系</span><span class="sxs-lookup"><span data-stu-id="532be-127">Relationships</span></span>

<span data-ttu-id="532be-128">无。</span><span class="sxs-lookup"><span data-stu-id="532be-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="532be-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="532be-129">JSON representation</span></span>

<span data-ttu-id="532be-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="532be-130">The following is a JSON representation of the resource.</span></span>

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


