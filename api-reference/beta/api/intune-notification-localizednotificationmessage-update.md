---
title: 更新 localizedNotificationMessage
description: 更新 localizedNotificationMessage 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1827b0d61462c4dbf05bbaed39ba00cfa3a57dc5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989946"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="fa279-103">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="fa279-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="fa279-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa279-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa279-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa279-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa279-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa279-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa279-107">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa279-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa279-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa279-108">Prerequisites</span></span>
<span data-ttu-id="fa279-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa279-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa279-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa279-111">Permission type</span></span>|<span data-ttu-id="fa279-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa279-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa279-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa279-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa279-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa279-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa279-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa279-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa279-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa279-116">Not supported.</span></span>|
|<span data-ttu-id="fa279-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa279-117">Application</span></span>|<span data-ttu-id="fa279-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa279-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa279-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa279-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="fa279-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa279-120">Request headers</span></span>
|<span data-ttu-id="fa279-121">标头</span><span class="sxs-lookup"><span data-stu-id="fa279-121">Header</span></span>|<span data-ttu-id="fa279-122">值</span><span class="sxs-lookup"><span data-stu-id="fa279-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa279-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa279-123">Authorization</span></span>|<span data-ttu-id="fa279-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa279-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa279-125">接受</span><span class="sxs-lookup"><span data-stu-id="fa279-125">Accept</span></span>|<span data-ttu-id="fa279-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa279-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa279-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa279-127">Request body</span></span>
<span data-ttu-id="fa279-128">在请求正文中，提供 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa279-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="fa279-129">下表显示创建 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa279-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="fa279-130">属性</span><span class="sxs-lookup"><span data-stu-id="fa279-130">Property</span></span>|<span data-ttu-id="fa279-131">类型</span><span class="sxs-lookup"><span data-stu-id="fa279-131">Type</span></span>|<span data-ttu-id="fa279-132">说明</span><span class="sxs-lookup"><span data-stu-id="fa279-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa279-133">id</span><span class="sxs-lookup"><span data-stu-id="fa279-133">id</span></span>|<span data-ttu-id="fa279-134">String</span><span class="sxs-lookup"><span data-stu-id="fa279-134">String</span></span>|<span data-ttu-id="fa279-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fa279-135">Key of the entity.</span></span>|
|<span data-ttu-id="fa279-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa279-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fa279-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa279-137">DateTimeOffset</span></span>|<span data-ttu-id="fa279-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fa279-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fa279-139">locale</span><span class="sxs-lookup"><span data-stu-id="fa279-139">locale</span></span>|<span data-ttu-id="fa279-140">String</span><span class="sxs-lookup"><span data-stu-id="fa279-140">String</span></span>|<span data-ttu-id="fa279-141">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="fa279-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="fa279-142">subject</span><span class="sxs-lookup"><span data-stu-id="fa279-142">subject</span></span>|<span data-ttu-id="fa279-143">String</span><span class="sxs-lookup"><span data-stu-id="fa279-143">String</span></span>|<span data-ttu-id="fa279-144">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="fa279-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="fa279-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="fa279-145">messageTemplate</span></span>|<span data-ttu-id="fa279-146">String</span><span class="sxs-lookup"><span data-stu-id="fa279-146">String</span></span>|<span data-ttu-id="fa279-147">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="fa279-147">The Message Template content.</span></span>|
|<span data-ttu-id="fa279-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="fa279-148">isDefault</span></span>|<span data-ttu-id="fa279-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa279-149">Boolean</span></span>|<span data-ttu-id="fa279-150">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="fa279-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="fa279-151">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="fa279-151">This flag can only be set.</span></span> <span data-ttu-id="fa279-152">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="fa279-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="fa279-153">响应</span><span class="sxs-lookup"><span data-stu-id="fa279-153">Response</span></span>
<span data-ttu-id="fa279-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa279-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa279-155">示例</span><span class="sxs-lookup"><span data-stu-id="fa279-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa279-156">请求</span><span class="sxs-lookup"><span data-stu-id="fa279-156">Request</span></span>
<span data-ttu-id="fa279-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa279-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="fa279-158">响应</span><span class="sxs-lookup"><span data-stu-id="fa279-158">Response</span></span>
<span data-ttu-id="fa279-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa279-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```






