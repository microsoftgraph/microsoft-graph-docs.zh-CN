---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: tfitzmac
ms.openlocfilehash: fd4320ecb62d4f9441f4e507ac451565d418a015
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309805"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="9ac2a-103">enrollmentTroubleshootingEvent 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ac2a-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="9ac2a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ac2a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ac2a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ac2a-107">表示注册失败的事件。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-107">Event representing an enrollment failure.</span></span>

<span data-ttu-id="9ac2a-108">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9ac2a-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9ac2a-109">方法</span><span class="sxs-lookup"><span data-stu-id="9ac2a-109">Methods</span></span>
|<span data-ttu-id="9ac2a-110">方法</span><span class="sxs-lookup"><span data-stu-id="9ac2a-110">Method</span></span>|<span data-ttu-id="9ac2a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ac2a-111">Return Type</span></span>|<span data-ttu-id="9ac2a-112">说明</span><span class="sxs-lookup"><span data-stu-id="9ac2a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ac2a-113">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="9ac2a-113">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="9ac2a-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ac2a-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="9ac2a-115">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-115">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="9ac2a-116">获取 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-116">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="9ac2a-117">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-117">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="9ac2a-118">读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-118">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="9ac2a-119">创建 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-119">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="9ac2a-120">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-120">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="9ac2a-121">创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-121">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="9ac2a-122">删除 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-122">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="9ac2a-123">无</span><span class="sxs-lookup"><span data-stu-id="9ac2a-123">None</span></span>|<span data-ttu-id="9ac2a-124">删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-124">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="9ac2a-125">更新 enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-125">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="9ac2a-126">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9ac2a-126">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="9ac2a-127">更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-127">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ac2a-128">属性</span><span class="sxs-lookup"><span data-stu-id="9ac2a-128">Properties</span></span>
|<span data-ttu-id="9ac2a-129">属性</span><span class="sxs-lookup"><span data-stu-id="9ac2a-129">Property</span></span>|<span data-ttu-id="9ac2a-130">类型</span><span class="sxs-lookup"><span data-stu-id="9ac2a-130">Type</span></span>|<span data-ttu-id="9ac2a-131">说明</span><span class="sxs-lookup"><span data-stu-id="9ac2a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac2a-132">id</span><span class="sxs-lookup"><span data-stu-id="9ac2a-132">id</span></span>|<span data-ttu-id="9ac2a-133">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-133">String</span></span>|<span data-ttu-id="9ac2a-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9ac2a-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9ac2a-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac2a-135">eventDateTime</span></span>|<span data-ttu-id="9ac2a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac2a-136">DateTimeOffset</span></span>|<span data-ttu-id="9ac2a-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-137">Time when the event occurred .</span></span> <span data-ttu-id="9ac2a-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9ac2a-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9ac2a-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="9ac2a-139">correlationId</span></span>|<span data-ttu-id="9ac2a-140">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-140">String</span></span>|<span data-ttu-id="9ac2a-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="9ac2a-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="9ac2a-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9ac2a-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ac2a-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="9ac2a-144">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-144">String</span></span>|<span data-ttu-id="9ac2a-145">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="9ac2a-146">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ac2a-146">operatingSystem</span></span>|<span data-ttu-id="9ac2a-147">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-147">String</span></span>|<span data-ttu-id="9ac2a-148">操作系统。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-148">Operating System.</span></span>|
|<span data-ttu-id="9ac2a-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="9ac2a-149">osVersion</span></span>|<span data-ttu-id="9ac2a-150">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-150">String</span></span>|<span data-ttu-id="9ac2a-151">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-151">OS Version.</span></span>|
|<span data-ttu-id="9ac2a-152">userId</span><span class="sxs-lookup"><span data-stu-id="9ac2a-152">userId</span></span>|<span data-ttu-id="9ac2a-153">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-153">String</span></span>|<span data-ttu-id="9ac2a-154">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-154">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="9ac2a-155">deviceId</span><span class="sxs-lookup"><span data-stu-id="9ac2a-155">deviceId</span></span>|<span data-ttu-id="9ac2a-156">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-156">String</span></span>|<span data-ttu-id="9ac2a-157">Azure AD 设备标识符。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-157">Azure AD device identifier.</span></span>|
|<span data-ttu-id="9ac2a-158">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="9ac2a-158">enrollmentType</span></span>|[<span data-ttu-id="9ac2a-159">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9ac2a-159">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="9ac2a-160">注册类型。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-160">Type of the enrollment.</span></span> <span data-ttu-id="9ac2a-161">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-161">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="9ac2a-162">failureCategory</span><span class="sxs-lookup"><span data-stu-id="9ac2a-162">failureCategory</span></span>|[<span data-ttu-id="9ac2a-163">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="9ac2a-163">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="9ac2a-164">Highlevel 失败类别。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-164">Highlevel failure category.</span></span> <span data-ttu-id="9ac2a-165">可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-165">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="9ac2a-166">failureReason</span><span class="sxs-lookup"><span data-stu-id="9ac2a-166">failureReason</span></span>|<span data-ttu-id="9ac2a-167">String</span><span class="sxs-lookup"><span data-stu-id="9ac2a-167">String</span></span>|<span data-ttu-id="9ac2a-168">详细失败原因。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-168">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac2a-169">关系</span><span class="sxs-lookup"><span data-stu-id="9ac2a-169">Relationships</span></span>
<span data-ttu-id="9ac2a-170">无</span><span class="sxs-lookup"><span data-stu-id="9ac2a-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ac2a-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ac2a-171">JSON Representation</span></span>
<span data-ttu-id="9ac2a-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ac2a-172">Here is a JSON representation of the resource.</span></span>
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





