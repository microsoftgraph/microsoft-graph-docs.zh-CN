---
title: 创建 notificationMessageTemplate
description: 创建新的 notificationMessageTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0252c4a84d3aad9ce6f42c8442878a969626604
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125882"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="8d924-103">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8d924-103">Create notificationMessageTemplate</span></span>

<span data-ttu-id="8d924-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d924-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d924-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d924-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d924-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d924-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d924-107">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8d924-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d924-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d924-108">Prerequisites</span></span>
<span data-ttu-id="8d924-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d924-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d924-111">Permission type</span></span>|<span data-ttu-id="8d924-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d924-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d924-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d924-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d924-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d924-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d924-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d924-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d924-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d924-116">Not supported.</span></span>|
|<span data-ttu-id="8d924-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d924-117">Application</span></span>|<span data-ttu-id="8d924-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d924-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d924-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d924-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="8d924-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d924-120">Request headers</span></span>
|<span data-ttu-id="8d924-121">标头</span><span class="sxs-lookup"><span data-stu-id="8d924-121">Header</span></span>|<span data-ttu-id="8d924-122">值</span><span class="sxs-lookup"><span data-stu-id="8d924-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d924-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d924-123">Authorization</span></span>|<span data-ttu-id="8d924-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d924-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d924-125">接受</span><span class="sxs-lookup"><span data-stu-id="8d924-125">Accept</span></span>|<span data-ttu-id="8d924-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d924-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d924-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d924-127">Request body</span></span>
<span data-ttu-id="8d924-128">在请求正文中，提供 notificationMessageTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d924-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="8d924-129">下表显示创建 notificationMessageTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8d924-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="8d924-130">属性</span><span class="sxs-lookup"><span data-stu-id="8d924-130">Property</span></span>|<span data-ttu-id="8d924-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d924-131">Type</span></span>|<span data-ttu-id="8d924-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d924-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d924-133">id</span><span class="sxs-lookup"><span data-stu-id="8d924-133">id</span></span>|<span data-ttu-id="8d924-134">String</span><span class="sxs-lookup"><span data-stu-id="8d924-134">String</span></span>|<span data-ttu-id="8d924-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8d924-135">Key of the entity.</span></span>|
|<span data-ttu-id="8d924-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d924-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d924-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d924-137">DateTimeOffset</span></span>|<span data-ttu-id="8d924-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8d924-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8d924-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8d924-139">displayName</span></span>|<span data-ttu-id="8d924-140">String</span><span class="sxs-lookup"><span data-stu-id="8d924-140">String</span></span>|<span data-ttu-id="8d924-141">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8d924-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="8d924-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="8d924-142">defaultLocale</span></span>|<span data-ttu-id="8d924-143">String</span><span class="sxs-lookup"><span data-stu-id="8d924-143">String</span></span>|<span data-ttu-id="8d924-144">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="8d924-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="8d924-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="8d924-145">brandingOptions</span></span>|[<span data-ttu-id="8d924-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="8d924-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="8d924-147">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="8d924-147">The Message Template Branding Options.</span></span> <span data-ttu-id="8d924-148">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="8d924-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="8d924-149">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`、`includeCompanyPortalLink`。</span><span class="sxs-lookup"><span data-stu-id="8d924-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="8d924-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d924-150">roleScopeTagIds</span></span>|<span data-ttu-id="8d924-151">String collection</span><span class="sxs-lookup"><span data-stu-id="8d924-151">String collection</span></span>|<span data-ttu-id="8d924-152">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8d924-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8d924-153">响应</span><span class="sxs-lookup"><span data-stu-id="8d924-153">Response</span></span>
<span data-ttu-id="8d924-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8d924-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d924-155">示例</span><span class="sxs-lookup"><span data-stu-id="8d924-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d924-156">请求</span><span class="sxs-lookup"><span data-stu-id="8d924-156">Request</span></span>
<span data-ttu-id="8d924-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d924-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
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

### <a name="response"></a><span data-ttu-id="8d924-158">响应</span><span class="sxs-lookup"><span data-stu-id="8d924-158">Response</span></span>
<span data-ttu-id="8d924-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d924-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




