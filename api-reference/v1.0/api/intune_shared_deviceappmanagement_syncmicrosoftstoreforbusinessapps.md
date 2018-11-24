# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="0423a-101">syncMicrosoftStoreForBusinessApps 操作</span><span class="sxs-lookup"><span data-stu-id="0423a-101">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="0423a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0423a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0423a-103">将 Intune 帐户与适用于企业的 Microsoft Store 同步</span><span class="sxs-lookup"><span data-stu-id="0423a-103">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0423a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0423a-104">Prerequisites</span></span>
<span data-ttu-id="0423a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="0423a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0423a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0423a-107">Permission type</span></span>|<span data-ttu-id="0423a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0423a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0423a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0423a-109">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="0423a-110">&nbsp;&nbsp; _入职培训_</span><span class="sxs-lookup"><span data-stu-id="0423a-110">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="0423a-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0423a-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0423a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0423a-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0423a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0423a-113">Not supported.</span></span>|
|<span data-ttu-id="0423a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0423a-114">Application</span></span>|<span data-ttu-id="0423a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0423a-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0423a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0423a-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="0423a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0423a-117">Request headers</span></span>
|<span data-ttu-id="0423a-118">标头</span><span class="sxs-lookup"><span data-stu-id="0423a-118">Header</span></span>|<span data-ttu-id="0423a-119">值</span><span class="sxs-lookup"><span data-stu-id="0423a-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0423a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0423a-120">Authorization</span></span>|<span data-ttu-id="0423a-121">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0423a-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0423a-122">Accept</span><span class="sxs-lookup"><span data-stu-id="0423a-122">Accept</span></span>|<span data-ttu-id="0423a-123">application/json</span><span class="sxs-lookup"><span data-stu-id="0423a-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0423a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0423a-124">Request body</span></span>
<span data-ttu-id="0423a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0423a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0423a-126">响应</span><span class="sxs-lookup"><span data-stu-id="0423a-126">Response</span></span>
<span data-ttu-id="0423a-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0423a-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="0423a-128">示例请求</span><span class="sxs-lookup"><span data-stu-id="0423a-128">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="0423a-129">响应</span><span class="sxs-lookup"><span data-stu-id="0423a-129">Response</span></span>

<span data-ttu-id="0423a-130">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="0423a-130">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0423a-131">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0423a-131">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



