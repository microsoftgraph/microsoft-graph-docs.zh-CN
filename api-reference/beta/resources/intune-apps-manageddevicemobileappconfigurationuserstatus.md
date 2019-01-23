---
title: managedDeviceMobileAppConfigurationUserStatus 资源类型
description: 包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68424e75859e938c1cedb8c14ba8f70141dc6899
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419455"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a><span data-ttu-id="4343d-103">managedDeviceMobileAppConfigurationUserStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="4343d-103">managedDeviceMobileAppConfigurationUserStatus resource type</span></span>

> <span data-ttu-id="4343d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4343d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4343d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4343d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4343d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4343d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4343d-107">包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="4343d-107">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="4343d-108">方法</span><span class="sxs-lookup"><span data-stu-id="4343d-108">Methods</span></span>
|<span data-ttu-id="4343d-109">方法</span><span class="sxs-lookup"><span data-stu-id="4343d-109">Method</span></span>|<span data-ttu-id="4343d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4343d-110">Return Type</span></span>|<span data-ttu-id="4343d-111">说明</span><span class="sxs-lookup"><span data-stu-id="4343d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4343d-112">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="4343d-112">List managedDeviceMobileAppConfigurationUserStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|<span data-ttu-id="4343d-113">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4343d-113">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="4343d-114">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4343d-114">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>|
|[<span data-ttu-id="4343d-115">获取 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-115">Get managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[<span data-ttu-id="4343d-116">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-116">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="4343d-117">读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4343d-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="4343d-118">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-118">Create managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[<span data-ttu-id="4343d-119">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-119">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="4343d-120">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4343d-120">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="4343d-121">删除 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-121">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|<span data-ttu-id="4343d-122">无</span><span class="sxs-lookup"><span data-stu-id="4343d-122">None</span></span>|<span data-ttu-id="4343d-123">删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="4343d-123">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>|
|[<span data-ttu-id="4343d-124">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-124">Update managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[<span data-ttu-id="4343d-125">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-125">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="4343d-126">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4343d-126">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4343d-127">属性</span><span class="sxs-lookup"><span data-stu-id="4343d-127">Properties</span></span>
|<span data-ttu-id="4343d-128">属性</span><span class="sxs-lookup"><span data-stu-id="4343d-128">Property</span></span>|<span data-ttu-id="4343d-129">类型</span><span class="sxs-lookup"><span data-stu-id="4343d-129">Type</span></span>|<span data-ttu-id="4343d-130">说明</span><span class="sxs-lookup"><span data-stu-id="4343d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4343d-131">id</span><span class="sxs-lookup"><span data-stu-id="4343d-131">id</span></span>|<span data-ttu-id="4343d-132">String</span><span class="sxs-lookup"><span data-stu-id="4343d-132">String</span></span>|<span data-ttu-id="4343d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4343d-133">Key of the entity.</span></span>|
|<span data-ttu-id="4343d-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4343d-134">userDisplayName</span></span>|<span data-ttu-id="4343d-135">String</span><span class="sxs-lookup"><span data-stu-id="4343d-135">String</span></span>|<span data-ttu-id="4343d-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="4343d-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4343d-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="4343d-137">devicesCount</span></span>|<span data-ttu-id="4343d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4343d-138">Int32</span></span>|<span data-ttu-id="4343d-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="4343d-139">Devices count for that user.</span></span>|
|<span data-ttu-id="4343d-140">status</span><span class="sxs-lookup"><span data-stu-id="4343d-140">status</span></span>|[<span data-ttu-id="4343d-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4343d-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4343d-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="4343d-142">Compliance status of the policy report.</span></span> <span data-ttu-id="4343d-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4343d-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4343d-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4343d-144">lastReportedDateTime</span></span>|<span data-ttu-id="4343d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4343d-145">DateTimeOffset</span></span>|<span data-ttu-id="4343d-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="4343d-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4343d-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4343d-147">userPrincipalName</span></span>|<span data-ttu-id="4343d-148">String</span><span class="sxs-lookup"><span data-stu-id="4343d-148">String</span></span>|<span data-ttu-id="4343d-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4343d-149">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4343d-150">关系</span><span class="sxs-lookup"><span data-stu-id="4343d-150">Relationships</span></span>
<span data-ttu-id="4343d-151">无</span><span class="sxs-lookup"><span data-stu-id="4343d-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4343d-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4343d-152">JSON Representation</span></span>
<span data-ttu-id="4343d-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4343d-153">Here is a JSON representation of the resource.</span></span>
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




