---
title: 更新 notificationMessageTemplate
description: 更新 notificationMessageTemplate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e12702f96f4f50086aff1c738cd44aa23df027bf
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253153"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="376b8-103">更新 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="376b8-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="376b8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="376b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="376b8-105">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="376b8-105">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="376b8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="376b8-106">Prerequisites</span></span>
<span data-ttu-id="376b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="376b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="376b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="376b8-109">Permission type</span></span>|<span data-ttu-id="376b8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="376b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="376b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="376b8-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376b8-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="376b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="376b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="376b8-114">Not supported.</span></span>|
|<span data-ttu-id="376b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="376b8-115">Application</span></span>|<span data-ttu-id="376b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="376b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="376b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="376b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="376b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="376b8-118">Request headers</span></span>
|<span data-ttu-id="376b8-119">标头</span><span class="sxs-lookup"><span data-stu-id="376b8-119">Header</span></span>|<span data-ttu-id="376b8-120">值</span><span class="sxs-lookup"><span data-stu-id="376b8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="376b8-121">Authorization</span></span>|<span data-ttu-id="376b8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="376b8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376b8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="376b8-123">Accept</span></span>|<span data-ttu-id="376b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="376b8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376b8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="376b8-125">Request body</span></span>
<span data-ttu-id="376b8-126">在请求正文中，提供 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="376b8-126">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="376b8-127">下表显示创建 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="376b8-127">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="376b8-128">属性</span><span class="sxs-lookup"><span data-stu-id="376b8-128">Property</span></span>|<span data-ttu-id="376b8-129">类型</span><span class="sxs-lookup"><span data-stu-id="376b8-129">Type</span></span>|<span data-ttu-id="376b8-130">说明</span><span class="sxs-lookup"><span data-stu-id="376b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376b8-131">id</span><span class="sxs-lookup"><span data-stu-id="376b8-131">id</span></span>|<span data-ttu-id="376b8-132">字符串</span><span class="sxs-lookup"><span data-stu-id="376b8-132">String</span></span>|<span data-ttu-id="376b8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="376b8-133">Key of the entity.</span></span>|
|<span data-ttu-id="376b8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="376b8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="376b8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="376b8-135">DateTimeOffset</span></span>|<span data-ttu-id="376b8-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="376b8-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="376b8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="376b8-137">displayName</span></span>|<span data-ttu-id="376b8-138">String</span><span class="sxs-lookup"><span data-stu-id="376b8-138">String</span></span>|<span data-ttu-id="376b8-139">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="376b8-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="376b8-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="376b8-140">defaultLocale</span></span>|<span data-ttu-id="376b8-141">String</span><span class="sxs-lookup"><span data-stu-id="376b8-141">String</span></span>|<span data-ttu-id="376b8-142">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="376b8-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="376b8-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="376b8-143">brandingOptions</span></span>|[<span data-ttu-id="376b8-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="376b8-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="376b8-145">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="376b8-145">The Message Template Branding Options.</span></span> <span data-ttu-id="376b8-146">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="376b8-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="376b8-147">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="376b8-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="376b8-148">响应</span><span class="sxs-lookup"><span data-stu-id="376b8-148">Response</span></span>
<span data-ttu-id="376b8-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="376b8-149">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376b8-150">示例</span><span class="sxs-lookup"><span data-stu-id="376b8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="376b8-151">请求</span><span class="sxs-lookup"><span data-stu-id="376b8-151">Request</span></span>
<span data-ttu-id="376b8-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="376b8-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="376b8-153">响应</span><span class="sxs-lookup"><span data-stu-id="376b8-153">Response</span></span>
<span data-ttu-id="376b8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="376b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



