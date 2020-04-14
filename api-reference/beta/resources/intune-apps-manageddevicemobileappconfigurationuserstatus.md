---
title: managedDeviceMobileAppConfigurationUserStatus 资源类型
description: 包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b51a474a3b3ed2742ebeb531ae8bf5e853fdb34
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458684"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a><span data-ttu-id="a3b40-103">managedDeviceMobileAppConfigurationUserStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3b40-103">managedDeviceMobileAppConfigurationUserStatus resource type</span></span>

<span data-ttu-id="a3b40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3b40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3b40-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3b40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3b40-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3b40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3b40-107">包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="a3b40-107">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="a3b40-108">方法</span><span class="sxs-lookup"><span data-stu-id="a3b40-108">Methods</span></span>
|<span data-ttu-id="a3b40-109">方法</span><span class="sxs-lookup"><span data-stu-id="a3b40-109">Method</span></span>|<span data-ttu-id="a3b40-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3b40-110">Return Type</span></span>|<span data-ttu-id="a3b40-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3b40-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3b40-112">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="a3b40-112">List managedDeviceMobileAppConfigurationUserStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|<span data-ttu-id="a3b40-113">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a3b40-113">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a3b40-114">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3b40-114">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>|
|[<span data-ttu-id="a3b40-115">获取 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-115">Get managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[<span data-ttu-id="a3b40-116">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-116">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="a3b40-117">读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3b40-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="a3b40-118">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-118">Create managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[<span data-ttu-id="a3b40-119">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-119">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="a3b40-120">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3b40-120">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="a3b40-121">删除 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-121">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|<span data-ttu-id="a3b40-122">无</span><span class="sxs-lookup"><span data-stu-id="a3b40-122">None</span></span>|<span data-ttu-id="a3b40-123">删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="a3b40-123">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>|
|[<span data-ttu-id="a3b40-124">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-124">Update managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[<span data-ttu-id="a3b40-125">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-125">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="a3b40-126">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a3b40-126">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3b40-127">属性</span><span class="sxs-lookup"><span data-stu-id="a3b40-127">Properties</span></span>
|<span data-ttu-id="a3b40-128">属性</span><span class="sxs-lookup"><span data-stu-id="a3b40-128">Property</span></span>|<span data-ttu-id="a3b40-129">类型</span><span class="sxs-lookup"><span data-stu-id="a3b40-129">Type</span></span>|<span data-ttu-id="a3b40-130">说明</span><span class="sxs-lookup"><span data-stu-id="a3b40-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b40-131">id</span><span class="sxs-lookup"><span data-stu-id="a3b40-131">id</span></span>|<span data-ttu-id="a3b40-132">String</span><span class="sxs-lookup"><span data-stu-id="a3b40-132">String</span></span>|<span data-ttu-id="a3b40-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a3b40-133">Key of the entity.</span></span>|
|<span data-ttu-id="a3b40-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3b40-134">userDisplayName</span></span>|<span data-ttu-id="a3b40-135">String</span><span class="sxs-lookup"><span data-stu-id="a3b40-135">String</span></span>|<span data-ttu-id="a3b40-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="a3b40-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a3b40-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="a3b40-137">devicesCount</span></span>|<span data-ttu-id="a3b40-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a3b40-138">Int32</span></span>|<span data-ttu-id="a3b40-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="a3b40-139">Devices count for that user.</span></span>|
|<span data-ttu-id="a3b40-140">status</span><span class="sxs-lookup"><span data-stu-id="a3b40-140">status</span></span>|[<span data-ttu-id="a3b40-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a3b40-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a3b40-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="a3b40-142">Compliance status of the policy report.</span></span> <span data-ttu-id="a3b40-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a3b40-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a3b40-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3b40-144">lastReportedDateTime</span></span>|<span data-ttu-id="a3b40-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3b40-145">DateTimeOffset</span></span>|<span data-ttu-id="a3b40-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="a3b40-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a3b40-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3b40-147">userPrincipalName</span></span>|<span data-ttu-id="a3b40-148">字符串</span><span class="sxs-lookup"><span data-stu-id="a3b40-148">String</span></span>|<span data-ttu-id="a3b40-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="a3b40-149">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3b40-150">关系</span><span class="sxs-lookup"><span data-stu-id="a3b40-150">Relationships</span></span>
<span data-ttu-id="a3b40-151">无</span><span class="sxs-lookup"><span data-stu-id="a3b40-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3b40-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3b40-152">JSON Representation</span></span>
<span data-ttu-id="a3b40-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3b40-153">Here is a JSON representation of the resource.</span></span>
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



