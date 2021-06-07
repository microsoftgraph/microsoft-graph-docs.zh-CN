---
title: deviceAppManagement 资源类型
description: 设备应用管理单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8906e96a0218360bbe78d1c08dd4d8767568775
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751839"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="060ef-103">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="060ef-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="060ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="060ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="060ef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="060ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060ef-106">设备应用管理单例实体。</span><span class="sxs-lookup"><span data-stu-id="060ef-106">Device app management singleton entity.</span></span>

## <a name="methods"></a><span data-ttu-id="060ef-107">方法</span><span class="sxs-lookup"><span data-stu-id="060ef-107">Methods</span></span>
|<span data-ttu-id="060ef-108">方法</span><span class="sxs-lookup"><span data-stu-id="060ef-108">Method</span></span>|<span data-ttu-id="060ef-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="060ef-109">Return Type</span></span>|<span data-ttu-id="060ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="060ef-110">Description</span></span>|
|:---|:---|:---|

## <a name="properties"></a><span data-ttu-id="060ef-111">属性</span><span class="sxs-lookup"><span data-stu-id="060ef-111">Properties</span></span>
|<span data-ttu-id="060ef-112">属性</span><span class="sxs-lookup"><span data-stu-id="060ef-112">Property</span></span>|<span data-ttu-id="060ef-113">类型</span><span class="sxs-lookup"><span data-stu-id="060ef-113">Type</span></span>|<span data-ttu-id="060ef-114">说明</span><span class="sxs-lookup"><span data-stu-id="060ef-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="060ef-115">id</span><span class="sxs-lookup"><span data-stu-id="060ef-115">id</span></span>|<span data-ttu-id="060ef-116">String</span><span class="sxs-lookup"><span data-stu-id="060ef-116">String</span></span>|<span data-ttu-id="060ef-117">实体的键。</span><span class="sxs-lookup"><span data-stu-id="060ef-117">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="060ef-118">关系</span><span class="sxs-lookup"><span data-stu-id="060ef-118">Relationships</span></span>
|<span data-ttu-id="060ef-119">关系</span><span class="sxs-lookup"><span data-stu-id="060ef-119">Relationship</span></span>|<span data-ttu-id="060ef-120">类型</span><span class="sxs-lookup"><span data-stu-id="060ef-120">Type</span></span>|<span data-ttu-id="060ef-121">说明</span><span class="sxs-lookup"><span data-stu-id="060ef-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="060ef-122">managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="060ef-122">managedAppPolicies</span></span>|<span data-ttu-id="060ef-123">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-123">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="060ef-124">托管应用策略。</span><span class="sxs-lookup"><span data-stu-id="060ef-124">Managed app policies.</span></span>|
|<span data-ttu-id="060ef-125">iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="060ef-125">iosManagedAppProtections</span></span>|<span data-ttu-id="060ef-126">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-126">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) collection</span></span>|<span data-ttu-id="060ef-127">iOS 托管应用策略。</span><span class="sxs-lookup"><span data-stu-id="060ef-127">iOS managed app policies.</span></span>|
|<span data-ttu-id="060ef-128">androidManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="060ef-128">androidManagedAppProtections</span></span>|<span data-ttu-id="060ef-129">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-129">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) collection</span></span>|<span data-ttu-id="060ef-130">Android 托管应用策略。</span><span class="sxs-lookup"><span data-stu-id="060ef-130">Android managed app policies.</span></span>|
|<span data-ttu-id="060ef-131">defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="060ef-131">defaultManagedAppProtections</span></span>|<span data-ttu-id="060ef-132">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-132">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) collection</span></span>|<span data-ttu-id="060ef-133">默认的托管应用策略。</span><span class="sxs-lookup"><span data-stu-id="060ef-133">Default managed app policies.</span></span>|
|<span data-ttu-id="060ef-134">targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="060ef-134">targetedManagedAppConfigurations</span></span>|<span data-ttu-id="060ef-135">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-135">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="060ef-136">托管应用配置目标。</span><span class="sxs-lookup"><span data-stu-id="060ef-136">Targeted managed app configurations.</span></span>|
|<span data-ttu-id="060ef-137">mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="060ef-137">mdmWindowsInformationProtectionPolicies</span></span>|<span data-ttu-id="060ef-138">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-138">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="060ef-139">对已注册 MDM 的设备上运行的应用的 Windows 信息保护。</span><span class="sxs-lookup"><span data-stu-id="060ef-139">Windows information protection for apps running on devices which are MDM enrolled.</span></span>|
|<span data-ttu-id="060ef-140">windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="060ef-140">windowsInformationProtectionPolicies</span></span>|<span data-ttu-id="060ef-141">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-141">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) collection</span></span>|<span data-ttu-id="060ef-142">对未注册 MDM 的设备上运行的应用的 Windows 信息保护。</span><span class="sxs-lookup"><span data-stu-id="060ef-142">Windows information protection for apps running on devices which are not MDM enrolled.</span></span>|
|<span data-ttu-id="060ef-143">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="060ef-143">managedAppRegistrations</span></span>|<span data-ttu-id="060ef-144">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-144">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="060ef-145">托管应用注册。</span><span class="sxs-lookup"><span data-stu-id="060ef-145">The managed app registrations.</span></span>|
|<span data-ttu-id="060ef-146">managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="060ef-146">managedAppStatuses</span></span>|<span data-ttu-id="060ef-147">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="060ef-147">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="060ef-148">托管应用状态。</span><span class="sxs-lookup"><span data-stu-id="060ef-148">The managed app statuses.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="060ef-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="060ef-149">JSON Representation</span></span>
<span data-ttu-id="060ef-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="060ef-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




