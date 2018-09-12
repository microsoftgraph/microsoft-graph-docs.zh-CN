# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c5d6a-101">创建 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c5d6a-101">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="c5d6a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5d6a-103">创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-103">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5d6a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5d6a-104">Prerequisites</span></span>
<span data-ttu-id="c5d6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5d6a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5d6a-107">Permission type</span></span>|<span data-ttu-id="c5d6a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5d6a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5d6a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d6a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c5d6a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d6a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5d6a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d6a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5d6a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-112">Not supported.</span></span>|
|<span data-ttu-id="c5d6a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5d6a-113">Application</span></span>|<span data-ttu-id="c5d6a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5d6a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5d6a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="c5d6a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5d6a-116">Request headers</span></span>
|<span data-ttu-id="c5d6a-117">标头</span><span class="sxs-lookup"><span data-stu-id="c5d6a-117">Header</span></span>|<span data-ttu-id="c5d6a-118">值</span><span class="sxs-lookup"><span data-stu-id="c5d6a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5d6a-119">授权</span><span class="sxs-lookup"><span data-stu-id="c5d6a-119">Authorization</span></span>|<span data-ttu-id="c5d6a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5d6a-121">接受</span><span class="sxs-lookup"><span data-stu-id="c5d6a-121">Accept</span></span>|<span data-ttu-id="c5d6a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d6a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d6a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5d6a-123">Request body</span></span>
<span data-ttu-id="c5d6a-124">在请求正文中，提供 windowsInformationProtectionAppLockerFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-124">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="c5d6a-125">下表显示创建 windowsInformationProtectionAppLockerFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-125">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="c5d6a-126">属性</span><span class="sxs-lookup"><span data-stu-id="c5d6a-126">Property</span></span>|<span data-ttu-id="c5d6a-127">类型</span><span class="sxs-lookup"><span data-stu-id="c5d6a-127">Type</span></span>|<span data-ttu-id="c5d6a-128">说明</span><span class="sxs-lookup"><span data-stu-id="c5d6a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d6a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d6a-129">displayName</span></span>|<span data-ttu-id="c5d6a-130">字符串</span><span class="sxs-lookup"><span data-stu-id="c5d6a-130">String</span></span>|<span data-ttu-id="c5d6a-131">友好名称</span><span class="sxs-lookup"><span data-stu-id="c5d6a-131">The friendly name</span></span>|
|<span data-ttu-id="c5d6a-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="c5d6a-132">fileHash</span></span>|<span data-ttu-id="c5d6a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c5d6a-133">String</span></span>|<span data-ttu-id="c5d6a-134">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="c5d6a-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="c5d6a-135">file</span><span class="sxs-lookup"><span data-stu-id="c5d6a-135">file</span></span>|<span data-ttu-id="c5d6a-136">二进制</span><span class="sxs-lookup"><span data-stu-id="c5d6a-136">Binary</span></span>|<span data-ttu-id="c5d6a-137">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="c5d6a-137">File as a byte array</span></span>|
|<span data-ttu-id="c5d6a-138">id</span><span class="sxs-lookup"><span data-stu-id="c5d6a-138">id</span></span>|<span data-ttu-id="c5d6a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c5d6a-139">String</span></span>|<span data-ttu-id="c5d6a-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-140">Key of the entity.</span></span>|
|<span data-ttu-id="c5d6a-141">version</span><span class="sxs-lookup"><span data-stu-id="c5d6a-141">version</span></span>|<span data-ttu-id="c5d6a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="c5d6a-142">String</span></span>|<span data-ttu-id="c5d6a-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c5d6a-144">响应</span><span class="sxs-lookup"><span data-stu-id="c5d6a-144">Response</span></span>
<span data-ttu-id="c5d6a-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d6a-146">示例</span><span class="sxs-lookup"><span data-stu-id="c5d6a-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5d6a-147">请求</span><span class="sxs-lookup"><span data-stu-id="c5d6a-147">Request</span></span>
<span data-ttu-id="c5d6a-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="c5d6a-149">响应</span><span class="sxs-lookup"><span data-stu-id="c5d6a-149">Response</span></span>
<span data-ttu-id="c5d6a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5d6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```








