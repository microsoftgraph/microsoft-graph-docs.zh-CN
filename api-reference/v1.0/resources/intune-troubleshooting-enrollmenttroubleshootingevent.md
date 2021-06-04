---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec13319b1f95677cd537b95ce04a69db0e579f68
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732398"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="29aaf-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="29aaf-103">enrollmentTroubleshootingEvent resource type</span></span>

<span data-ttu-id="29aaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29aaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29aaf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29aaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29aaf-106">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="29aaf-106">Event representing an enrollment failure.</span></span>


<span data-ttu-id="29aaf-107">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29aaf-107">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="29aaf-108">Methods</span><span class="sxs-lookup"><span data-stu-id="29aaf-108">Methods</span></span>
|<span data-ttu-id="29aaf-109">方法</span><span class="sxs-lookup"><span data-stu-id="29aaf-109">Method</span></span>|<span data-ttu-id="29aaf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="29aaf-110">Return Type</span></span>|<span data-ttu-id="29aaf-111">Description</span><span class="sxs-lookup"><span data-stu-id="29aaf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29aaf-112">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="29aaf-112">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="29aaf-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29aaf-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="29aaf-114">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29aaf-114">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="29aaf-115">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-115">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="29aaf-116">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-116">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="29aaf-117">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29aaf-117">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="29aaf-118">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-118">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="29aaf-119">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-119">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="29aaf-120">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29aaf-120">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="29aaf-121">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-121">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="29aaf-122">无</span><span class="sxs-lookup"><span data-stu-id="29aaf-122">None</span></span>|<span data-ttu-id="29aaf-123">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="29aaf-123">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="29aaf-124">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-124">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="29aaf-125">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29aaf-125">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="29aaf-126">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="29aaf-126">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29aaf-127">属性</span><span class="sxs-lookup"><span data-stu-id="29aaf-127">Properties</span></span>
|<span data-ttu-id="29aaf-128">属性</span><span class="sxs-lookup"><span data-stu-id="29aaf-128">Property</span></span>|<span data-ttu-id="29aaf-129">类型</span><span class="sxs-lookup"><span data-stu-id="29aaf-129">Type</span></span>|<span data-ttu-id="29aaf-130">说明</span><span class="sxs-lookup"><span data-stu-id="29aaf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29aaf-131">id</span><span class="sxs-lookup"><span data-stu-id="29aaf-131">id</span></span>|<span data-ttu-id="29aaf-132">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-132">String</span></span>|<span data-ttu-id="29aaf-133">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29aaf-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29aaf-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="29aaf-134">eventDateTime</span></span>|<span data-ttu-id="29aaf-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29aaf-135">DateTimeOffset</span></span>|<span data-ttu-id="29aaf-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="29aaf-136">Time when the event occurred .</span></span> <span data-ttu-id="29aaf-137">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29aaf-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29aaf-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="29aaf-138">correlationId</span></span>|<span data-ttu-id="29aaf-139">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-139">String</span></span>|<span data-ttu-id="29aaf-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="29aaf-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="29aaf-141">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="29aaf-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29aaf-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="29aaf-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="29aaf-143">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-143">String</span></span>|<span data-ttu-id="29aaf-144">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="29aaf-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="29aaf-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="29aaf-145">operatingSystem</span></span>|<span data-ttu-id="29aaf-146">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-146">String</span></span>|<span data-ttu-id="29aaf-147">操作系统。</span><span class="sxs-lookup"><span data-stu-id="29aaf-147">Operating System.</span></span>|
|<span data-ttu-id="29aaf-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="29aaf-148">osVersion</span></span>|<span data-ttu-id="29aaf-149">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-149">String</span></span>|<span data-ttu-id="29aaf-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="29aaf-150">OS Version.</span></span>|
|<span data-ttu-id="29aaf-151">userId</span><span class="sxs-lookup"><span data-stu-id="29aaf-151">userId</span></span>|<span data-ttu-id="29aaf-152">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-152">String</span></span>|<span data-ttu-id="29aaf-153">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="29aaf-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="29aaf-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="29aaf-154">deviceId</span></span>|<span data-ttu-id="29aaf-155">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-155">String</span></span>|<span data-ttu-id="29aaf-156">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="29aaf-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="29aaf-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="29aaf-157">enrollmentType</span></span>|[<span data-ttu-id="29aaf-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="29aaf-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="29aaf-159">注册类型。</span><span class="sxs-lookup"><span data-stu-id="29aaf-159">Type of the enrollment.</span></span> <span data-ttu-id="29aaf-160">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="29aaf-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="29aaf-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="29aaf-161">failureCategory</span></span>|[<span data-ttu-id="29aaf-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="29aaf-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="29aaf-163">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="29aaf-163">Highlevel failure category.</span></span> <span data-ttu-id="29aaf-164">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="29aaf-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="29aaf-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="29aaf-165">failureReason</span></span>|<span data-ttu-id="29aaf-166">String</span><span class="sxs-lookup"><span data-stu-id="29aaf-166">String</span></span>|<span data-ttu-id="29aaf-167">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="29aaf-167">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29aaf-168">关系</span><span class="sxs-lookup"><span data-stu-id="29aaf-168">Relationships</span></span>
<span data-ttu-id="29aaf-169">无</span><span class="sxs-lookup"><span data-stu-id="29aaf-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29aaf-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29aaf-170">JSON Representation</span></span>
<span data-ttu-id="29aaf-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29aaf-171">Here is a JSON representation of the resource.</span></span>
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









