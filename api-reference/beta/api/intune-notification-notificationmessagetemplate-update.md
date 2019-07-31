---
title: 更新 notificationMessageTemplate
description: 更新 notificationMessageTemplate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ba404f8a0c738891a9791c3f0875ecc2d4d4d99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994276"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="07cfe-103">更新 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="07cfe-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="07cfe-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07cfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07cfe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07cfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07cfe-106">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07cfe-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07cfe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="07cfe-107">Prerequisites</span></span>
<span data-ttu-id="07cfe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07cfe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="07cfe-110">Permission type</span></span>|<span data-ttu-id="07cfe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="07cfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07cfe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07cfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07cfe-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07cfe-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07cfe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07cfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07cfe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="07cfe-115">Not supported.</span></span>|
|<span data-ttu-id="07cfe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="07cfe-116">Application</span></span>|<span data-ttu-id="07cfe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="07cfe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07cfe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07cfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="07cfe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="07cfe-119">Request headers</span></span>
|<span data-ttu-id="07cfe-120">标头</span><span class="sxs-lookup"><span data-stu-id="07cfe-120">Header</span></span>|<span data-ttu-id="07cfe-121">值</span><span class="sxs-lookup"><span data-stu-id="07cfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07cfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07cfe-122">Authorization</span></span>|<span data-ttu-id="07cfe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07cfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07cfe-124">接受</span><span class="sxs-lookup"><span data-stu-id="07cfe-124">Accept</span></span>|<span data-ttu-id="07cfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07cfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07cfe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="07cfe-126">Request body</span></span>
<span data-ttu-id="07cfe-127">在请求正文中，提供 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07cfe-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="07cfe-128">下表显示创建 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07cfe-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="07cfe-129">属性</span><span class="sxs-lookup"><span data-stu-id="07cfe-129">Property</span></span>|<span data-ttu-id="07cfe-130">类型</span><span class="sxs-lookup"><span data-stu-id="07cfe-130">Type</span></span>|<span data-ttu-id="07cfe-131">说明</span><span class="sxs-lookup"><span data-stu-id="07cfe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07cfe-132">id</span><span class="sxs-lookup"><span data-stu-id="07cfe-132">id</span></span>|<span data-ttu-id="07cfe-133">String</span><span class="sxs-lookup"><span data-stu-id="07cfe-133">String</span></span>|<span data-ttu-id="07cfe-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="07cfe-134">Key of the entity.</span></span>|
|<span data-ttu-id="07cfe-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07cfe-135">lastModifiedDateTime</span></span>|<span data-ttu-id="07cfe-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07cfe-136">DateTimeOffset</span></span>|<span data-ttu-id="07cfe-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="07cfe-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="07cfe-138">displayName</span><span class="sxs-lookup"><span data-stu-id="07cfe-138">displayName</span></span>|<span data-ttu-id="07cfe-139">字符串</span><span class="sxs-lookup"><span data-stu-id="07cfe-139">String</span></span>|<span data-ttu-id="07cfe-140">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="07cfe-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="07cfe-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="07cfe-141">defaultLocale</span></span>|<span data-ttu-id="07cfe-142">String</span><span class="sxs-lookup"><span data-stu-id="07cfe-142">String</span></span>|<span data-ttu-id="07cfe-143">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="07cfe-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="07cfe-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="07cfe-144">brandingOptions</span></span>|[<span data-ttu-id="07cfe-145">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="07cfe-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="07cfe-146">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="07cfe-146">The Message Template Branding Options.</span></span> <span data-ttu-id="07cfe-147">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="07cfe-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="07cfe-148">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="07cfe-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="07cfe-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07cfe-149">roleScopeTagIds</span></span>|<span data-ttu-id="07cfe-150">String collection</span><span class="sxs-lookup"><span data-stu-id="07cfe-150">String collection</span></span>|<span data-ttu-id="07cfe-151">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="07cfe-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="07cfe-152">响应</span><span class="sxs-lookup"><span data-stu-id="07cfe-152">Response</span></span>
<span data-ttu-id="07cfe-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07cfe-153">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07cfe-154">示例</span><span class="sxs-lookup"><span data-stu-id="07cfe-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="07cfe-155">请求</span><span class="sxs-lookup"><span data-stu-id="07cfe-155">Request</span></span>
<span data-ttu-id="07cfe-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07cfe-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 259

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="07cfe-157">响应</span><span class="sxs-lookup"><span data-stu-id="07cfe-157">Response</span></span>
<span data-ttu-id="07cfe-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07cfe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





