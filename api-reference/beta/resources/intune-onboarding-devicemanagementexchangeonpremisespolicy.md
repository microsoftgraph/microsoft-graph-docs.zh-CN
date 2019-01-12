---
title: deviceManagementExchangeOnPremisesPolicy 资源类型
description: 代表为租户配置的 Exchange OnPremises 策略 singleton 实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c4f513242694228b53268772d9b2910fa40bbd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990332"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a><span data-ttu-id="07354-103">deviceManagementExchangeOnPremisesPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="07354-103">deviceManagementExchangeOnPremisesPolicy resource type</span></span>

> <span data-ttu-id="07354-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="07354-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07354-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="07354-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07354-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="07354-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07354-107">代表为租户配置的 Exchange OnPremises 策略 singleton 实体。</span><span class="sxs-lookup"><span data-stu-id="07354-107">Singleton entity which represents the Exchange OnPremises policy configured for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="07354-108">方法</span><span class="sxs-lookup"><span data-stu-id="07354-108">Methods</span></span>
|<span data-ttu-id="07354-109">方法</span><span class="sxs-lookup"><span data-stu-id="07354-109">Method</span></span>|<span data-ttu-id="07354-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="07354-110">Return Type</span></span>|<span data-ttu-id="07354-111">说明</span><span class="sxs-lookup"><span data-stu-id="07354-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07354-112">获取 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="07354-112">Get deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[<span data-ttu-id="07354-113">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="07354-113">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="07354-114">读取属性和[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="07354-114">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|
|[<span data-ttu-id="07354-115">更新 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="07354-115">Update deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[<span data-ttu-id="07354-116">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="07354-116">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="07354-117">更新[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07354-117">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07354-118">属性</span><span class="sxs-lookup"><span data-stu-id="07354-118">Properties</span></span>
|<span data-ttu-id="07354-119">属性</span><span class="sxs-lookup"><span data-stu-id="07354-119">Property</span></span>|<span data-ttu-id="07354-120">类型</span><span class="sxs-lookup"><span data-stu-id="07354-120">Type</span></span>|<span data-ttu-id="07354-121">说明</span><span class="sxs-lookup"><span data-stu-id="07354-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07354-122">id</span><span class="sxs-lookup"><span data-stu-id="07354-122">id</span></span>|<span data-ttu-id="07354-123">字符串</span><span class="sxs-lookup"><span data-stu-id="07354-123">String</span></span>|<span data-ttu-id="07354-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="07354-124">Not yet documented</span></span>|
|<span data-ttu-id="07354-125">notificationContent</span><span class="sxs-lookup"><span data-stu-id="07354-125">notificationContent</span></span>|<span data-ttu-id="07354-126">Binary</span><span class="sxs-lookup"><span data-stu-id="07354-126">Binary</span></span>|<span data-ttu-id="07354-127">将发送到隔离通过此策略的用户的通知文本。</span><span class="sxs-lookup"><span data-stu-id="07354-127">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="07354-128">这是 UTF8 编码字节数组 HTML。</span><span class="sxs-lookup"><span data-stu-id="07354-128">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="07354-129">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="07354-129">defaultAccessLevel</span></span>|[<span data-ttu-id="07354-130">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="07354-130">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="07354-131">Exchange 中的默认访问状态。</span><span class="sxs-lookup"><span data-stu-id="07354-131">Default access state in Exchange.</span></span> <span data-ttu-id="07354-132">此规则全局适用于整个 Exchange 组织。</span><span class="sxs-lookup"><span data-stu-id="07354-132">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="07354-133">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="07354-133">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="07354-134">accessRules</span><span class="sxs-lookup"><span data-stu-id="07354-134">accessRules</span></span>|<span data-ttu-id="07354-135">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="07354-135">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="07354-136">在 Exchange 规则设备访问的列表。</span><span class="sxs-lookup"><span data-stu-id="07354-136">The list of device access rules in Exchange.</span></span> <span data-ttu-id="07354-137">访问规则应用于整个 Exchange 组织的全局</span><span class="sxs-lookup"><span data-stu-id="07354-137">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="07354-138">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="07354-138">knownDeviceClasses</span></span>|<span data-ttu-id="07354-139">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)集合</span><span class="sxs-lookup"><span data-stu-id="07354-139">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="07354-140">已知到 Exchange 的设备类列表</span><span class="sxs-lookup"><span data-stu-id="07354-140">The list of device classes known to Exchange</span></span>|

## <a name="relationships"></a><span data-ttu-id="07354-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="07354-141">Relationships</span></span>
|<span data-ttu-id="07354-142">关系</span><span class="sxs-lookup"><span data-stu-id="07354-142">Relationship</span></span>|<span data-ttu-id="07354-143">类型</span><span class="sxs-lookup"><span data-stu-id="07354-143">Type</span></span>|<span data-ttu-id="07354-144">说明</span><span class="sxs-lookup"><span data-stu-id="07354-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07354-145">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="07354-145">conditionalAccessSettings</span></span>|[<span data-ttu-id="07354-146">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="07354-146">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="07354-147">Exchange 本地条件访问设置。</span><span class="sxs-lookup"><span data-stu-id="07354-147">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="07354-148">本地条件访问需要设备注册并符合邮件访问要求</span><span class="sxs-lookup"><span data-stu-id="07354-148">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07354-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07354-149">JSON Representation</span></span>
<span data-ttu-id="07354-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07354-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```





