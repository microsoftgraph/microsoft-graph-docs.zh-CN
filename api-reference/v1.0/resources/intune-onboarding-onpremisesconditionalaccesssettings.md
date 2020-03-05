---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fda9b2c4e8dff366fc347ea145ba627e6c764ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448037"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="c55bd-103">onPremisesConditionalAccessSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c55bd-103">onPremisesConditionalAccessSettings resource type</span></span>

<span data-ttu-id="c55bd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c55bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c55bd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c55bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c55bd-106">表示租户的 Exchange 本地条件访问设置的单例实体。</span><span class="sxs-lookup"><span data-stu-id="c55bd-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="c55bd-107">方法</span><span class="sxs-lookup"><span data-stu-id="c55bd-107">Methods</span></span>
|<span data-ttu-id="c55bd-108">方法</span><span class="sxs-lookup"><span data-stu-id="c55bd-108">Method</span></span>|<span data-ttu-id="c55bd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c55bd-109">Return Type</span></span>|<span data-ttu-id="c55bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="c55bd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c55bd-111">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="c55bd-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="c55bd-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="c55bd-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="c55bd-113">读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c55bd-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="c55bd-114">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="c55bd-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="c55bd-115">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="c55bd-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="c55bd-116">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c55bd-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c55bd-117">属性</span><span class="sxs-lookup"><span data-stu-id="c55bd-117">Properties</span></span>
|<span data-ttu-id="c55bd-118">属性</span><span class="sxs-lookup"><span data-stu-id="c55bd-118">Property</span></span>|<span data-ttu-id="c55bd-119">类型</span><span class="sxs-lookup"><span data-stu-id="c55bd-119">Type</span></span>|<span data-ttu-id="c55bd-120">说明</span><span class="sxs-lookup"><span data-stu-id="c55bd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c55bd-121">id</span><span class="sxs-lookup"><span data-stu-id="c55bd-121">id</span></span>|<span data-ttu-id="c55bd-122">String</span><span class="sxs-lookup"><span data-stu-id="c55bd-122">String</span></span>|<span data-ttu-id="c55bd-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c55bd-123">Not yet documented</span></span>|
|<span data-ttu-id="c55bd-124">enabled</span><span class="sxs-lookup"><span data-stu-id="c55bd-124">enabled</span></span>|<span data-ttu-id="c55bd-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="c55bd-125">Boolean</span></span>|<span data-ttu-id="c55bd-126">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="c55bd-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="c55bd-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="c55bd-127">includedGroups</span></span>|<span data-ttu-id="c55bd-128">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="c55bd-128">Guid collection</span></span>|<span data-ttu-id="c55bd-129">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="c55bd-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="c55bd-130">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="c55bd-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="c55bd-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="c55bd-131">excludedGroups</span></span>|<span data-ttu-id="c55bd-132">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="c55bd-132">Guid collection</span></span>|<span data-ttu-id="c55bd-133">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="c55bd-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="c55bd-134">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="c55bd-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="c55bd-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="c55bd-135">overrideDefaultRule</span></span>|<span data-ttu-id="c55bd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55bd-136">Boolean</span></span>|<span data-ttu-id="c55bd-137">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="c55bd-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c55bd-138">关系</span><span class="sxs-lookup"><span data-stu-id="c55bd-138">Relationships</span></span>
<span data-ttu-id="c55bd-139">无</span><span class="sxs-lookup"><span data-stu-id="c55bd-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c55bd-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c55bd-140">JSON Representation</span></span>
<span data-ttu-id="c55bd-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c55bd-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```




