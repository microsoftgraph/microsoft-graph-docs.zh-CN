---
title: 更新 localizedNotificationMessage
description: 更新 localizedNotificationMessage 对象的属性。
ms.openlocfilehash: d61f97d44e4c5b2e6f5b17e1538620f774200a18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042665"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="27e6c-103">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="27e6c-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="27e6c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27e6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27e6c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27e6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27e6c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="27e6c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27e6c-107">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27e6c-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27e6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27e6c-108">Prerequisites</span></span>
<span data-ttu-id="27e6c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="27e6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27e6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27e6c-111">Permission type</span></span>|<span data-ttu-id="27e6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27e6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27e6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27e6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27e6c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e6c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27e6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27e6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27e6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27e6c-116">Not supported.</span></span>|
|<span data-ttu-id="27e6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="27e6c-117">Application</span></span>|<span data-ttu-id="27e6c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="27e6c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27e6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27e6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="27e6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27e6c-120">Request headers</span></span>
|<span data-ttu-id="27e6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="27e6c-121">Header</span></span>|<span data-ttu-id="27e6c-122">值</span><span class="sxs-lookup"><span data-stu-id="27e6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27e6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27e6c-123">Authorization</span></span>|<span data-ttu-id="27e6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27e6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27e6c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27e6c-125">Accept</span></span>|<span data-ttu-id="27e6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27e6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27e6c-127">Request body</span></span>
<span data-ttu-id="27e6c-128">在请求正文中，提供 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27e6c-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="27e6c-129">下表显示创建 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27e6c-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="27e6c-130">属性</span><span class="sxs-lookup"><span data-stu-id="27e6c-130">Property</span></span>|<span data-ttu-id="27e6c-131">类型</span><span class="sxs-lookup"><span data-stu-id="27e6c-131">Type</span></span>|<span data-ttu-id="27e6c-132">说明</span><span class="sxs-lookup"><span data-stu-id="27e6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27e6c-133">id</span><span class="sxs-lookup"><span data-stu-id="27e6c-133">id</span></span>|<span data-ttu-id="27e6c-134">String</span><span class="sxs-lookup"><span data-stu-id="27e6c-134">String</span></span>|<span data-ttu-id="27e6c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27e6c-135">Key of the entity.</span></span>|
|<span data-ttu-id="27e6c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27e6c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="27e6c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27e6c-137">DateTimeOffset</span></span>|<span data-ttu-id="27e6c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27e6c-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="27e6c-139">locale</span><span class="sxs-lookup"><span data-stu-id="27e6c-139">locale</span></span>|<span data-ttu-id="27e6c-140">String</span><span class="sxs-lookup"><span data-stu-id="27e6c-140">String</span></span>|<span data-ttu-id="27e6c-141">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="27e6c-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="27e6c-142">subject</span><span class="sxs-lookup"><span data-stu-id="27e6c-142">subject</span></span>|<span data-ttu-id="27e6c-143">String</span><span class="sxs-lookup"><span data-stu-id="27e6c-143">String</span></span>|<span data-ttu-id="27e6c-144">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="27e6c-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="27e6c-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="27e6c-145">messageTemplate</span></span>|<span data-ttu-id="27e6c-146">String</span><span class="sxs-lookup"><span data-stu-id="27e6c-146">String</span></span>|<span data-ttu-id="27e6c-147">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="27e6c-147">The Message Template content.</span></span>|
|<span data-ttu-id="27e6c-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="27e6c-148">isDefault</span></span>|<span data-ttu-id="27e6c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="27e6c-149">Boolean</span></span>|<span data-ttu-id="27e6c-150">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="27e6c-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="27e6c-151">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="27e6c-151">This flag can only be set.</span></span> <span data-ttu-id="27e6c-152">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="27e6c-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="27e6c-153">响应</span><span class="sxs-lookup"><span data-stu-id="27e6c-153">Response</span></span>
<span data-ttu-id="27e6c-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27e6c-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27e6c-155">示例</span><span class="sxs-lookup"><span data-stu-id="27e6c-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="27e6c-156">请求</span><span class="sxs-lookup"><span data-stu-id="27e6c-156">Request</span></span>
<span data-ttu-id="27e6c-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27e6c-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="27e6c-158">响应</span><span class="sxs-lookup"><span data-stu-id="27e6c-158">Response</span></span>
<span data-ttu-id="27e6c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27e6c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





