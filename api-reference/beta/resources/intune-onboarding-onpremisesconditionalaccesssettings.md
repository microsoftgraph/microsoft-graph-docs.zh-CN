---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 196dcb136b85059b9c97d56ae3de9acc07eac5b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421646"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="8d18c-103">onPremisesConditionalAccessSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d18c-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="8d18c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8d18c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d18c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d18c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d18c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d18c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d18c-107">表示租户的 Exchange 本地条件访问设置的单例实体。</span><span class="sxs-lookup"><span data-stu-id="8d18c-107">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="8d18c-108">方法</span><span class="sxs-lookup"><span data-stu-id="8d18c-108">Methods</span></span>
|<span data-ttu-id="8d18c-109">方法</span><span class="sxs-lookup"><span data-stu-id="8d18c-109">Method</span></span>|<span data-ttu-id="8d18c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d18c-110">Return Type</span></span>|<span data-ttu-id="8d18c-111">说明</span><span class="sxs-lookup"><span data-stu-id="8d18c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8d18c-112">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8d18c-112">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="8d18c-113">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8d18c-113">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="8d18c-114">读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d18c-114">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="8d18c-115">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8d18c-115">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="8d18c-116">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8d18c-116">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="8d18c-117">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8d18c-117">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d18c-118">属性</span><span class="sxs-lookup"><span data-stu-id="8d18c-118">Properties</span></span>
|<span data-ttu-id="8d18c-119">属性</span><span class="sxs-lookup"><span data-stu-id="8d18c-119">Property</span></span>|<span data-ttu-id="8d18c-120">类型</span><span class="sxs-lookup"><span data-stu-id="8d18c-120">Type</span></span>|<span data-ttu-id="8d18c-121">说明</span><span class="sxs-lookup"><span data-stu-id="8d18c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d18c-122">id</span><span class="sxs-lookup"><span data-stu-id="8d18c-122">id</span></span>|<span data-ttu-id="8d18c-123">String</span><span class="sxs-lookup"><span data-stu-id="8d18c-123">String</span></span>|<span data-ttu-id="8d18c-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d18c-124">Not yet documented</span></span>|
|<span data-ttu-id="8d18c-125">enabled</span><span class="sxs-lookup"><span data-stu-id="8d18c-125">enabled</span></span>|<span data-ttu-id="8d18c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d18c-126">Boolean</span></span>|<span data-ttu-id="8d18c-127">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="8d18c-127">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="8d18c-128">includedGroups</span><span class="sxs-lookup"><span data-stu-id="8d18c-128">includedGroups</span></span>|<span data-ttu-id="8d18c-129">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="8d18c-129">Guid collection</span></span>|<span data-ttu-id="8d18c-130">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="8d18c-130">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="8d18c-131">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="8d18c-131">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="8d18c-132">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="8d18c-132">excludedGroups</span></span>|<span data-ttu-id="8d18c-133">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="8d18c-133">Guid collection</span></span>|<span data-ttu-id="8d18c-134">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="8d18c-134">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="8d18c-135">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="8d18c-135">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="8d18c-136">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="8d18c-136">overrideDefaultRule</span></span>|<span data-ttu-id="8d18c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d18c-137">Boolean</span></span>|<span data-ttu-id="8d18c-138">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="8d18c-138">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d18c-139">关系</span><span class="sxs-lookup"><span data-stu-id="8d18c-139">Relationships</span></span>
<span data-ttu-id="8d18c-140">无</span><span class="sxs-lookup"><span data-stu-id="8d18c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d18c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d18c-141">JSON Representation</span></span>
<span data-ttu-id="8d18c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d18c-142">Here is a JSON representation of the resource.</span></span>
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




