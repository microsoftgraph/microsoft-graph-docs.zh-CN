# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="f8652-101">创建 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="f8652-101">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="f8652-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f8652-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8652-103">创建新的 [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8652-103">Create a new [plannerBucket](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8652-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8652-104">Prerequisites</span></span>
<span data-ttu-id="f8652-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f8652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8652-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8652-107">Permission type</span></span>|<span data-ttu-id="f8652-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8652-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8652-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8652-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f8652-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8652-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8652-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8652-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8652-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8652-112">Not supported.</span></span>|
|<span data-ttu-id="f8652-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8652-113">Application</span></span>|<span data-ttu-id="f8652-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8652-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8652-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8652-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="f8652-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8652-116">Request headers</span></span>
|<span data-ttu-id="f8652-117">标头</span><span class="sxs-lookup"><span data-stu-id="f8652-117">Header</span></span>|<span data-ttu-id="f8652-118">值</span><span class="sxs-lookup"><span data-stu-id="f8652-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8652-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8652-119">Authorization</span></span>|<span data-ttu-id="f8652-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8652-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f8652-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f8652-121">Accept</span></span>|<span data-ttu-id="f8652-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f8652-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8652-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8652-123">Request body</span></span>
<span data-ttu-id="f8652-124">在请求正文中，提供 androidForWorkAppConfigurationSchema 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8652-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="f8652-125">下表显示创建 androidForWorkAppConfigurationSchema 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8652-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="f8652-126">属性</span><span class="sxs-lookup"><span data-stu-id="f8652-126">Property</span></span>|<span data-ttu-id="f8652-127">类型</span><span class="sxs-lookup"><span data-stu-id="f8652-127">Type</span></span>|<span data-ttu-id="f8652-128">说明</span><span class="sxs-lookup"><span data-stu-id="f8652-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8652-129">id</span><span class="sxs-lookup"><span data-stu-id="f8652-129">id</span></span>|<span data-ttu-id="f8652-130">String</span><span class="sxs-lookup"><span data-stu-id="f8652-130">String</span></span>|<span data-ttu-id="f8652-131">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="f8652-131">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="f8652-132">exampleJson</span><span class="sxs-lookup"><span data-stu-id="f8652-132">exampleJson</span></span>|<span data-ttu-id="f8652-133">Binary</span><span class="sxs-lookup"><span data-stu-id="f8652-133">Binary</span></span>|<span data-ttu-id="f8652-134">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="f8652-134">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="f8652-135">schemaItems</span><span class="sxs-lookup"><span data-stu-id="f8652-135">schemaItems</span></span>|<span data-ttu-id="f8652-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8652-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="f8652-137">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="f8652-137">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="f8652-138">响应</span><span class="sxs-lookup"><span data-stu-id="f8652-138">Response</span></span>
<span data-ttu-id="f8652-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8652-139">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8652-140">示例</span><span class="sxs-lookup"><span data-stu-id="f8652-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8652-141">请求</span><span class="sxs-lookup"><span data-stu-id="f8652-141">Request</span></span>
<span data-ttu-id="f8652-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8652-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f8652-143">响应</span><span class="sxs-lookup"><span data-stu-id="f8652-143">Response</span></span>
<span data-ttu-id="f8652-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8652-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



