# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="f5511-101">更新 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="f5511-101">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="f5511-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5511-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5511-103">更新 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f5511-103">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5511-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5511-104">Prerequisites</span></span>
<span data-ttu-id="f5511-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f5511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5511-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5511-107">Permission type</span></span>|<span data-ttu-id="f5511-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5511-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5511-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5511-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f5511-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5511-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f5511-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5511-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5511-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5511-112">Not supported.</span></span>|
|<span data-ttu-id="f5511-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5511-113">Application</span></span>|<span data-ttu-id="f5511-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5511-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5511-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5511-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="f5511-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5511-116">Request headers</span></span>
|<span data-ttu-id="f5511-117">标头</span><span class="sxs-lookup"><span data-stu-id="f5511-117">Header</span></span>|<span data-ttu-id="f5511-118">值</span><span class="sxs-lookup"><span data-stu-id="f5511-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5511-119">授权</span><span class="sxs-lookup"><span data-stu-id="f5511-119">Authorization</span></span>|<span data-ttu-id="f5511-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5511-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5511-121">接受</span><span class="sxs-lookup"><span data-stu-id="f5511-121">Accept</span></span>|<span data-ttu-id="f5511-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f5511-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5511-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5511-123">Request body</span></span>
<span data-ttu-id="f5511-124">在请求正文中，提供 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5511-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="f5511-125">下表显示创建 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5511-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="f5511-126">属性</span><span class="sxs-lookup"><span data-stu-id="f5511-126">Property</span></span>|<span data-ttu-id="f5511-127">类型</span><span class="sxs-lookup"><span data-stu-id="f5511-127">Type</span></span>|<span data-ttu-id="f5511-128">说明</span><span class="sxs-lookup"><span data-stu-id="f5511-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5511-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f5511-129">displayName</span></span>|<span data-ttu-id="f5511-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f5511-130">String</span></span>|<span data-ttu-id="f5511-131">友好名称</span><span class="sxs-lookup"><span data-stu-id="f5511-131">The friendly name</span></span>|
|<span data-ttu-id="f5511-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="f5511-132">fileHash</span></span>|<span data-ttu-id="f5511-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f5511-133">String</span></span>|<span data-ttu-id="f5511-134">文件的 SHA256 哈希</span><span class="sxs-lookup"><span data-stu-id="f5511-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="f5511-135">file</span><span class="sxs-lookup"><span data-stu-id="f5511-135">file</span></span>|<span data-ttu-id="f5511-136">二进制</span><span class="sxs-lookup"><span data-stu-id="f5511-136">Binary</span></span>|<span data-ttu-id="f5511-137">字节数组形式的文件</span><span class="sxs-lookup"><span data-stu-id="f5511-137">File as a byte array</span></span>|
|<span data-ttu-id="f5511-138">ID</span><span class="sxs-lookup"><span data-stu-id="f5511-138">id</span></span>|<span data-ttu-id="f5511-139">字符串</span><span class="sxs-lookup"><span data-stu-id="f5511-139">String</span></span>|<span data-ttu-id="f5511-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5511-140">Key of the entity.</span></span>|
|<span data-ttu-id="f5511-141">version</span><span class="sxs-lookup"><span data-stu-id="f5511-141">version</span></span>|<span data-ttu-id="f5511-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f5511-142">String</span></span>|<span data-ttu-id="f5511-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="f5511-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f5511-144">响应</span><span class="sxs-lookup"><span data-stu-id="f5511-144">Response</span></span>
<span data-ttu-id="f5511-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5511-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5511-146">示例</span><span class="sxs-lookup"><span data-stu-id="f5511-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5511-147">请求</span><span class="sxs-lookup"><span data-stu-id="f5511-147">Request</span></span>
<span data-ttu-id="f5511-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5511-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 131

{
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="f5511-149">响应</span><span class="sxs-lookup"><span data-stu-id="f5511-149">Response</span></span>
<span data-ttu-id="f5511-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5511-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








