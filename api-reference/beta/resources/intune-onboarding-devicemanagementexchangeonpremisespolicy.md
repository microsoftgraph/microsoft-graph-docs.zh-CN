---
title: deviceManagementExchangeOnPremisesPolicy 资源类型
description: 代表为租户配置的 Exchange OnPremises 策略 singleton 实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 516b2d96ab365e4f04102472f3118d29823d32be
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398574"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a><span data-ttu-id="54002-103">deviceManagementExchangeOnPremisesPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="54002-103">deviceManagementExchangeOnPremisesPolicy resource type</span></span>

> <span data-ttu-id="54002-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="54002-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54002-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54002-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54002-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54002-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54002-107">代表为租户配置的 Exchange OnPremises 策略 singleton 实体。</span><span class="sxs-lookup"><span data-stu-id="54002-107">Singleton entity which represents the Exchange OnPremises policy configured for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="54002-108">方法</span><span class="sxs-lookup"><span data-stu-id="54002-108">Methods</span></span>
|<span data-ttu-id="54002-109">方法</span><span class="sxs-lookup"><span data-stu-id="54002-109">Method</span></span>|<span data-ttu-id="54002-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="54002-110">Return Type</span></span>|<span data-ttu-id="54002-111">说明</span><span class="sxs-lookup"><span data-stu-id="54002-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54002-112">获取 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="54002-112">Get deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[<span data-ttu-id="54002-113">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="54002-113">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="54002-114">读取属性和[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="54002-114">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|
|[<span data-ttu-id="54002-115">更新 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="54002-115">Update deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[<span data-ttu-id="54002-116">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="54002-116">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="54002-117">更新[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="54002-117">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54002-118">属性</span><span class="sxs-lookup"><span data-stu-id="54002-118">Properties</span></span>
|<span data-ttu-id="54002-119">属性</span><span class="sxs-lookup"><span data-stu-id="54002-119">Property</span></span>|<span data-ttu-id="54002-120">类型</span><span class="sxs-lookup"><span data-stu-id="54002-120">Type</span></span>|<span data-ttu-id="54002-121">说明</span><span class="sxs-lookup"><span data-stu-id="54002-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54002-122">id</span><span class="sxs-lookup"><span data-stu-id="54002-122">id</span></span>|<span data-ttu-id="54002-123">String</span><span class="sxs-lookup"><span data-stu-id="54002-123">String</span></span>|<span data-ttu-id="54002-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="54002-124">Not yet documented</span></span>|
|<span data-ttu-id="54002-125">notificationContent</span><span class="sxs-lookup"><span data-stu-id="54002-125">notificationContent</span></span>|<span data-ttu-id="54002-126">Binary</span><span class="sxs-lookup"><span data-stu-id="54002-126">Binary</span></span>|<span data-ttu-id="54002-127">将发送到隔离通过此策略的用户的通知文本。</span><span class="sxs-lookup"><span data-stu-id="54002-127">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="54002-128">这是 UTF8 编码字节数组 HTML。</span><span class="sxs-lookup"><span data-stu-id="54002-128">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="54002-129">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="54002-129">defaultAccessLevel</span></span>|[<span data-ttu-id="54002-130">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="54002-130">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="54002-131">Exchange 中的默认访问状态。</span><span class="sxs-lookup"><span data-stu-id="54002-131">Default access state in Exchange.</span></span> <span data-ttu-id="54002-132">此规则全局适用于整个 Exchange 组织。</span><span class="sxs-lookup"><span data-stu-id="54002-132">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="54002-133">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="54002-133">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="54002-134">accessRules</span><span class="sxs-lookup"><span data-stu-id="54002-134">accessRules</span></span>|<span data-ttu-id="54002-135">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="54002-135">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="54002-136">在 Exchange 规则设备访问的列表。</span><span class="sxs-lookup"><span data-stu-id="54002-136">The list of device access rules in Exchange.</span></span> <span data-ttu-id="54002-137">访问规则应用于整个 Exchange 组织的全局</span><span class="sxs-lookup"><span data-stu-id="54002-137">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="54002-138">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="54002-138">knownDeviceClasses</span></span>|<span data-ttu-id="54002-139">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)集合</span><span class="sxs-lookup"><span data-stu-id="54002-139">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="54002-140">已知到 Exchange 的设备类列表</span><span class="sxs-lookup"><span data-stu-id="54002-140">The list of device classes known to Exchange</span></span>|

## <a name="relationships"></a><span data-ttu-id="54002-141">关系</span><span class="sxs-lookup"><span data-stu-id="54002-141">Relationships</span></span>
|<span data-ttu-id="54002-142">关系</span><span class="sxs-lookup"><span data-stu-id="54002-142">Relationship</span></span>|<span data-ttu-id="54002-143">类型</span><span class="sxs-lookup"><span data-stu-id="54002-143">Type</span></span>|<span data-ttu-id="54002-144">说明</span><span class="sxs-lookup"><span data-stu-id="54002-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54002-145">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="54002-145">conditionalAccessSettings</span></span>|[<span data-ttu-id="54002-146">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="54002-146">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="54002-147">Exchange 本地条件访问设置。</span><span class="sxs-lookup"><span data-stu-id="54002-147">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="54002-148">本地条件访问需要设备注册并符合邮件访问要求</span><span class="sxs-lookup"><span data-stu-id="54002-148">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54002-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54002-149">JSON Representation</span></span>
<span data-ttu-id="54002-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54002-150">Here is a JSON representation of the resource.</span></span>
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




