---
title: 创建 localizedNotificationMessage
description: 创建新的 localizedNotificationMessage 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da30922d7de4f4c8291befdac1471ff2e56bc03d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958779"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="53192-103">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="53192-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="53192-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53192-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53192-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53192-106">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53192-106">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53192-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="53192-107">Prerequisites</span></span>
<span data-ttu-id="53192-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53192-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53192-110">Permission type</span></span>|<span data-ttu-id="53192-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53192-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53192-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53192-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53192-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53192-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53192-115">Not supported.</span></span>|
|<span data-ttu-id="53192-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53192-116">Application</span></span>|<span data-ttu-id="53192-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="53192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53192-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53192-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="53192-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53192-119">Request headers</span></span>
|<span data-ttu-id="53192-120">标头</span><span class="sxs-lookup"><span data-stu-id="53192-120">Header</span></span>|<span data-ttu-id="53192-121">值</span><span class="sxs-lookup"><span data-stu-id="53192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53192-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53192-122">Authorization</span></span>|<span data-ttu-id="53192-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53192-124">接受</span><span class="sxs-lookup"><span data-stu-id="53192-124">Accept</span></span>|<span data-ttu-id="53192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53192-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53192-126">Request body</span></span>
<span data-ttu-id="53192-127">在请求正文中，提供 localizedNotificationMessage 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53192-127">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="53192-128">下表显示创建 localizedNotificationMessage 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53192-128">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="53192-129">属性</span><span class="sxs-lookup"><span data-stu-id="53192-129">Property</span></span>|<span data-ttu-id="53192-130">类型</span><span class="sxs-lookup"><span data-stu-id="53192-130">Type</span></span>|<span data-ttu-id="53192-131">说明</span><span class="sxs-lookup"><span data-stu-id="53192-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53192-132">id</span><span class="sxs-lookup"><span data-stu-id="53192-132">id</span></span>|<span data-ttu-id="53192-133">String</span><span class="sxs-lookup"><span data-stu-id="53192-133">String</span></span>|<span data-ttu-id="53192-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53192-134">Key of the entity.</span></span>|
|<span data-ttu-id="53192-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53192-135">lastModifiedDateTime</span></span>|<span data-ttu-id="53192-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53192-136">DateTimeOffset</span></span>|<span data-ttu-id="53192-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="53192-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="53192-138">locale</span><span class="sxs-lookup"><span data-stu-id="53192-138">locale</span></span>|<span data-ttu-id="53192-139">String</span><span class="sxs-lookup"><span data-stu-id="53192-139">String</span></span>|<span data-ttu-id="53192-140">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="53192-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="53192-141">subject</span><span class="sxs-lookup"><span data-stu-id="53192-141">subject</span></span>|<span data-ttu-id="53192-142">String</span><span class="sxs-lookup"><span data-stu-id="53192-142">String</span></span>|<span data-ttu-id="53192-143">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="53192-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="53192-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="53192-144">messageTemplate</span></span>|<span data-ttu-id="53192-145">String</span><span class="sxs-lookup"><span data-stu-id="53192-145">String</span></span>|<span data-ttu-id="53192-146">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="53192-146">The Message Template content.</span></span>|
|<span data-ttu-id="53192-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="53192-147">isDefault</span></span>|<span data-ttu-id="53192-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="53192-148">Boolean</span></span>|<span data-ttu-id="53192-149">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="53192-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="53192-150">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="53192-150">This flag can only be set.</span></span> <span data-ttu-id="53192-151">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="53192-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="53192-152">响应</span><span class="sxs-lookup"><span data-stu-id="53192-152">Response</span></span>
<span data-ttu-id="53192-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53192-153">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53192-154">示例</span><span class="sxs-lookup"><span data-stu-id="53192-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="53192-155">请求</span><span class="sxs-lookup"><span data-stu-id="53192-155">Request</span></span>
<span data-ttu-id="53192-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53192-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53192-157">响应</span><span class="sxs-lookup"><span data-stu-id="53192-157">Response</span></span>
<span data-ttu-id="53192-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53192-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




