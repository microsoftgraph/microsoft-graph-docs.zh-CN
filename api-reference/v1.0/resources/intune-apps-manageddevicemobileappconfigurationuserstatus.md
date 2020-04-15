---
title: managedDeviceMobileAppConfigurationUserStatus 资源类型
description: 包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69a9d500fcf6e11c2df64bfb99cf3d7147f4cc8a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474203"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a><span data-ttu-id="05e56-103">managedDeviceMobileAppConfigurationUserStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="05e56-103">managedDeviceMobileAppConfigurationUserStatus resource type</span></span>

<span data-ttu-id="05e56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05e56-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05e56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05e56-106">包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="05e56-106">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="05e56-107">方法</span><span class="sxs-lookup"><span data-stu-id="05e56-107">Methods</span></span>
|<span data-ttu-id="05e56-108">方法</span><span class="sxs-lookup"><span data-stu-id="05e56-108">Method</span></span>|<span data-ttu-id="05e56-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="05e56-109">Return Type</span></span>|<span data-ttu-id="05e56-110">说明</span><span class="sxs-lookup"><span data-stu-id="05e56-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05e56-111">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="05e56-111">List managedDeviceMobileAppConfigurationUserStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|<span data-ttu-id="05e56-112">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="05e56-112">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="05e56-113">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05e56-113">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>|
|[<span data-ttu-id="05e56-114">获取 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-114">Get managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[<span data-ttu-id="05e56-115">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-115">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="05e56-116">读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05e56-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="05e56-117">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-117">Create managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[<span data-ttu-id="05e56-118">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-118">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="05e56-119">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05e56-119">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="05e56-120">删除 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-120">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|<span data-ttu-id="05e56-121">无</span><span class="sxs-lookup"><span data-stu-id="05e56-121">None</span></span>|<span data-ttu-id="05e56-122">删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="05e56-122">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>|
|[<span data-ttu-id="05e56-123">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-123">Update managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[<span data-ttu-id="05e56-124">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-124">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="05e56-125">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="05e56-125">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05e56-126">属性</span><span class="sxs-lookup"><span data-stu-id="05e56-126">Properties</span></span>
|<span data-ttu-id="05e56-127">属性</span><span class="sxs-lookup"><span data-stu-id="05e56-127">Property</span></span>|<span data-ttu-id="05e56-128">类型</span><span class="sxs-lookup"><span data-stu-id="05e56-128">Type</span></span>|<span data-ttu-id="05e56-129">说明</span><span class="sxs-lookup"><span data-stu-id="05e56-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05e56-130">id</span><span class="sxs-lookup"><span data-stu-id="05e56-130">id</span></span>|<span data-ttu-id="05e56-131">String</span><span class="sxs-lookup"><span data-stu-id="05e56-131">String</span></span>|<span data-ttu-id="05e56-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="05e56-132">Key of the entity.</span></span>|
|<span data-ttu-id="05e56-133">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="05e56-133">userDisplayName</span></span>|<span data-ttu-id="05e56-134">String</span><span class="sxs-lookup"><span data-stu-id="05e56-134">String</span></span>|<span data-ttu-id="05e56-135">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="05e56-135">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="05e56-136">devicesCount</span><span class="sxs-lookup"><span data-stu-id="05e56-136">devicesCount</span></span>|<span data-ttu-id="05e56-137">Int32</span><span class="sxs-lookup"><span data-stu-id="05e56-137">Int32</span></span>|<span data-ttu-id="05e56-138">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="05e56-138">Devices count for that user.</span></span>|
|<span data-ttu-id="05e56-139">status</span><span class="sxs-lookup"><span data-stu-id="05e56-139">status</span></span>|[<span data-ttu-id="05e56-140">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="05e56-140">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="05e56-141">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="05e56-141">Compliance status of the policy report.</span></span> <span data-ttu-id="05e56-142">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="05e56-142">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="05e56-143">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="05e56-143">lastReportedDateTime</span></span>|<span data-ttu-id="05e56-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05e56-144">DateTimeOffset</span></span>|<span data-ttu-id="05e56-145">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="05e56-145">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="05e56-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05e56-146">userPrincipalName</span></span>|<span data-ttu-id="05e56-147">字符串</span><span class="sxs-lookup"><span data-stu-id="05e56-147">String</span></span>|<span data-ttu-id="05e56-148">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="05e56-148">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05e56-149">关系</span><span class="sxs-lookup"><span data-stu-id="05e56-149">Relationships</span></span>
<span data-ttu-id="05e56-150">无</span><span class="sxs-lookup"><span data-stu-id="05e56-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05e56-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05e56-151">JSON Representation</span></span>
<span data-ttu-id="05e56-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05e56-152">Here is a JSON representation of the resource.</span></span>
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







