---
title: 创建 localizedNotificationMessage
description: 创建新的 localizedNotificationMessage 对象。
author: tfitzmac
ms.openlocfilehash: 8bc782f69e769e32acd29932b4f224c7cf764c04
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353541"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="21020-103">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="21020-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="21020-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="21020-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21020-105">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21020-105">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21020-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="21020-106">Prerequisites</span></span>
<span data-ttu-id="21020-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="21020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21020-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="21020-109">Permission type</span></span>|<span data-ttu-id="21020-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21020-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21020-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21020-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21020-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21020-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21020-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21020-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21020-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="21020-114">Not supported.</span></span>|
|<span data-ttu-id="21020-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="21020-115">Application</span></span>|<span data-ttu-id="21020-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21020-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21020-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21020-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="21020-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="21020-118">Request headers</span></span>
|<span data-ttu-id="21020-119">标头</span><span class="sxs-lookup"><span data-stu-id="21020-119">Header</span></span>|<span data-ttu-id="21020-120">值</span><span class="sxs-lookup"><span data-stu-id="21020-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21020-121">授权</span><span class="sxs-lookup"><span data-stu-id="21020-121">Authorization</span></span>|<span data-ttu-id="21020-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21020-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21020-123">Accept</span><span class="sxs-lookup"><span data-stu-id="21020-123">Accept</span></span>|<span data-ttu-id="21020-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21020-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21020-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="21020-125">Request body</span></span>
<span data-ttu-id="21020-126">在请求正文中，提供 localizedNotificationMessage 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21020-126">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="21020-127">下表显示创建 localizedNotificationMessage 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="21020-127">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="21020-128">属性</span><span class="sxs-lookup"><span data-stu-id="21020-128">Property</span></span>|<span data-ttu-id="21020-129">类型</span><span class="sxs-lookup"><span data-stu-id="21020-129">Type</span></span>|<span data-ttu-id="21020-130">说明</span><span class="sxs-lookup"><span data-stu-id="21020-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21020-131">id</span><span class="sxs-lookup"><span data-stu-id="21020-131">id</span></span>|<span data-ttu-id="21020-132">String</span><span class="sxs-lookup"><span data-stu-id="21020-132">String</span></span>|<span data-ttu-id="21020-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="21020-133">Key of the entity.</span></span>|
|<span data-ttu-id="21020-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21020-134">lastModifiedDateTime</span></span>|<span data-ttu-id="21020-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21020-135">DateTimeOffset</span></span>|<span data-ttu-id="21020-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="21020-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="21020-137">locale</span><span class="sxs-lookup"><span data-stu-id="21020-137">locale</span></span>|<span data-ttu-id="21020-138">String</span><span class="sxs-lookup"><span data-stu-id="21020-138">String</span></span>|<span data-ttu-id="21020-139">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="21020-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="21020-140">subject</span><span class="sxs-lookup"><span data-stu-id="21020-140">subject</span></span>|<span data-ttu-id="21020-141">String</span><span class="sxs-lookup"><span data-stu-id="21020-141">String</span></span>|<span data-ttu-id="21020-142">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="21020-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="21020-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="21020-143">messageTemplate</span></span>|<span data-ttu-id="21020-144">String</span><span class="sxs-lookup"><span data-stu-id="21020-144">String</span></span>|<span data-ttu-id="21020-145">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="21020-145">The Message Template content.</span></span>|
|<span data-ttu-id="21020-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="21020-146">isDefault</span></span>|<span data-ttu-id="21020-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="21020-147">Boolean</span></span>|<span data-ttu-id="21020-148">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="21020-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="21020-149">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="21020-149">This flag can only be set.</span></span> <span data-ttu-id="21020-150">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="21020-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="21020-151">响应</span><span class="sxs-lookup"><span data-stu-id="21020-151">Response</span></span>
<span data-ttu-id="21020-152">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21020-152">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21020-153">示例</span><span class="sxs-lookup"><span data-stu-id="21020-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="21020-154">请求</span><span class="sxs-lookup"><span data-stu-id="21020-154">Request</span></span>
<span data-ttu-id="21020-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21020-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21020-156">响应</span><span class="sxs-lookup"><span data-stu-id="21020-156">Response</span></span>
<span data-ttu-id="21020-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21020-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



