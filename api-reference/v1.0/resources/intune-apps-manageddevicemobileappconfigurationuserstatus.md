---
title: managedDeviceMobileAppConfigurationUserStatus 资源类型
description: 包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 96dff33ed62c968880959e281c92d752669ce1b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029020"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a><span data-ttu-id="ceabc-103">managedDeviceMobileAppConfigurationUserStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ceabc-103">managedDeviceMobileAppConfigurationUserStatus resource type</span></span>

> <span data-ttu-id="ceabc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ceabc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceabc-105">包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="ceabc-105">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="ceabc-106">方法</span><span class="sxs-lookup"><span data-stu-id="ceabc-106">Methods</span></span>
|<span data-ttu-id="ceabc-107">方法</span><span class="sxs-lookup"><span data-stu-id="ceabc-107">Method</span></span>|<span data-ttu-id="ceabc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ceabc-108">Return Type</span></span>|<span data-ttu-id="ceabc-109">说明</span><span class="sxs-lookup"><span data-stu-id="ceabc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ceabc-110">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="ceabc-110">List managedDeviceMobileAppConfigurationUserStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|<span data-ttu-id="ceabc-111">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ceabc-111">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ceabc-112">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ceabc-112">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>|
|[<span data-ttu-id="ceabc-113">获取 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-113">Get managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[<span data-ttu-id="ceabc-114">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-114">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="ceabc-115">读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ceabc-115">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="ceabc-116">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-116">Create managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[<span data-ttu-id="ceabc-117">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-117">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="ceabc-118">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceabc-118">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="ceabc-119">删除 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-119">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|<span data-ttu-id="ceabc-120">无</span><span class="sxs-lookup"><span data-stu-id="ceabc-120">None</span></span>|<span data-ttu-id="ceabc-121">删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="ceabc-121">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>|
|[<span data-ttu-id="ceabc-122">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-122">Update managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[<span data-ttu-id="ceabc-123">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-123">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="ceabc-124">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ceabc-124">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ceabc-125">属性</span><span class="sxs-lookup"><span data-stu-id="ceabc-125">Properties</span></span>
|<span data-ttu-id="ceabc-126">属性</span><span class="sxs-lookup"><span data-stu-id="ceabc-126">Property</span></span>|<span data-ttu-id="ceabc-127">类型</span><span class="sxs-lookup"><span data-stu-id="ceabc-127">Type</span></span>|<span data-ttu-id="ceabc-128">说明</span><span class="sxs-lookup"><span data-stu-id="ceabc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceabc-129">id</span><span class="sxs-lookup"><span data-stu-id="ceabc-129">id</span></span>|<span data-ttu-id="ceabc-130">String</span><span class="sxs-lookup"><span data-stu-id="ceabc-130">String</span></span>|<span data-ttu-id="ceabc-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ceabc-131">Key of the entity.</span></span>|
|<span data-ttu-id="ceabc-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ceabc-132">userDisplayName</span></span>|<span data-ttu-id="ceabc-133">String</span><span class="sxs-lookup"><span data-stu-id="ceabc-133">String</span></span>|<span data-ttu-id="ceabc-134">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="ceabc-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ceabc-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ceabc-135">devicesCount</span></span>|<span data-ttu-id="ceabc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ceabc-136">Int32</span></span>|<span data-ttu-id="ceabc-137">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="ceabc-137">Devices count for that user.</span></span>|
|<span data-ttu-id="ceabc-138">status</span><span class="sxs-lookup"><span data-stu-id="ceabc-138">status</span></span>|[<span data-ttu-id="ceabc-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ceabc-139">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ceabc-140">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="ceabc-140">Compliance status of the policy report.</span></span> <span data-ttu-id="ceabc-141">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ceabc-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ceabc-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceabc-142">lastReportedDateTime</span></span>|<span data-ttu-id="ceabc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceabc-143">DateTimeOffset</span></span>|<span data-ttu-id="ceabc-144">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ceabc-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ceabc-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ceabc-145">userPrincipalName</span></span>|<span data-ttu-id="ceabc-146">字符串</span><span class="sxs-lookup"><span data-stu-id="ceabc-146">String</span></span>|<span data-ttu-id="ceabc-147">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ceabc-147">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceabc-148">关系</span><span class="sxs-lookup"><span data-stu-id="ceabc-148">Relationships</span></span>
<span data-ttu-id="ceabc-149">无</span><span class="sxs-lookup"><span data-stu-id="ceabc-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceabc-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ceabc-150">JSON Representation</span></span>
<span data-ttu-id="ceabc-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceabc-151">Here is a JSON representation of the resource.</span></span>
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



