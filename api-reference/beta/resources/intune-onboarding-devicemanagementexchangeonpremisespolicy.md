---
title: deviceManagementExchangeOnPremisesPolicy 资源类型
description: 表示为租户配置的 Exchange OnPremises 策略的单一实例实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05548aef02888268fa93e92fd5aeea3cfaed93a6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958688"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a><span data-ttu-id="9cf69-103">deviceManagementExchangeOnPremisesPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cf69-103">deviceManagementExchangeOnPremisesPolicy resource type</span></span>

> <span data-ttu-id="9cf69-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9cf69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf69-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9cf69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf69-106">表示为租户配置的 Exchange OnPremises 策略的单一实例实体。</span><span class="sxs-lookup"><span data-stu-id="9cf69-106">Singleton entity which represents the Exchange OnPremises policy configured for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="9cf69-107">方法</span><span class="sxs-lookup"><span data-stu-id="9cf69-107">Methods</span></span>
|<span data-ttu-id="9cf69-108">方法</span><span class="sxs-lookup"><span data-stu-id="9cf69-108">Method</span></span>|<span data-ttu-id="9cf69-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9cf69-109">Return Type</span></span>|<span data-ttu-id="9cf69-110">说明</span><span class="sxs-lookup"><span data-stu-id="9cf69-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9cf69-111">获取 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="9cf69-111">Get deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[<span data-ttu-id="9cf69-112">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="9cf69-112">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="9cf69-113">读取[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9cf69-113">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|
|[<span data-ttu-id="9cf69-114">更新 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="9cf69-114">Update deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[<span data-ttu-id="9cf69-115">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="9cf69-115">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="9cf69-116">更新[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9cf69-116">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9cf69-117">属性</span><span class="sxs-lookup"><span data-stu-id="9cf69-117">Properties</span></span>
|<span data-ttu-id="9cf69-118">属性</span><span class="sxs-lookup"><span data-stu-id="9cf69-118">Property</span></span>|<span data-ttu-id="9cf69-119">类型</span><span class="sxs-lookup"><span data-stu-id="9cf69-119">Type</span></span>|<span data-ttu-id="9cf69-120">说明</span><span class="sxs-lookup"><span data-stu-id="9cf69-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf69-121">id</span><span class="sxs-lookup"><span data-stu-id="9cf69-121">id</span></span>|<span data-ttu-id="9cf69-122">String</span><span class="sxs-lookup"><span data-stu-id="9cf69-122">String</span></span>|<span data-ttu-id="9cf69-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9cf69-123">Not yet documented</span></span>|
|<span data-ttu-id="9cf69-124">notificationContent</span><span class="sxs-lookup"><span data-stu-id="9cf69-124">notificationContent</span></span>|<span data-ttu-id="9cf69-125">Binary</span><span class="sxs-lookup"><span data-stu-id="9cf69-125">Binary</span></span>|<span data-ttu-id="9cf69-126">将发送给此策略隔离的用户的通知文本。</span><span class="sxs-lookup"><span data-stu-id="9cf69-126">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="9cf69-127">这是 UTF8 编码的字节数组 HTML。</span><span class="sxs-lookup"><span data-stu-id="9cf69-127">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="9cf69-128">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="9cf69-128">defaultAccessLevel</span></span>|[<span data-ttu-id="9cf69-129">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="9cf69-129">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="9cf69-130">Exchange 中的默认访问状态。</span><span class="sxs-lookup"><span data-stu-id="9cf69-130">Default access state in Exchange.</span></span> <span data-ttu-id="9cf69-131">此规则全局应用于整个 Exchange 组织。</span><span class="sxs-lookup"><span data-stu-id="9cf69-131">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="9cf69-132">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="9cf69-132">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="9cf69-133">accessRules</span><span class="sxs-lookup"><span data-stu-id="9cf69-133">accessRules</span></span>|<span data-ttu-id="9cf69-134">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="9cf69-134">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="9cf69-135">Exchange 中的设备访问规则列表。</span><span class="sxs-lookup"><span data-stu-id="9cf69-135">The list of device access rules in Exchange.</span></span> <span data-ttu-id="9cf69-136">访问规则全局应用于整个 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="9cf69-136">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="9cf69-137">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="9cf69-137">knownDeviceClasses</span></span>|<span data-ttu-id="9cf69-138">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)集合</span><span class="sxs-lookup"><span data-stu-id="9cf69-138">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="9cf69-139">已知的 Exchange 设备类别的列表</span><span class="sxs-lookup"><span data-stu-id="9cf69-139">The list of device classes known to Exchange</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cf69-140">关系</span><span class="sxs-lookup"><span data-stu-id="9cf69-140">Relationships</span></span>
|<span data-ttu-id="9cf69-141">关系</span><span class="sxs-lookup"><span data-stu-id="9cf69-141">Relationship</span></span>|<span data-ttu-id="9cf69-142">类型</span><span class="sxs-lookup"><span data-stu-id="9cf69-142">Type</span></span>|<span data-ttu-id="9cf69-143">说明</span><span class="sxs-lookup"><span data-stu-id="9cf69-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf69-144">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="9cf69-144">conditionalAccessSettings</span></span>|[<span data-ttu-id="9cf69-145">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="9cf69-145">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="9cf69-146">Exchange 本地条件访问设置。</span><span class="sxs-lookup"><span data-stu-id="9cf69-146">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="9cf69-147">本地条件访问需要设备注册并符合邮件访问要求</span><span class="sxs-lookup"><span data-stu-id="9cf69-147">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cf69-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cf69-148">JSON Representation</span></span>
<span data-ttu-id="9cf69-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cf69-149">Here is a JSON representation of the resource.</span></span>
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





