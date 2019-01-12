---
title: 创建 notificationMessageTemplate
description: 创建新的 notificationMessageTemplate 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d7e8fb5f7e718ec2ec1c0a0f5b35241ef408aaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912349"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="0292f-103">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="0292f-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="0292f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0292f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0292f-105">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0292f-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0292f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0292f-106">Prerequisites</span></span>
<span data-ttu-id="0292f-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0292f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0292f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0292f-109">Permission type</span></span>|<span data-ttu-id="0292f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0292f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0292f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0292f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0292f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0292f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0292f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0292f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0292f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0292f-114">Not supported.</span></span>|
|<span data-ttu-id="0292f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0292f-115">Application</span></span>|<span data-ttu-id="0292f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0292f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0292f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0292f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="0292f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0292f-118">Request headers</span></span>
|<span data-ttu-id="0292f-119">标头</span><span class="sxs-lookup"><span data-stu-id="0292f-119">Header</span></span>|<span data-ttu-id="0292f-120">值</span><span class="sxs-lookup"><span data-stu-id="0292f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0292f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0292f-121">Authorization</span></span>|<span data-ttu-id="0292f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0292f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0292f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0292f-123">Accept</span></span>|<span data-ttu-id="0292f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0292f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0292f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0292f-125">Request body</span></span>
<span data-ttu-id="0292f-126">在请求正文中，提供 notificationMessageTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0292f-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="0292f-127">下表显示创建 notificationMessageTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0292f-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="0292f-128">属性</span><span class="sxs-lookup"><span data-stu-id="0292f-128">Property</span></span>|<span data-ttu-id="0292f-129">类型</span><span class="sxs-lookup"><span data-stu-id="0292f-129">Type</span></span>|<span data-ttu-id="0292f-130">说明</span><span class="sxs-lookup"><span data-stu-id="0292f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0292f-131">id</span><span class="sxs-lookup"><span data-stu-id="0292f-131">id</span></span>|<span data-ttu-id="0292f-132">String</span><span class="sxs-lookup"><span data-stu-id="0292f-132">String</span></span>|<span data-ttu-id="0292f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0292f-133">Key of the entity.</span></span>|
|<span data-ttu-id="0292f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0292f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="0292f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0292f-135">DateTimeOffset</span></span>|<span data-ttu-id="0292f-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0292f-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0292f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0292f-137">displayName</span></span>|<span data-ttu-id="0292f-138">String</span><span class="sxs-lookup"><span data-stu-id="0292f-138">String</span></span>|<span data-ttu-id="0292f-139">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0292f-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="0292f-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="0292f-140">defaultLocale</span></span>|<span data-ttu-id="0292f-141">String</span><span class="sxs-lookup"><span data-stu-id="0292f-141">String</span></span>|<span data-ttu-id="0292f-142">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="0292f-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="0292f-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="0292f-143">brandingOptions</span></span>|[<span data-ttu-id="0292f-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="0292f-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="0292f-145">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="0292f-145">The Message Template Branding Options.</span></span> <span data-ttu-id="0292f-146">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="0292f-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="0292f-147">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="0292f-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="0292f-148">响应</span><span class="sxs-lookup"><span data-stu-id="0292f-148">Response</span></span>
<span data-ttu-id="0292f-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0292f-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0292f-150">示例</span><span class="sxs-lookup"><span data-stu-id="0292f-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="0292f-151">请求</span><span class="sxs-lookup"><span data-stu-id="0292f-151">Request</span></span>
<span data-ttu-id="0292f-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0292f-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="0292f-153">响应</span><span class="sxs-lookup"><span data-stu-id="0292f-153">Response</span></span>
<span data-ttu-id="0292f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0292f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```



