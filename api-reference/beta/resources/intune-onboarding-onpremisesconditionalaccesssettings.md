---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf378696795689b618f5ec18ebb668028e00804d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029433"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="49894-103">onPremisesConditionalAccessSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="49894-103">onPremisesConditionalAccessSettings resource type</span></span>

<span data-ttu-id="49894-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49894-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49894-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49894-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49894-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49894-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49894-107">表示租户的 Exchange 本地条件访问设置的单例实体。</span><span class="sxs-lookup"><span data-stu-id="49894-107">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="49894-108">方法</span><span class="sxs-lookup"><span data-stu-id="49894-108">Methods</span></span>
|<span data-ttu-id="49894-109">方法</span><span class="sxs-lookup"><span data-stu-id="49894-109">Method</span></span>|<span data-ttu-id="49894-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="49894-110">Return Type</span></span>|<span data-ttu-id="49894-111">说明</span><span class="sxs-lookup"><span data-stu-id="49894-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49894-112">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49894-112">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="49894-113">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49894-113">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="49894-114">读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49894-114">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="49894-115">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49894-115">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="49894-116">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="49894-116">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="49894-117">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="49894-117">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="49894-118">属性</span><span class="sxs-lookup"><span data-stu-id="49894-118">Properties</span></span>
|<span data-ttu-id="49894-119">属性</span><span class="sxs-lookup"><span data-stu-id="49894-119">Property</span></span>|<span data-ttu-id="49894-120">类型</span><span class="sxs-lookup"><span data-stu-id="49894-120">Type</span></span>|<span data-ttu-id="49894-121">说明</span><span class="sxs-lookup"><span data-stu-id="49894-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49894-122">id</span><span class="sxs-lookup"><span data-stu-id="49894-122">id</span></span>|<span data-ttu-id="49894-123">String</span><span class="sxs-lookup"><span data-stu-id="49894-123">String</span></span>|<span data-ttu-id="49894-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49894-124">Not yet documented</span></span>|
|<span data-ttu-id="49894-125">enabled</span><span class="sxs-lookup"><span data-stu-id="49894-125">enabled</span></span>|<span data-ttu-id="49894-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="49894-126">Boolean</span></span>|<span data-ttu-id="49894-127">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="49894-127">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="49894-128">includedGroups</span><span class="sxs-lookup"><span data-stu-id="49894-128">includedGroups</span></span>|<span data-ttu-id="49894-129">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="49894-129">Guid collection</span></span>|<span data-ttu-id="49894-130">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="49894-130">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="49894-131">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="49894-131">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="49894-132">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="49894-132">excludedGroups</span></span>|<span data-ttu-id="49894-133">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="49894-133">Guid collection</span></span>|<span data-ttu-id="49894-134">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="49894-134">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="49894-135">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="49894-135">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="49894-136">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="49894-136">overrideDefaultRule</span></span>|<span data-ttu-id="49894-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="49894-137">Boolean</span></span>|<span data-ttu-id="49894-138">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="49894-138">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49894-139">关系</span><span class="sxs-lookup"><span data-stu-id="49894-139">Relationships</span></span>
<span data-ttu-id="49894-140">无</span><span class="sxs-lookup"><span data-stu-id="49894-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49894-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49894-141">JSON Representation</span></span>
<span data-ttu-id="49894-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49894-142">Here is a JSON representation of the resource.</span></span>
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






