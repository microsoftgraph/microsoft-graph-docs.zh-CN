---
title: managedDeviceMobileAppConfigurationUserStatus 资源类型
description: 包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。
localization_priority: Normal
ms.openlocfilehash: 719f784b2b135d58950892c185614a1247b5d25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846751"
---
# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a><span data-ttu-id="ae68f-103">managedDeviceMobileAppConfigurationUserStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae68f-103">managedDeviceMobileAppConfigurationUserStatus resource type</span></span>

> <span data-ttu-id="ae68f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae68f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae68f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae68f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae68f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ae68f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae68f-107">包含某个用户的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="ae68f-107">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="ae68f-108">方法</span><span class="sxs-lookup"><span data-stu-id="ae68f-108">Methods</span></span>
|<span data-ttu-id="ae68f-109">方法</span><span class="sxs-lookup"><span data-stu-id="ae68f-109">Method</span></span>|<span data-ttu-id="ae68f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ae68f-110">Return Type</span></span>|<span data-ttu-id="ae68f-111">说明</span><span class="sxs-lookup"><span data-stu-id="ae68f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae68f-112">列出 managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="ae68f-112">List managedDeviceMobileAppConfigurationUserStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-list.md)|<span data-ttu-id="ae68f-113">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ae68f-113">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ae68f-114">列出 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae68f-114">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>|
|[<span data-ttu-id="ae68f-115">获取 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-115">Get managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-get.md)|[<span data-ttu-id="ae68f-116">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-116">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="ae68f-117">读取 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae68f-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="ae68f-118">创建 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-118">Create managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-create.md)|[<span data-ttu-id="ae68f-119">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-119">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="ae68f-120">创建新的 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae68f-120">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|
|[<span data-ttu-id="ae68f-121">删除 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-121">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-delete.md)|<span data-ttu-id="ae68f-122">无</span><span class="sxs-lookup"><span data-stu-id="ae68f-122">None</span></span>|<span data-ttu-id="ae68f-123">删除 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="ae68f-123">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>|
|[<span data-ttu-id="ae68f-124">更新 managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-124">Update managedDeviceMobileAppConfigurationUserStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationuserstatus-update.md)|[<span data-ttu-id="ae68f-125">managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-125">managedDeviceMobileAppConfigurationUserStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|<span data-ttu-id="ae68f-126">更新 [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ae68f-126">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae68f-127">属性</span><span class="sxs-lookup"><span data-stu-id="ae68f-127">Properties</span></span>
|<span data-ttu-id="ae68f-128">属性</span><span class="sxs-lookup"><span data-stu-id="ae68f-128">Property</span></span>|<span data-ttu-id="ae68f-129">类型</span><span class="sxs-lookup"><span data-stu-id="ae68f-129">Type</span></span>|<span data-ttu-id="ae68f-130">说明</span><span class="sxs-lookup"><span data-stu-id="ae68f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae68f-131">id</span><span class="sxs-lookup"><span data-stu-id="ae68f-131">id</span></span>|<span data-ttu-id="ae68f-132">String</span><span class="sxs-lookup"><span data-stu-id="ae68f-132">String</span></span>|<span data-ttu-id="ae68f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ae68f-133">Key of the entity.</span></span>|
|<span data-ttu-id="ae68f-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ae68f-134">userDisplayName</span></span>|<span data-ttu-id="ae68f-135">String</span><span class="sxs-lookup"><span data-stu-id="ae68f-135">String</span></span>|<span data-ttu-id="ae68f-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="ae68f-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ae68f-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ae68f-137">devicesCount</span></span>|<span data-ttu-id="ae68f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ae68f-138">Int32</span></span>|<span data-ttu-id="ae68f-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="ae68f-139">Devices count for that user.</span></span>|
|<span data-ttu-id="ae68f-140">status</span><span class="sxs-lookup"><span data-stu-id="ae68f-140">status</span></span>|[<span data-ttu-id="ae68f-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ae68f-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ae68f-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="ae68f-142">Compliance status of the policy report.</span></span> <span data-ttu-id="ae68f-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ae68f-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ae68f-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae68f-144">lastReportedDateTime</span></span>|<span data-ttu-id="ae68f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae68f-145">DateTimeOffset</span></span>|<span data-ttu-id="ae68f-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ae68f-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ae68f-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae68f-147">userPrincipalName</span></span>|<span data-ttu-id="ae68f-148">String</span><span class="sxs-lookup"><span data-stu-id="ae68f-148">String</span></span>|<span data-ttu-id="ae68f-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ae68f-149">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae68f-150">关系</span><span class="sxs-lookup"><span data-stu-id="ae68f-150">Relationships</span></span>
<span data-ttu-id="ae68f-151">无</span><span class="sxs-lookup"><span data-stu-id="ae68f-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae68f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae68f-152">JSON Representation</span></span>
<span data-ttu-id="ae68f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae68f-153">Here is a JSON representation of the resource.</span></span>
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





