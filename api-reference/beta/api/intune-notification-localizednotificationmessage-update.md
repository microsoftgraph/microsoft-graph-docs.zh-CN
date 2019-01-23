---
title: 更新 localizedNotificationMessage
description: 更新 localizedNotificationMessage 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bae1ef62325a7675b626be0bc21f65e3cb45b513
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395501"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="bc3c5-103">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bc3c5-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="bc3c5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc3c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc3c5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc3c5-107">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc3c5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc3c5-108">Prerequisites</span></span>
<span data-ttu-id="bc3c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc3c5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc3c5-111">Permission type</span></span>|<span data-ttu-id="bc3c5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc3c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc3c5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc3c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc3c5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc3c5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bc3c5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc3c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc3c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-116">Not supported.</span></span>|
|<span data-ttu-id="bc3c5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc3c5-117">Application</span></span>|<span data-ttu-id="bc3c5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc3c5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc3c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="bc3c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc3c5-120">Request headers</span></span>
|<span data-ttu-id="bc3c5-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc3c5-121">Header</span></span>|<span data-ttu-id="bc3c5-122">值</span><span class="sxs-lookup"><span data-stu-id="bc3c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc3c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc3c5-123">Authorization</span></span>|<span data-ttu-id="bc3c5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc3c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc3c5-125">Accept</span></span>|<span data-ttu-id="bc3c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc3c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc3c5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc3c5-127">Request body</span></span>
<span data-ttu-id="bc3c5-128">在请求正文中，提供 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="bc3c5-129">下表显示创建 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="bc3c5-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc3c5-130">Property</span></span>|<span data-ttu-id="bc3c5-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc3c5-131">Type</span></span>|<span data-ttu-id="bc3c5-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc3c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc3c5-133">id</span><span class="sxs-lookup"><span data-stu-id="bc3c5-133">id</span></span>|<span data-ttu-id="bc3c5-134">String</span><span class="sxs-lookup"><span data-stu-id="bc3c5-134">String</span></span>|<span data-ttu-id="bc3c5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-135">Key of the entity.</span></span>|
|<span data-ttu-id="bc3c5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc3c5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bc3c5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc3c5-137">DateTimeOffset</span></span>|<span data-ttu-id="bc3c5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bc3c5-139">locale</span><span class="sxs-lookup"><span data-stu-id="bc3c5-139">locale</span></span>|<span data-ttu-id="bc3c5-140">String</span><span class="sxs-lookup"><span data-stu-id="bc3c5-140">String</span></span>|<span data-ttu-id="bc3c5-141">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="bc3c5-142">subject</span><span class="sxs-lookup"><span data-stu-id="bc3c5-142">subject</span></span>|<span data-ttu-id="bc3c5-143">String</span><span class="sxs-lookup"><span data-stu-id="bc3c5-143">String</span></span>|<span data-ttu-id="bc3c5-144">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="bc3c5-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="bc3c5-145">messageTemplate</span></span>|<span data-ttu-id="bc3c5-146">String</span><span class="sxs-lookup"><span data-stu-id="bc3c5-146">String</span></span>|<span data-ttu-id="bc3c5-147">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-147">The Message Template content.</span></span>|
|<span data-ttu-id="bc3c5-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="bc3c5-148">isDefault</span></span>|<span data-ttu-id="bc3c5-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc3c5-149">Boolean</span></span>|<span data-ttu-id="bc3c5-150">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="bc3c5-151">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-151">This flag can only be set.</span></span> <span data-ttu-id="bc3c5-152">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="bc3c5-153">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c5-153">Response</span></span>
<span data-ttu-id="bc3c5-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc3c5-155">示例</span><span class="sxs-lookup"><span data-stu-id="bc3c5-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc3c5-156">请求</span><span class="sxs-lookup"><span data-stu-id="bc3c5-156">Request</span></span>
<span data-ttu-id="bc3c5-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc3c5-158">响应</span><span class="sxs-lookup"><span data-stu-id="bc3c5-158">Response</span></span>
<span data-ttu-id="bc3c5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc3c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




