---
title: 更新 localizedNotificationMessage
description: 更新 localizedNotificationMessage 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f6f3ddffd84976f2a7a1cbc8355e44efdbaffc7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462619"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="c807b-103">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="c807b-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="c807b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c807b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c807b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c807b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c807b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c807b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c807b-107">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c807b-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c807b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c807b-108">Prerequisites</span></span>
<span data-ttu-id="c807b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c807b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c807b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c807b-111">Permission type</span></span>|<span data-ttu-id="c807b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c807b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c807b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c807b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c807b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c807b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c807b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c807b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c807b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c807b-116">Not supported.</span></span>|
|<span data-ttu-id="c807b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c807b-117">Application</span></span>|<span data-ttu-id="c807b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c807b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c807b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c807b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="c807b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c807b-120">Request headers</span></span>
|<span data-ttu-id="c807b-121">标头</span><span class="sxs-lookup"><span data-stu-id="c807b-121">Header</span></span>|<span data-ttu-id="c807b-122">值</span><span class="sxs-lookup"><span data-stu-id="c807b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c807b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c807b-123">Authorization</span></span>|<span data-ttu-id="c807b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c807b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c807b-125">接受</span><span class="sxs-lookup"><span data-stu-id="c807b-125">Accept</span></span>|<span data-ttu-id="c807b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c807b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c807b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c807b-127">Request body</span></span>
<span data-ttu-id="c807b-128">在请求正文中，提供 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c807b-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="c807b-129">下表显示创建 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c807b-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="c807b-130">属性</span><span class="sxs-lookup"><span data-stu-id="c807b-130">Property</span></span>|<span data-ttu-id="c807b-131">类型</span><span class="sxs-lookup"><span data-stu-id="c807b-131">Type</span></span>|<span data-ttu-id="c807b-132">说明</span><span class="sxs-lookup"><span data-stu-id="c807b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c807b-133">id</span><span class="sxs-lookup"><span data-stu-id="c807b-133">id</span></span>|<span data-ttu-id="c807b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c807b-134">String</span></span>|<span data-ttu-id="c807b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c807b-135">Key of the entity.</span></span>|
|<span data-ttu-id="c807b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c807b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c807b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c807b-137">DateTimeOffset</span></span>|<span data-ttu-id="c807b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c807b-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c807b-139">locale</span><span class="sxs-lookup"><span data-stu-id="c807b-139">locale</span></span>|<span data-ttu-id="c807b-140">String</span><span class="sxs-lookup"><span data-stu-id="c807b-140">String</span></span>|<span data-ttu-id="c807b-141">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="c807b-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="c807b-142">subject</span><span class="sxs-lookup"><span data-stu-id="c807b-142">subject</span></span>|<span data-ttu-id="c807b-143">String</span><span class="sxs-lookup"><span data-stu-id="c807b-143">String</span></span>|<span data-ttu-id="c807b-144">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="c807b-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="c807b-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="c807b-145">messageTemplate</span></span>|<span data-ttu-id="c807b-146">String</span><span class="sxs-lookup"><span data-stu-id="c807b-146">String</span></span>|<span data-ttu-id="c807b-147">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="c807b-147">The Message Template content.</span></span>|
|<span data-ttu-id="c807b-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="c807b-148">isDefault</span></span>|<span data-ttu-id="c807b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c807b-149">Boolean</span></span>|<span data-ttu-id="c807b-150">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="c807b-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="c807b-151">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="c807b-151">This flag can only be set.</span></span> <span data-ttu-id="c807b-152">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c807b-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="c807b-153">响应</span><span class="sxs-lookup"><span data-stu-id="c807b-153">Response</span></span>
<span data-ttu-id="c807b-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c807b-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c807b-155">示例</span><span class="sxs-lookup"><span data-stu-id="c807b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c807b-156">请求</span><span class="sxs-lookup"><span data-stu-id="c807b-156">Request</span></span>
<span data-ttu-id="c807b-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c807b-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c807b-158">响应</span><span class="sxs-lookup"><span data-stu-id="c807b-158">Response</span></span>
<span data-ttu-id="c807b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c807b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





