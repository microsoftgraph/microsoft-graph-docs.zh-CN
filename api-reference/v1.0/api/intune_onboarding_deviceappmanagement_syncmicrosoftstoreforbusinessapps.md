# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="45e77-101">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="45e77-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="45e77-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45e77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45e77-103">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="45e77-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45e77-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="45e77-104">Prerequisites</span></span>
<span data-ttu-id="45e77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="45e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45e77-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="45e77-107">Permission type</span></span>|<span data-ttu-id="45e77-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45e77-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45e77-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45e77-109">Delegated (work or school account)</span></span>|<span data-ttu-id="45e77-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45e77-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45e77-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45e77-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45e77-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="45e77-112">Not supported.</span></span>|
|<span data-ttu-id="45e77-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="45e77-113">Application</span></span>|<span data-ttu-id="45e77-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45e77-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45e77-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45e77-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="45e77-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="45e77-116">Request headers</span></span>
|<span data-ttu-id="45e77-117">标头</span><span class="sxs-lookup"><span data-stu-id="45e77-117">Header</span></span>|<span data-ttu-id="45e77-118">值</span><span class="sxs-lookup"><span data-stu-id="45e77-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45e77-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="45e77-119">Authorization</span></span>|<span data-ttu-id="45e77-120">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="45e77-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="45e77-121">Accept</span><span class="sxs-lookup"><span data-stu-id="45e77-121">Accept</span></span>|<span data-ttu-id="45e77-122">application/json</span><span class="sxs-lookup"><span data-stu-id="45e77-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45e77-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="45e77-123">Request body</span></span>
<span data-ttu-id="45e77-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45e77-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45e77-125">响应</span><span class="sxs-lookup"><span data-stu-id="45e77-125">Response</span></span>
<span data-ttu-id="45e77-126">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="45e77-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45e77-127">示例</span><span class="sxs-lookup"><span data-stu-id="45e77-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="45e77-128">请求</span><span class="sxs-lookup"><span data-stu-id="45e77-128">Request</span></span>
<span data-ttu-id="45e77-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45e77-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="45e77-130">响应</span><span class="sxs-lookup"><span data-stu-id="45e77-130">Response</span></span>
<span data-ttu-id="45e77-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45e77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



