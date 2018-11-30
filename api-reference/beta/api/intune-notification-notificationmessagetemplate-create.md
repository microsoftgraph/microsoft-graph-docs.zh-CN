---
title: 创建 notificationMessageTemplate
description: 创建新的 notificationMessageTemplate 对象。
ms.openlocfilehash: 013acd831979fdbb22eb67be66552b2d21d590b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049526"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="1a662-103">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="1a662-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="1a662-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a662-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a662-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a662-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a662-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a662-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a662-107">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a662-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a662-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a662-108">Prerequisites</span></span>
<span data-ttu-id="1a662-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1a662-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a662-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a662-111">Permission type</span></span>|<span data-ttu-id="1a662-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a662-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a662-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a662-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a662-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a662-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a662-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a662-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a662-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a662-116">Not supported.</span></span>|
|<span data-ttu-id="1a662-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a662-117">Application</span></span>|<span data-ttu-id="1a662-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a662-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a662-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a662-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="1a662-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a662-120">Request headers</span></span>
|<span data-ttu-id="1a662-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a662-121">Header</span></span>|<span data-ttu-id="1a662-122">值</span><span class="sxs-lookup"><span data-stu-id="1a662-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a662-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a662-123">Authorization</span></span>|<span data-ttu-id="1a662-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a662-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a662-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a662-125">Accept</span></span>|<span data-ttu-id="1a662-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a662-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a662-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a662-127">Request body</span></span>
<span data-ttu-id="1a662-128">在请求正文中，提供 notificationMessageTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a662-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="1a662-129">下表显示创建 notificationMessageTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a662-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="1a662-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a662-130">Property</span></span>|<span data-ttu-id="1a662-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a662-131">Type</span></span>|<span data-ttu-id="1a662-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a662-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a662-133">id</span><span class="sxs-lookup"><span data-stu-id="1a662-133">id</span></span>|<span data-ttu-id="1a662-134">String</span><span class="sxs-lookup"><span data-stu-id="1a662-134">String</span></span>|<span data-ttu-id="1a662-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a662-135">Key of the entity.</span></span>|
|<span data-ttu-id="1a662-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a662-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1a662-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a662-137">DateTimeOffset</span></span>|<span data-ttu-id="1a662-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a662-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1a662-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1a662-139">displayName</span></span>|<span data-ttu-id="1a662-140">String</span><span class="sxs-lookup"><span data-stu-id="1a662-140">String</span></span>|<span data-ttu-id="1a662-141">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1a662-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="1a662-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="1a662-142">defaultLocale</span></span>|<span data-ttu-id="1a662-143">String</span><span class="sxs-lookup"><span data-stu-id="1a662-143">String</span></span>|<span data-ttu-id="1a662-144">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="1a662-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="1a662-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="1a662-145">brandingOptions</span></span>|[<span data-ttu-id="1a662-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="1a662-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="1a662-147">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="1a662-147">The Message Template Branding Options.</span></span> <span data-ttu-id="1a662-148">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="1a662-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="1a662-149">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="1a662-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="1a662-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a662-150">roleScopeTagIds</span></span>|<span data-ttu-id="1a662-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a662-151">String collection</span></span>|<span data-ttu-id="1a662-152">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1a662-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1a662-153">响应</span><span class="sxs-lookup"><span data-stu-id="1a662-153">Response</span></span>
<span data-ttu-id="1a662-154">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a662-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a662-155">示例</span><span class="sxs-lookup"><span data-stu-id="1a662-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a662-156">请求</span><span class="sxs-lookup"><span data-stu-id="1a662-156">Request</span></span>
<span data-ttu-id="1a662-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a662-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1a662-158">响应</span><span class="sxs-lookup"><span data-stu-id="1a662-158">Response</span></span>
<span data-ttu-id="1a662-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a662-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





