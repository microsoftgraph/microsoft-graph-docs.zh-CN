---
title: 创建 localizedNotificationMessage
description: 创建新的 localizedNotificationMessage 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 359eb958053dab839d6ce10dc0b27e954389f4b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087367"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="cc35d-103">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="cc35d-103">Create localizedNotificationMessage</span></span>

<span data-ttu-id="cc35d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc35d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc35d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc35d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc35d-106">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc35d-106">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc35d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc35d-107">Prerequisites</span></span>
<span data-ttu-id="cc35d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc35d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc35d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc35d-110">Permission type</span></span>|<span data-ttu-id="cc35d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc35d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc35d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc35d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc35d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc35d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc35d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc35d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc35d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc35d-115">Not supported.</span></span>|
|<span data-ttu-id="cc35d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc35d-116">Application</span></span>|<span data-ttu-id="cc35d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc35d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc35d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc35d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="cc35d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc35d-119">Request headers</span></span>
|<span data-ttu-id="cc35d-120">标头</span><span class="sxs-lookup"><span data-stu-id="cc35d-120">Header</span></span>|<span data-ttu-id="cc35d-121">值</span><span class="sxs-lookup"><span data-stu-id="cc35d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc35d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc35d-122">Authorization</span></span>|<span data-ttu-id="cc35d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cc35d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc35d-124">接受</span><span class="sxs-lookup"><span data-stu-id="cc35d-124">Accept</span></span>|<span data-ttu-id="cc35d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc35d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc35d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc35d-126">Request body</span></span>
<span data-ttu-id="cc35d-127">在请求正文中，提供 localizedNotificationMessage 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc35d-127">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="cc35d-128">下表显示创建 localizedNotificationMessage 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cc35d-128">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="cc35d-129">属性</span><span class="sxs-lookup"><span data-stu-id="cc35d-129">Property</span></span>|<span data-ttu-id="cc35d-130">类型</span><span class="sxs-lookup"><span data-stu-id="cc35d-130">Type</span></span>|<span data-ttu-id="cc35d-131">说明</span><span class="sxs-lookup"><span data-stu-id="cc35d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc35d-132">id</span><span class="sxs-lookup"><span data-stu-id="cc35d-132">id</span></span>|<span data-ttu-id="cc35d-133">String</span><span class="sxs-lookup"><span data-stu-id="cc35d-133">String</span></span>|<span data-ttu-id="cc35d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cc35d-134">Key of the entity.</span></span>|
|<span data-ttu-id="cc35d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc35d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cc35d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc35d-136">DateTimeOffset</span></span>|<span data-ttu-id="cc35d-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cc35d-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="cc35d-138">locale</span><span class="sxs-lookup"><span data-stu-id="cc35d-138">locale</span></span>|<span data-ttu-id="cc35d-139">String</span><span class="sxs-lookup"><span data-stu-id="cc35d-139">String</span></span>|<span data-ttu-id="cc35d-140">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="cc35d-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="cc35d-141">subject</span><span class="sxs-lookup"><span data-stu-id="cc35d-141">subject</span></span>|<span data-ttu-id="cc35d-142">String</span><span class="sxs-lookup"><span data-stu-id="cc35d-142">String</span></span>|<span data-ttu-id="cc35d-143">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="cc35d-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="cc35d-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="cc35d-144">messageTemplate</span></span>|<span data-ttu-id="cc35d-145">String</span><span class="sxs-lookup"><span data-stu-id="cc35d-145">String</span></span>|<span data-ttu-id="cc35d-146">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="cc35d-146">The Message Template content.</span></span>|
|<span data-ttu-id="cc35d-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="cc35d-147">isDefault</span></span>|<span data-ttu-id="cc35d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc35d-148">Boolean</span></span>|<span data-ttu-id="cc35d-149">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="cc35d-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="cc35d-150">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="cc35d-150">This flag can only be set.</span></span> <span data-ttu-id="cc35d-151">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="cc35d-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="cc35d-152">响应</span><span class="sxs-lookup"><span data-stu-id="cc35d-152">Response</span></span>
<span data-ttu-id="cc35d-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc35d-153">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc35d-154">示例</span><span class="sxs-lookup"><span data-stu-id="cc35d-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc35d-155">请求</span><span class="sxs-lookup"><span data-stu-id="cc35d-155">Request</span></span>
<span data-ttu-id="cc35d-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc35d-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="cc35d-157">响应</span><span class="sxs-lookup"><span data-stu-id="cc35d-157">Response</span></span>
<span data-ttu-id="cc35d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc35d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









