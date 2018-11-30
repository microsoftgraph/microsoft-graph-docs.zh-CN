---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
ms.openlocfilehash: f44fa444cf57c0b864162d370b1e9ee1b6fa41e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011617"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="a7e06-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7e06-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="a7e06-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7e06-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7e06-105">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="a7e06-105">Event representing an enrollment failure.</span></span>

<span data-ttu-id="a7e06-106">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a7e06-106">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a7e06-107">方法</span><span class="sxs-lookup"><span data-stu-id="a7e06-107">Methods</span></span>
|<span data-ttu-id="a7e06-108">方法</span><span class="sxs-lookup"><span data-stu-id="a7e06-108">Method</span></span>|<span data-ttu-id="a7e06-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7e06-109">Return Type</span></span>|<span data-ttu-id="a7e06-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7e06-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7e06-111">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="a7e06-111">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="a7e06-112">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7e06-112">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="a7e06-113">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7e06-113">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="a7e06-114">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-114">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="a7e06-115">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-115">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="a7e06-116">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7e06-116">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="a7e06-117">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-117">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="a7e06-118">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-118">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="a7e06-119">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7e06-119">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="a7e06-120">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-120">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="a7e06-121">无</span><span class="sxs-lookup"><span data-stu-id="a7e06-121">None</span></span>|<span data-ttu-id="a7e06-122">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="a7e06-122">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="a7e06-123">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-123">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="a7e06-124">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a7e06-124">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="a7e06-125">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7e06-125">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7e06-126">属性</span><span class="sxs-lookup"><span data-stu-id="a7e06-126">Properties</span></span>
|<span data-ttu-id="a7e06-127">属性</span><span class="sxs-lookup"><span data-stu-id="a7e06-127">Property</span></span>|<span data-ttu-id="a7e06-128">类型</span><span class="sxs-lookup"><span data-stu-id="a7e06-128">Type</span></span>|<span data-ttu-id="a7e06-129">说明</span><span class="sxs-lookup"><span data-stu-id="a7e06-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e06-130">id</span><span class="sxs-lookup"><span data-stu-id="a7e06-130">id</span></span>|<span data-ttu-id="a7e06-131">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-131">String</span></span>|<span data-ttu-id="a7e06-132">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a7e06-132">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a7e06-133">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a7e06-133">eventDateTime</span></span>|<span data-ttu-id="a7e06-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7e06-134">DateTimeOffset</span></span>|<span data-ttu-id="a7e06-135">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="a7e06-135">Time when the event occurred .</span></span> <span data-ttu-id="a7e06-136">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a7e06-136">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a7e06-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="a7e06-137">correlationId</span></span>|<span data-ttu-id="a7e06-138">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-138">String</span></span>|<span data-ttu-id="a7e06-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="a7e06-139">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="a7e06-140">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a7e06-140">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a7e06-141">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a7e06-141">managedDeviceIdentifier</span></span>|<span data-ttu-id="a7e06-142">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-142">String</span></span>|<span data-ttu-id="a7e06-143">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="a7e06-143">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="a7e06-144">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a7e06-144">operatingSystem</span></span>|<span data-ttu-id="a7e06-145">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-145">String</span></span>|<span data-ttu-id="a7e06-146">操作系统。</span><span class="sxs-lookup"><span data-stu-id="a7e06-146">Operating System.</span></span>|
|<span data-ttu-id="a7e06-147">osVersion</span><span class="sxs-lookup"><span data-stu-id="a7e06-147">osVersion</span></span>|<span data-ttu-id="a7e06-148">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-148">String</span></span>|<span data-ttu-id="a7e06-149">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a7e06-149">OS Version.</span></span>|
|<span data-ttu-id="a7e06-150">userId</span><span class="sxs-lookup"><span data-stu-id="a7e06-150">userId</span></span>|<span data-ttu-id="a7e06-151">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-151">String</span></span>|<span data-ttu-id="a7e06-152">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="a7e06-152">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="a7e06-153">deviceId</span><span class="sxs-lookup"><span data-stu-id="a7e06-153">deviceId</span></span>|<span data-ttu-id="a7e06-154">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-154">String</span></span>|<span data-ttu-id="a7e06-155">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="a7e06-155">Azure AD device identifier.</span></span>|
|<span data-ttu-id="a7e06-156">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="a7e06-156">enrollmentType</span></span>|[<span data-ttu-id="a7e06-157">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a7e06-157">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="a7e06-158">注册类型。</span><span class="sxs-lookup"><span data-stu-id="a7e06-158">Type of the enrollment.</span></span> <span data-ttu-id="a7e06-159">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="a7e06-159">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="a7e06-160">failureCategory</span><span class="sxs-lookup"><span data-stu-id="a7e06-160">failureCategory</span></span>|[<span data-ttu-id="a7e06-161">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="a7e06-161">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="a7e06-162">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="a7e06-162">Highlevel failure category.</span></span> <span data-ttu-id="a7e06-163">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="a7e06-163">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="a7e06-164">failureReason</span><span class="sxs-lookup"><span data-stu-id="a7e06-164">failureReason</span></span>|<span data-ttu-id="a7e06-165">String</span><span class="sxs-lookup"><span data-stu-id="a7e06-165">String</span></span>|<span data-ttu-id="a7e06-166">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="a7e06-166">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7e06-167">关系</span><span class="sxs-lookup"><span data-stu-id="a7e06-167">Relationships</span></span>
<span data-ttu-id="a7e06-168">无</span><span class="sxs-lookup"><span data-stu-id="a7e06-168">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7e06-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7e06-169">JSON Representation</span></span>
<span data-ttu-id="a7e06-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7e06-170">Here is a JSON representation of the resource.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->



