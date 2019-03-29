---
title: 创建 notificationMessageTemplate
description: 创建新的 notificationMessageTemplate 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22bca3bfef9de68875337fe23a1f40c63babe2c4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964449"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="56305-103">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="56305-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="56305-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56305-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56305-105">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56305-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56305-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="56305-106">Prerequisites</span></span>
<span data-ttu-id="56305-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56305-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56305-109">Permission type</span></span>|<span data-ttu-id="56305-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56305-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56305-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56305-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56305-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56305-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="56305-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56305-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56305-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56305-114">Not supported.</span></span>|
|<span data-ttu-id="56305-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56305-115">Application</span></span>|<span data-ttu-id="56305-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56305-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56305-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56305-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="56305-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="56305-118">Request headers</span></span>
|<span data-ttu-id="56305-119">标头</span><span class="sxs-lookup"><span data-stu-id="56305-119">Header</span></span>|<span data-ttu-id="56305-120">值</span><span class="sxs-lookup"><span data-stu-id="56305-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56305-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56305-121">Authorization</span></span>|<span data-ttu-id="56305-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56305-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56305-123">接受</span><span class="sxs-lookup"><span data-stu-id="56305-123">Accept</span></span>|<span data-ttu-id="56305-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56305-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56305-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="56305-125">Request body</span></span>
<span data-ttu-id="56305-126">在请求正文中，提供 notificationMessageTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56305-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="56305-127">下表显示创建 notificationMessageTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="56305-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="56305-128">属性</span><span class="sxs-lookup"><span data-stu-id="56305-128">Property</span></span>|<span data-ttu-id="56305-129">类型</span><span class="sxs-lookup"><span data-stu-id="56305-129">Type</span></span>|<span data-ttu-id="56305-130">说明</span><span class="sxs-lookup"><span data-stu-id="56305-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56305-131">id</span><span class="sxs-lookup"><span data-stu-id="56305-131">id</span></span>|<span data-ttu-id="56305-132">String</span><span class="sxs-lookup"><span data-stu-id="56305-132">String</span></span>|<span data-ttu-id="56305-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56305-133">Key of the entity.</span></span>|
|<span data-ttu-id="56305-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56305-134">lastModifiedDateTime</span></span>|<span data-ttu-id="56305-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56305-135">DateTimeOffset</span></span>|<span data-ttu-id="56305-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56305-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="56305-137">displayName</span><span class="sxs-lookup"><span data-stu-id="56305-137">displayName</span></span>|<span data-ttu-id="56305-138">字符串</span><span class="sxs-lookup"><span data-stu-id="56305-138">String</span></span>|<span data-ttu-id="56305-139">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="56305-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="56305-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="56305-140">defaultLocale</span></span>|<span data-ttu-id="56305-141">String</span><span class="sxs-lookup"><span data-stu-id="56305-141">String</span></span>|<span data-ttu-id="56305-142">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="56305-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="56305-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="56305-143">brandingOptions</span></span>|[<span data-ttu-id="56305-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="56305-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="56305-145">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="56305-145">The Message Template Branding Options.</span></span> <span data-ttu-id="56305-146">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="56305-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="56305-147">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="56305-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="56305-148">响应</span><span class="sxs-lookup"><span data-stu-id="56305-148">Response</span></span>
<span data-ttu-id="56305-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56305-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56305-150">示例</span><span class="sxs-lookup"><span data-stu-id="56305-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="56305-151">请求</span><span class="sxs-lookup"><span data-stu-id="56305-151">Request</span></span>
<span data-ttu-id="56305-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56305-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56305-153">响应</span><span class="sxs-lookup"><span data-stu-id="56305-153">Response</span></span>
<span data-ttu-id="56305-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56305-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



