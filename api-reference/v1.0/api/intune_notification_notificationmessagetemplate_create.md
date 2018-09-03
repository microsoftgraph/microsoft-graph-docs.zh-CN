# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="e0ba4-101">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="e0ba4-101">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="e0ba4-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0ba4-103">创建新的 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-103">Create a new [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0ba4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0ba4-104">Prerequisites</span></span>
<span data-ttu-id="e0ba4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0ba4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0ba4-107">Permission type</span></span>|<span data-ttu-id="e0ba4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0ba4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0ba4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ba4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e0ba4-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ba4-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e0ba4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0ba4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0ba4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-112">Not supported.</span></span>|
|<span data-ttu-id="e0ba4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0ba4-113">Application</span></span>|<span data-ttu-id="e0ba4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0ba4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0ba4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="e0ba4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0ba4-116">Request headers</span></span>
|<span data-ttu-id="e0ba4-117">标头</span><span class="sxs-lookup"><span data-stu-id="e0ba4-117">Header</span></span>|<span data-ttu-id="e0ba4-118">值</span><span class="sxs-lookup"><span data-stu-id="e0ba4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0ba4-119">授权</span><span class="sxs-lookup"><span data-stu-id="e0ba4-119">Authorization</span></span>|<span data-ttu-id="e0ba4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0ba4-121">接受</span><span class="sxs-lookup"><span data-stu-id="e0ba4-121">Accept</span></span>|<span data-ttu-id="e0ba4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e0ba4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0ba4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0ba4-123">Request body</span></span>
<span data-ttu-id="e0ba4-124">在请求正文中，提供 notificationMessageTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-124">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="e0ba4-125">下表显示创建 notificationMessageTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-125">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="e0ba4-126">属性</span><span class="sxs-lookup"><span data-stu-id="e0ba4-126">Property</span></span>|<span data-ttu-id="e0ba4-127">类型</span><span class="sxs-lookup"><span data-stu-id="e0ba4-127">Type</span></span>|<span data-ttu-id="e0ba4-128">说明</span><span class="sxs-lookup"><span data-stu-id="e0ba4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0ba4-129">ID</span><span class="sxs-lookup"><span data-stu-id="e0ba4-129">id</span></span>|<span data-ttu-id="e0ba4-130">字符串</span><span class="sxs-lookup"><span data-stu-id="e0ba4-130">String</span></span>|<span data-ttu-id="e0ba4-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-131">Key of the entity.</span></span>|
|<span data-ttu-id="e0ba4-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0ba4-132">lastModifiedDateTime</span></span>|<span data-ttu-id="e0ba4-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0ba4-133">DateTimeOffset</span></span>|<span data-ttu-id="e0ba4-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e0ba4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e0ba4-135">displayName</span></span>|<span data-ttu-id="e0ba4-136">字符串</span><span class="sxs-lookup"><span data-stu-id="e0ba4-136">String</span></span>|<span data-ttu-id="e0ba4-137">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="e0ba4-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="e0ba4-138">defaultLocale</span></span>|<span data-ttu-id="e0ba4-139">字符串</span><span class="sxs-lookup"><span data-stu-id="e0ba4-139">String</span></span>|<span data-ttu-id="e0ba4-140">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="e0ba4-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="e0ba4-141">brandingOptions</span></span>|[<span data-ttu-id="e0ba4-142">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="e0ba4-142">notificationTemplateBrandingOptions</span></span>](../resources/intune_notification_notificationtemplatebrandingoptions.md)|<span data-ttu-id="e0ba4-143">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-143">The Message Template Branding Options.</span></span> <span data-ttu-id="e0ba4-144">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-144">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="e0ba4-145">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-145">The possible values are `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="e0ba4-146">响应</span><span class="sxs-lookup"><span data-stu-id="e0ba4-146">Response</span></span>
<span data-ttu-id="e0ba4-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-147">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ba4-148">示例</span><span class="sxs-lookup"><span data-stu-id="e0ba4-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0ba4-149">请求</span><span class="sxs-lookup"><span data-stu-id="e0ba4-149">Request</span></span>
<span data-ttu-id="e0ba4-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="e0ba4-151">响应</span><span class="sxs-lookup"><span data-stu-id="e0ba4-151">Response</span></span>
<span data-ttu-id="e0ba4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0ba4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



