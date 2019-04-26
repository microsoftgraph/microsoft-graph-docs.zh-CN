---
title: managedDeviceMobileAppConfigurationUserStatus 资源类型
description: 包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cd2f0a697f8535d07afb9d30d11efed315941d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552140"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a><span data-ttu-id="e4f05-103">managedDeviceMobileAppConfigurationUserStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4f05-103">managedDeviceMobileAppConfigurationUserStatus resource type</span></span>

> <span data-ttu-id="e4f05-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4f05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4f05-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4f05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4f05-106">包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="e4f05-106">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="e4f05-107">方法</span><span class="sxs-lookup"><span data-stu-id="e4f05-107">Methods</span></span>
|<span data-ttu-id="e4f05-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4f05-108">Method</span></span>|<span data-ttu-id="e4f05-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4f05-109">Return Type</span></span>|<span data-ttu-id="e4f05-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4f05-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4f05-111">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="e4f05-111">List managedDeviceMobileAppConfigurationUserStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|<span data-ttu-id="e4f05-112">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4f05-112">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="e4f05-113">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4f05-113">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>|
|[<span data-ttu-id="e4f05-114">获取 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-114">Get managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[<span data-ttu-id="e4f05-115">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-115">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="e4f05-116">读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4f05-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="e4f05-117">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-117">Create managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[<span data-ttu-id="e4f05-118">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-118">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="e4f05-119">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4f05-119">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="e4f05-120">删除 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-120">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|<span data-ttu-id="e4f05-121">无</span><span class="sxs-lookup"><span data-stu-id="e4f05-121">None</span></span>|<span data-ttu-id="e4f05-122">删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="e4f05-122">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>|
|[<span data-ttu-id="e4f05-123">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-123">Update managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[<span data-ttu-id="e4f05-124">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-124">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="e4f05-125">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4f05-125">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4f05-126">属性</span><span class="sxs-lookup"><span data-stu-id="e4f05-126">Properties</span></span>
|<span data-ttu-id="e4f05-127">属性</span><span class="sxs-lookup"><span data-stu-id="e4f05-127">Property</span></span>|<span data-ttu-id="e4f05-128">类型</span><span class="sxs-lookup"><span data-stu-id="e4f05-128">Type</span></span>|<span data-ttu-id="e4f05-129">说明</span><span class="sxs-lookup"><span data-stu-id="e4f05-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4f05-130">id</span><span class="sxs-lookup"><span data-stu-id="e4f05-130">id</span></span>|<span data-ttu-id="e4f05-131">字符串</span><span class="sxs-lookup"><span data-stu-id="e4f05-131">String</span></span>|<span data-ttu-id="e4f05-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e4f05-132">Key of the entity.</span></span>|
|<span data-ttu-id="e4f05-133">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e4f05-133">userDisplayName</span></span>|<span data-ttu-id="e4f05-134">String</span><span class="sxs-lookup"><span data-stu-id="e4f05-134">String</span></span>|<span data-ttu-id="e4f05-135">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="e4f05-135">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="e4f05-136">devicesCount</span><span class="sxs-lookup"><span data-stu-id="e4f05-136">devicesCount</span></span>|<span data-ttu-id="e4f05-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f05-137">Int32</span></span>|<span data-ttu-id="e4f05-138">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="e4f05-138">Devices count for that user.</span></span>|
|<span data-ttu-id="e4f05-139">status</span><span class="sxs-lookup"><span data-stu-id="e4f05-139">status</span></span>|[<span data-ttu-id="e4f05-140">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e4f05-140">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e4f05-141">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="e4f05-141">Compliance status of the policy report.</span></span> <span data-ttu-id="e4f05-142">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="e4f05-142">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e4f05-143">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4f05-143">lastReportedDateTime</span></span>|<span data-ttu-id="e4f05-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4f05-144">DateTimeOffset</span></span>|<span data-ttu-id="e4f05-145">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="e4f05-145">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="e4f05-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e4f05-146">userPrincipalName</span></span>|<span data-ttu-id="e4f05-147">String</span><span class="sxs-lookup"><span data-stu-id="e4f05-147">String</span></span>|<span data-ttu-id="e4f05-148">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="e4f05-148">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4f05-149">关系</span><span class="sxs-lookup"><span data-stu-id="e4f05-149">Relationships</span></span>
<span data-ttu-id="e4f05-150">无</span><span class="sxs-lookup"><span data-stu-id="e4f05-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4f05-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4f05-151">JSON Representation</span></span>
<span data-ttu-id="e4f05-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f05-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





