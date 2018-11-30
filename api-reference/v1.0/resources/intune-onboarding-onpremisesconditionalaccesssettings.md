---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
ms.openlocfilehash: 903a3e6a3fafd837fc8c5caf55eb57d23ddd0d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009694"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="ad568-103">onPremisesConditionalAccessSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad568-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="ad568-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ad568-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad568-105">表示租户的 Exchange 本地条件访问设置的单例实体。</span><span class="sxs-lookup"><span data-stu-id="ad568-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="ad568-106">方法</span><span class="sxs-lookup"><span data-stu-id="ad568-106">Methods</span></span>
|<span data-ttu-id="ad568-107">方法</span><span class="sxs-lookup"><span data-stu-id="ad568-107">Method</span></span>|<span data-ttu-id="ad568-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ad568-108">Return Type</span></span>|<span data-ttu-id="ad568-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad568-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ad568-110">获取 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ad568-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="ad568-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ad568-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ad568-112">读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad568-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="ad568-113">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ad568-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="ad568-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ad568-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ad568-115">更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad568-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad568-116">属性</span><span class="sxs-lookup"><span data-stu-id="ad568-116">Properties</span></span>
|<span data-ttu-id="ad568-117">属性</span><span class="sxs-lookup"><span data-stu-id="ad568-117">Property</span></span>|<span data-ttu-id="ad568-118">类型</span><span class="sxs-lookup"><span data-stu-id="ad568-118">Type</span></span>|<span data-ttu-id="ad568-119">说明</span><span class="sxs-lookup"><span data-stu-id="ad568-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad568-120">id</span><span class="sxs-lookup"><span data-stu-id="ad568-120">id</span></span>|<span data-ttu-id="ad568-121">字符串</span><span class="sxs-lookup"><span data-stu-id="ad568-121">String</span></span>|<span data-ttu-id="ad568-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ad568-122">Not yet documented</span></span>|
|<span data-ttu-id="ad568-123">enabled</span><span class="sxs-lookup"><span data-stu-id="ad568-123">enabled</span></span>|<span data-ttu-id="ad568-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad568-124">Boolean</span></span>|<span data-ttu-id="ad568-125">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="ad568-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="ad568-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="ad568-126">includedGroups</span></span>|<span data-ttu-id="ad568-127">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="ad568-127">Guid collection</span></span>|<span data-ttu-id="ad568-128">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="ad568-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="ad568-129">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="ad568-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="ad568-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="ad568-130">excludedGroups</span></span>|<span data-ttu-id="ad568-131">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="ad568-131">Guid collection</span></span>|<span data-ttu-id="ad568-132">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="ad568-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="ad568-133">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="ad568-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="ad568-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="ad568-134">overrideDefaultRule</span></span>|<span data-ttu-id="ad568-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad568-135">Boolean</span></span>|<span data-ttu-id="ad568-136">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="ad568-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad568-137">关系</span><span class="sxs-lookup"><span data-stu-id="ad568-137">Relationships</span></span>
<span data-ttu-id="ad568-138">无</span><span class="sxs-lookup"><span data-stu-id="ad568-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad568-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad568-139">JSON Representation</span></span>
<span data-ttu-id="ad568-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad568-140">Here is a JSON representation of the resource.</span></span>
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



