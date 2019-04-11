---
title: 创建 localizedNotificationMessage
description: 创建新的 localizedNotificationMessage 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5458605b4b4e58b27e65298f709121283fc91ecd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793306"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="efd05-103">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="efd05-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="efd05-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efd05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efd05-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efd05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd05-106">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efd05-106">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efd05-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="efd05-107">Prerequisites</span></span>
<span data-ttu-id="efd05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd05-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd05-110">Permission type</span></span>|<span data-ttu-id="efd05-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efd05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efd05-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efd05-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd05-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efd05-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efd05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd05-115">Not supported.</span></span>|
|<span data-ttu-id="efd05-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd05-116">Application</span></span>|<span data-ttu-id="efd05-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efd05-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="efd05-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd05-119">Request headers</span></span>
|<span data-ttu-id="efd05-120">标头</span><span class="sxs-lookup"><span data-stu-id="efd05-120">Header</span></span>|<span data-ttu-id="efd05-121">值</span><span class="sxs-lookup"><span data-stu-id="efd05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efd05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd05-122">Authorization</span></span>|<span data-ttu-id="efd05-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efd05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efd05-124">接受</span><span class="sxs-lookup"><span data-stu-id="efd05-124">Accept</span></span>|<span data-ttu-id="efd05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efd05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd05-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd05-126">Request body</span></span>
<span data-ttu-id="efd05-127">在请求正文中，提供 localizedNotificationMessage 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efd05-127">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="efd05-128">下表显示创建 localizedNotificationMessage 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="efd05-128">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="efd05-129">属性</span><span class="sxs-lookup"><span data-stu-id="efd05-129">Property</span></span>|<span data-ttu-id="efd05-130">类型</span><span class="sxs-lookup"><span data-stu-id="efd05-130">Type</span></span>|<span data-ttu-id="efd05-131">说明</span><span class="sxs-lookup"><span data-stu-id="efd05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd05-132">id</span><span class="sxs-lookup"><span data-stu-id="efd05-132">id</span></span>|<span data-ttu-id="efd05-133">String</span><span class="sxs-lookup"><span data-stu-id="efd05-133">String</span></span>|<span data-ttu-id="efd05-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="efd05-134">Key of the entity.</span></span>|
|<span data-ttu-id="efd05-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efd05-135">lastModifiedDateTime</span></span>|<span data-ttu-id="efd05-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efd05-136">DateTimeOffset</span></span>|<span data-ttu-id="efd05-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="efd05-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="efd05-138">locale</span><span class="sxs-lookup"><span data-stu-id="efd05-138">locale</span></span>|<span data-ttu-id="efd05-139">String</span><span class="sxs-lookup"><span data-stu-id="efd05-139">String</span></span>|<span data-ttu-id="efd05-140">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="efd05-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="efd05-141">subject</span><span class="sxs-lookup"><span data-stu-id="efd05-141">subject</span></span>|<span data-ttu-id="efd05-142">String</span><span class="sxs-lookup"><span data-stu-id="efd05-142">String</span></span>|<span data-ttu-id="efd05-143">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="efd05-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="efd05-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="efd05-144">messageTemplate</span></span>|<span data-ttu-id="efd05-145">String</span><span class="sxs-lookup"><span data-stu-id="efd05-145">String</span></span>|<span data-ttu-id="efd05-146">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="efd05-146">The Message Template content.</span></span>|
|<span data-ttu-id="efd05-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="efd05-147">isDefault</span></span>|<span data-ttu-id="efd05-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="efd05-148">Boolean</span></span>|<span data-ttu-id="efd05-149">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="efd05-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="efd05-150">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="efd05-150">This flag can only be set.</span></span> <span data-ttu-id="efd05-151">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="efd05-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="efd05-152">响应</span><span class="sxs-lookup"><span data-stu-id="efd05-152">Response</span></span>
<span data-ttu-id="efd05-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efd05-153">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd05-154">示例</span><span class="sxs-lookup"><span data-stu-id="efd05-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="efd05-155">请求</span><span class="sxs-lookup"><span data-stu-id="efd05-155">Request</span></span>
<span data-ttu-id="efd05-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efd05-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efd05-157">响应</span><span class="sxs-lookup"><span data-stu-id="efd05-157">Response</span></span>
<span data-ttu-id="efd05-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efd05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





