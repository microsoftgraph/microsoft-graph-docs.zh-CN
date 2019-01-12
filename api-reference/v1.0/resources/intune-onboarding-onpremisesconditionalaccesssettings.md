---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d39d7da372c562c12dd15c702d7f7e6f161a67a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970288"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="99e18-103">onPremisesConditionalAccessSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="99e18-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="99e18-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99e18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99e18-105">表示租户的 Exchange 本地条件访问设置的单例实体。</span><span class="sxs-lookup"><span data-stu-id="99e18-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="99e18-106">方法</span><span class="sxs-lookup"><span data-stu-id="99e18-106">Methods</span></span>
|<span data-ttu-id="99e18-107">方法</span><span class="sxs-lookup"><span data-stu-id="99e18-107">Method</span></span>|<span data-ttu-id="99e18-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="99e18-108">Return Type</span></span>|<span data-ttu-id="99e18-109">说明</span><span class="sxs-lookup"><span data-stu-id="99e18-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99e18-110">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="99e18-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="99e18-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="99e18-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="99e18-112">读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99e18-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="99e18-113">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="99e18-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="99e18-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="99e18-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="99e18-115">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99e18-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99e18-116">属性</span><span class="sxs-lookup"><span data-stu-id="99e18-116">Properties</span></span>
|<span data-ttu-id="99e18-117">属性</span><span class="sxs-lookup"><span data-stu-id="99e18-117">Property</span></span>|<span data-ttu-id="99e18-118">类型</span><span class="sxs-lookup"><span data-stu-id="99e18-118">Type</span></span>|<span data-ttu-id="99e18-119">说明</span><span class="sxs-lookup"><span data-stu-id="99e18-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99e18-120">id</span><span class="sxs-lookup"><span data-stu-id="99e18-120">id</span></span>|<span data-ttu-id="99e18-121">字符串</span><span class="sxs-lookup"><span data-stu-id="99e18-121">String</span></span>|<span data-ttu-id="99e18-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99e18-122">Not yet documented</span></span>|
|<span data-ttu-id="99e18-123">enabled</span><span class="sxs-lookup"><span data-stu-id="99e18-123">enabled</span></span>|<span data-ttu-id="99e18-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="99e18-124">Boolean</span></span>|<span data-ttu-id="99e18-125">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="99e18-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="99e18-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="99e18-126">includedGroups</span></span>|<span data-ttu-id="99e18-127">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="99e18-127">Guid collection</span></span>|<span data-ttu-id="99e18-128">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="99e18-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="99e18-129">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="99e18-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="99e18-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="99e18-130">excludedGroups</span></span>|<span data-ttu-id="99e18-131">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="99e18-131">Guid collection</span></span>|<span data-ttu-id="99e18-132">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="99e18-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="99e18-133">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="99e18-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="99e18-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="99e18-134">overrideDefaultRule</span></span>|<span data-ttu-id="99e18-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="99e18-135">Boolean</span></span>|<span data-ttu-id="99e18-136">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="99e18-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99e18-137">关系</span><span class="sxs-lookup"><span data-stu-id="99e18-137">Relationships</span></span>
<span data-ttu-id="99e18-138">无</span><span class="sxs-lookup"><span data-stu-id="99e18-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99e18-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99e18-139">JSON Representation</span></span>
<span data-ttu-id="99e18-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99e18-140">Here is a JSON representation of the resource.</span></span>
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



