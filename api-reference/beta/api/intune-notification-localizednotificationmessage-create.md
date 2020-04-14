---
title: 创建 localizedNotificationMessage
description: 创建新的 localizedNotificationMessage 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b08bf858e496b59e3e3440c649c8c5457402e46b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441413"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="08c94-103">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="08c94-103">Create localizedNotificationMessage</span></span>

<span data-ttu-id="08c94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08c94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08c94-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08c94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08c94-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08c94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08c94-107">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08c94-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08c94-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08c94-108">Prerequisites</span></span>
<span data-ttu-id="08c94-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08c94-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08c94-111">Permission type</span></span>|<span data-ttu-id="08c94-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08c94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08c94-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08c94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08c94-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c94-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08c94-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08c94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08c94-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08c94-116">Not supported.</span></span>|
|<span data-ttu-id="08c94-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08c94-117">Application</span></span>|<span data-ttu-id="08c94-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c94-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08c94-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08c94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="08c94-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08c94-120">Request headers</span></span>
|<span data-ttu-id="08c94-121">标头</span><span class="sxs-lookup"><span data-stu-id="08c94-121">Header</span></span>|<span data-ttu-id="08c94-122">值</span><span class="sxs-lookup"><span data-stu-id="08c94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08c94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08c94-123">Authorization</span></span>|<span data-ttu-id="08c94-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08c94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08c94-125">接受</span><span class="sxs-lookup"><span data-stu-id="08c94-125">Accept</span></span>|<span data-ttu-id="08c94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08c94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08c94-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08c94-127">Request body</span></span>
<span data-ttu-id="08c94-128">在请求正文中，提供 localizedNotificationMessage 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08c94-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="08c94-129">下表显示创建 localizedNotificationMessage 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08c94-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="08c94-130">属性</span><span class="sxs-lookup"><span data-stu-id="08c94-130">Property</span></span>|<span data-ttu-id="08c94-131">类型</span><span class="sxs-lookup"><span data-stu-id="08c94-131">Type</span></span>|<span data-ttu-id="08c94-132">说明</span><span class="sxs-lookup"><span data-stu-id="08c94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c94-133">id</span><span class="sxs-lookup"><span data-stu-id="08c94-133">id</span></span>|<span data-ttu-id="08c94-134">字符串</span><span class="sxs-lookup"><span data-stu-id="08c94-134">String</span></span>|<span data-ttu-id="08c94-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="08c94-135">Key of the entity.</span></span>|
|<span data-ttu-id="08c94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08c94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="08c94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c94-137">DateTimeOffset</span></span>|<span data-ttu-id="08c94-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="08c94-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="08c94-139">locale</span><span class="sxs-lookup"><span data-stu-id="08c94-139">locale</span></span>|<span data-ttu-id="08c94-140">String</span><span class="sxs-lookup"><span data-stu-id="08c94-140">String</span></span>|<span data-ttu-id="08c94-141">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="08c94-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="08c94-142">subject</span><span class="sxs-lookup"><span data-stu-id="08c94-142">subject</span></span>|<span data-ttu-id="08c94-143">String</span><span class="sxs-lookup"><span data-stu-id="08c94-143">String</span></span>|<span data-ttu-id="08c94-144">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="08c94-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="08c94-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="08c94-145">messageTemplate</span></span>|<span data-ttu-id="08c94-146">String</span><span class="sxs-lookup"><span data-stu-id="08c94-146">String</span></span>|<span data-ttu-id="08c94-147">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="08c94-147">The Message Template content.</span></span>|
|<span data-ttu-id="08c94-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="08c94-148">isDefault</span></span>|<span data-ttu-id="08c94-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="08c94-149">Boolean</span></span>|<span data-ttu-id="08c94-150">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="08c94-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="08c94-151">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="08c94-151">This flag can only be set.</span></span> <span data-ttu-id="08c94-152">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="08c94-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="08c94-153">响应</span><span class="sxs-lookup"><span data-stu-id="08c94-153">Response</span></span>
<span data-ttu-id="08c94-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08c94-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08c94-155">示例</span><span class="sxs-lookup"><span data-stu-id="08c94-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="08c94-156">请求</span><span class="sxs-lookup"><span data-stu-id="08c94-156">Request</span></span>
<span data-ttu-id="08c94-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08c94-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="08c94-158">响应</span><span class="sxs-lookup"><span data-stu-id="08c94-158">Response</span></span>
<span data-ttu-id="08c94-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08c94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



