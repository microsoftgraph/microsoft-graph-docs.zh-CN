---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 513f65198e234d78ffe91bf00736796dff14707b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847017"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="b5ea8-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5ea8-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="b5ea8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5ea8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5ea8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5ea8-107">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-107">Event representing an enrollment failure.</span></span>

<span data-ttu-id="b5ea8-108">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b5ea8-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b5ea8-109">方法</span><span class="sxs-lookup"><span data-stu-id="b5ea8-109">Methods</span></span>
|<span data-ttu-id="b5ea8-110">方法</span><span class="sxs-lookup"><span data-stu-id="b5ea8-110">Method</span></span>|<span data-ttu-id="b5ea8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5ea8-111">Return Type</span></span>|<span data-ttu-id="b5ea8-112">说明</span><span class="sxs-lookup"><span data-stu-id="b5ea8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5ea8-113">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="b5ea8-113">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="b5ea8-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b5ea8-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="b5ea8-115">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-115">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="b5ea8-116">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-116">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="b5ea8-117">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-117">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="b5ea8-118">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-118">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="b5ea8-119">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-119">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="b5ea8-120">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-120">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="b5ea8-121">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-121">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="b5ea8-122">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-122">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="b5ea8-123">无</span><span class="sxs-lookup"><span data-stu-id="b5ea8-123">None</span></span>|<span data-ttu-id="b5ea8-124">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-124">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="b5ea8-125">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-125">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="b5ea8-126">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b5ea8-126">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="b5ea8-127">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-127">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5ea8-128">属性</span><span class="sxs-lookup"><span data-stu-id="b5ea8-128">Properties</span></span>
|<span data-ttu-id="b5ea8-129">属性</span><span class="sxs-lookup"><span data-stu-id="b5ea8-129">Property</span></span>|<span data-ttu-id="b5ea8-130">类型</span><span class="sxs-lookup"><span data-stu-id="b5ea8-130">Type</span></span>|<span data-ttu-id="b5ea8-131">说明</span><span class="sxs-lookup"><span data-stu-id="b5ea8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ea8-132">id</span><span class="sxs-lookup"><span data-stu-id="b5ea8-132">id</span></span>|<span data-ttu-id="b5ea8-133">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-133">String</span></span>|<span data-ttu-id="b5ea8-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b5ea8-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b5ea8-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b5ea8-135">eventDateTime</span></span>|<span data-ttu-id="b5ea8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5ea8-136">DateTimeOffset</span></span>|<span data-ttu-id="b5ea8-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-137">Time when the event occurred .</span></span> <span data-ttu-id="b5ea8-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b5ea8-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b5ea8-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="b5ea8-139">correlationId</span></span>|<span data-ttu-id="b5ea8-140">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-140">String</span></span>|<span data-ttu-id="b5ea8-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="b5ea8-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="b5ea8-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b5ea8-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5ea8-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="b5ea8-144">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-144">String</span></span>|<span data-ttu-id="b5ea8-145">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b5ea8-146">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b5ea8-146">operatingSystem</span></span>|<span data-ttu-id="b5ea8-147">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-147">String</span></span>|<span data-ttu-id="b5ea8-148">操作系统。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-148">Operating System.</span></span>|
|<span data-ttu-id="b5ea8-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="b5ea8-149">osVersion</span></span>|<span data-ttu-id="b5ea8-150">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-150">String</span></span>|<span data-ttu-id="b5ea8-151">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-151">OS Version.</span></span>|
|<span data-ttu-id="b5ea8-152">userId</span><span class="sxs-lookup"><span data-stu-id="b5ea8-152">userId</span></span>|<span data-ttu-id="b5ea8-153">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-153">String</span></span>|<span data-ttu-id="b5ea8-154">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-154">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="b5ea8-155">deviceId</span><span class="sxs-lookup"><span data-stu-id="b5ea8-155">deviceId</span></span>|<span data-ttu-id="b5ea8-156">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-156">String</span></span>|<span data-ttu-id="b5ea8-157">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-157">Azure AD device identifier.</span></span>|
|<span data-ttu-id="b5ea8-158">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b5ea8-158">enrollmentType</span></span>|[<span data-ttu-id="b5ea8-159">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b5ea8-159">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b5ea8-160">注册类型。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-160">Type of the enrollment.</span></span> <span data-ttu-id="b5ea8-161">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-161">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b5ea8-162">failureCategory</span><span class="sxs-lookup"><span data-stu-id="b5ea8-162">failureCategory</span></span>|[<span data-ttu-id="b5ea8-163">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="b5ea8-163">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="b5ea8-164">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-164">Highlevel failure category.</span></span> <span data-ttu-id="b5ea8-165">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-165">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="b5ea8-166">failureReason</span><span class="sxs-lookup"><span data-stu-id="b5ea8-166">failureReason</span></span>|<span data-ttu-id="b5ea8-167">String</span><span class="sxs-lookup"><span data-stu-id="b5ea8-167">String</span></span>|<span data-ttu-id="b5ea8-168">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-168">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5ea8-169">关系</span><span class="sxs-lookup"><span data-stu-id="b5ea8-169">Relationships</span></span>
<span data-ttu-id="b5ea8-170">无</span><span class="sxs-lookup"><span data-stu-id="b5ea8-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5ea8-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5ea8-171">JSON Representation</span></span>
<span data-ttu-id="b5ea8-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5ea8-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```





