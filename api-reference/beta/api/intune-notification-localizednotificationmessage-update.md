---
title: 更新 localizedNotificationMessage
description: 更新 localizedNotificationMessage 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7aa5f527fe8e4f55d422722a8f409ba2d10e32f7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803159"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="e39b3-103">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="e39b3-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="e39b3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e39b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e39b3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e39b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e39b3-106">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e39b3-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e39b3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e39b3-107">Prerequisites</span></span>
<span data-ttu-id="e39b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e39b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e39b3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e39b3-110">Permission type</span></span>|<span data-ttu-id="e39b3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e39b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e39b3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e39b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e39b3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39b3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e39b3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e39b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e39b3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e39b3-115">Not supported.</span></span>|
|<span data-ttu-id="e39b3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e39b3-116">Application</span></span>|<span data-ttu-id="e39b3-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39b3-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e39b3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e39b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="e39b3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e39b3-119">Request headers</span></span>
|<span data-ttu-id="e39b3-120">标头</span><span class="sxs-lookup"><span data-stu-id="e39b3-120">Header</span></span>|<span data-ttu-id="e39b3-121">值</span><span class="sxs-lookup"><span data-stu-id="e39b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e39b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e39b3-122">Authorization</span></span>|<span data-ttu-id="e39b3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e39b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e39b3-124">接受</span><span class="sxs-lookup"><span data-stu-id="e39b3-124">Accept</span></span>|<span data-ttu-id="e39b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e39b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e39b3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e39b3-126">Request body</span></span>
<span data-ttu-id="e39b3-127">在请求正文中，提供 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e39b3-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="e39b3-128">下表显示创建 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e39b3-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="e39b3-129">属性</span><span class="sxs-lookup"><span data-stu-id="e39b3-129">Property</span></span>|<span data-ttu-id="e39b3-130">类型</span><span class="sxs-lookup"><span data-stu-id="e39b3-130">Type</span></span>|<span data-ttu-id="e39b3-131">说明</span><span class="sxs-lookup"><span data-stu-id="e39b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e39b3-132">id</span><span class="sxs-lookup"><span data-stu-id="e39b3-132">id</span></span>|<span data-ttu-id="e39b3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e39b3-133">String</span></span>|<span data-ttu-id="e39b3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e39b3-134">Key of the entity.</span></span>|
|<span data-ttu-id="e39b3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e39b3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e39b3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39b3-136">DateTimeOffset</span></span>|<span data-ttu-id="e39b3-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e39b3-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e39b3-138">locale</span><span class="sxs-lookup"><span data-stu-id="e39b3-138">locale</span></span>|<span data-ttu-id="e39b3-139">String</span><span class="sxs-lookup"><span data-stu-id="e39b3-139">String</span></span>|<span data-ttu-id="e39b3-140">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="e39b3-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="e39b3-141">subject</span><span class="sxs-lookup"><span data-stu-id="e39b3-141">subject</span></span>|<span data-ttu-id="e39b3-142">String</span><span class="sxs-lookup"><span data-stu-id="e39b3-142">String</span></span>|<span data-ttu-id="e39b3-143">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="e39b3-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="e39b3-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="e39b3-144">messageTemplate</span></span>|<span data-ttu-id="e39b3-145">String</span><span class="sxs-lookup"><span data-stu-id="e39b3-145">String</span></span>|<span data-ttu-id="e39b3-146">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="e39b3-146">The Message Template content.</span></span>|
|<span data-ttu-id="e39b3-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="e39b3-147">isDefault</span></span>|<span data-ttu-id="e39b3-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e39b3-148">Boolean</span></span>|<span data-ttu-id="e39b3-149">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="e39b3-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="e39b3-150">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="e39b3-150">This flag can only be set.</span></span> <span data-ttu-id="e39b3-151">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="e39b3-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="e39b3-152">响应</span><span class="sxs-lookup"><span data-stu-id="e39b3-152">Response</span></span>
<span data-ttu-id="e39b3-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e39b3-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e39b3-154">示例</span><span class="sxs-lookup"><span data-stu-id="e39b3-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e39b3-155">请求</span><span class="sxs-lookup"><span data-stu-id="e39b3-155">Request</span></span>
<span data-ttu-id="e39b3-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e39b3-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e39b3-157">响应</span><span class="sxs-lookup"><span data-stu-id="e39b3-157">Response</span></span>
<span data-ttu-id="e39b3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e39b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




