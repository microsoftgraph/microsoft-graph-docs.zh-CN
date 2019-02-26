---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb1f0764753a576c9e6b1a10112f23257fe339e0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250367"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="77d07-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="77d07-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="77d07-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77d07-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77d07-105">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="77d07-105">Event representing an enrollment failure.</span></span>


<span data-ttu-id="77d07-106">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="77d07-106">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="77d07-107">方法</span><span class="sxs-lookup"><span data-stu-id="77d07-107">Methods</span></span>
|<span data-ttu-id="77d07-108">方法</span><span class="sxs-lookup"><span data-stu-id="77d07-108">Method</span></span>|<span data-ttu-id="77d07-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="77d07-109">Return Type</span></span>|<span data-ttu-id="77d07-110">说明</span><span class="sxs-lookup"><span data-stu-id="77d07-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="77d07-111">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="77d07-111">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="77d07-112">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77d07-112">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="77d07-113">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77d07-113">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="77d07-114">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-114">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="77d07-115">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-115">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="77d07-116">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77d07-116">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="77d07-117">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-117">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="77d07-118">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-118">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="77d07-119">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77d07-119">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="77d07-120">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-120">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="77d07-121">无</span><span class="sxs-lookup"><span data-stu-id="77d07-121">None</span></span>|<span data-ttu-id="77d07-122">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="77d07-122">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="77d07-123">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-123">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="77d07-124">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77d07-124">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="77d07-125">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77d07-125">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="77d07-126">属性</span><span class="sxs-lookup"><span data-stu-id="77d07-126">Properties</span></span>
|<span data-ttu-id="77d07-127">属性</span><span class="sxs-lookup"><span data-stu-id="77d07-127">Property</span></span>|<span data-ttu-id="77d07-128">类型</span><span class="sxs-lookup"><span data-stu-id="77d07-128">Type</span></span>|<span data-ttu-id="77d07-129">说明</span><span class="sxs-lookup"><span data-stu-id="77d07-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77d07-130">id</span><span class="sxs-lookup"><span data-stu-id="77d07-130">id</span></span>|<span data-ttu-id="77d07-131">字符串</span><span class="sxs-lookup"><span data-stu-id="77d07-131">String</span></span>|<span data-ttu-id="77d07-132">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="77d07-132">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="77d07-133">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="77d07-133">eventDateTime</span></span>|<span data-ttu-id="77d07-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77d07-134">DateTimeOffset</span></span>|<span data-ttu-id="77d07-135">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="77d07-135">Time when the event occurred .</span></span> <span data-ttu-id="77d07-136">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="77d07-136">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="77d07-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="77d07-137">correlationId</span></span>|<span data-ttu-id="77d07-138">String</span><span class="sxs-lookup"><span data-stu-id="77d07-138">String</span></span>|<span data-ttu-id="77d07-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="77d07-139">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="77d07-140">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="77d07-140">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="77d07-141">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="77d07-141">managedDeviceIdentifier</span></span>|<span data-ttu-id="77d07-142">String</span><span class="sxs-lookup"><span data-stu-id="77d07-142">String</span></span>|<span data-ttu-id="77d07-143">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="77d07-143">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="77d07-144">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="77d07-144">operatingSystem</span></span>|<span data-ttu-id="77d07-145">String</span><span class="sxs-lookup"><span data-stu-id="77d07-145">String</span></span>|<span data-ttu-id="77d07-146">操作系统。</span><span class="sxs-lookup"><span data-stu-id="77d07-146">Operating System.</span></span>|
|<span data-ttu-id="77d07-147">osVersion</span><span class="sxs-lookup"><span data-stu-id="77d07-147">osVersion</span></span>|<span data-ttu-id="77d07-148">String</span><span class="sxs-lookup"><span data-stu-id="77d07-148">String</span></span>|<span data-ttu-id="77d07-149">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="77d07-149">OS Version.</span></span>|
|<span data-ttu-id="77d07-150">userId</span><span class="sxs-lookup"><span data-stu-id="77d07-150">userId</span></span>|<span data-ttu-id="77d07-151">String</span><span class="sxs-lookup"><span data-stu-id="77d07-151">String</span></span>|<span data-ttu-id="77d07-152">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="77d07-152">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="77d07-153">deviceId</span><span class="sxs-lookup"><span data-stu-id="77d07-153">deviceId</span></span>|<span data-ttu-id="77d07-154">String</span><span class="sxs-lookup"><span data-stu-id="77d07-154">String</span></span>|<span data-ttu-id="77d07-155">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="77d07-155">Azure AD device identifier.</span></span>|
|<span data-ttu-id="77d07-156">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="77d07-156">enrollmentType</span></span>|[<span data-ttu-id="77d07-157">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="77d07-157">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="77d07-158">注册类型。</span><span class="sxs-lookup"><span data-stu-id="77d07-158">Type of the enrollment.</span></span> <span data-ttu-id="77d07-159">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="77d07-159">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="77d07-160">failureCategory</span><span class="sxs-lookup"><span data-stu-id="77d07-160">failureCategory</span></span>|[<span data-ttu-id="77d07-161">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="77d07-161">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="77d07-162">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="77d07-162">Highlevel failure category.</span></span> <span data-ttu-id="77d07-163">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="77d07-163">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="77d07-164">failureReason</span><span class="sxs-lookup"><span data-stu-id="77d07-164">failureReason</span></span>|<span data-ttu-id="77d07-165">String</span><span class="sxs-lookup"><span data-stu-id="77d07-165">String</span></span>|<span data-ttu-id="77d07-166">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="77d07-166">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77d07-167">关系</span><span class="sxs-lookup"><span data-stu-id="77d07-167">Relationships</span></span>
<span data-ttu-id="77d07-168">无</span><span class="sxs-lookup"><span data-stu-id="77d07-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77d07-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77d07-169">JSON Representation</span></span>
<span data-ttu-id="77d07-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77d07-170">Here is a JSON representation of the resource.</span></span>
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



