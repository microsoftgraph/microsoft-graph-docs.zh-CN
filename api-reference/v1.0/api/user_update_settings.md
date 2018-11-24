# <a name="update-settings"></a><span data-ttu-id="5de85-101">更新设置</span><span class="sxs-lookup"><span data-stu-id="5de85-101">Update settings</span></span>

<span data-ttu-id="5de85-102">更新[设置](../resources/user_settings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5de85-102">Update the properties of the [settings](../resources/user_settings.md) object.</span></span> <span data-ttu-id="5de85-103">在同一组织的用户可以根据他们输入首选项或组织策略的不同设置。</span><span class="sxs-lookup"><span data-stu-id="5de85-103">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="5de85-104">若要获取用户当前设置，请参阅[当前用户设置](user_get_settings.md)。</span><span class="sxs-lookup"><span data-stu-id="5de85-104">To get the user current settings, see [current user settings](user_get_settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="5de85-105">权限</span><span class="sxs-lookup"><span data-stu-id="5de85-105">Permissions</span></span>

<span data-ttu-id="5de85-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5de85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5de85-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5de85-108">Permission type</span></span>      | <span data-ttu-id="5de85-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5de85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5de85-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5de85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5de85-111">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de85-111">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="5de85-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5de85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de85-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5de85-113">Not supported.</span></span>    |
|<span data-ttu-id="5de85-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5de85-114">Application</span></span> | <span data-ttu-id="5de85-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de85-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de85-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5de85-116">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

<span data-ttu-id="5de85-117">请求用户 id 或者 userPrincipalName 才可以访问由用户或由具有 User.ReadWrite.All 权限的用户。</span><span class="sxs-lookup"><span data-stu-id="5de85-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="5de85-118">若要了解详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5de85-118">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span> 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="5de85-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5de85-119">Request headers</span></span>

| <span data-ttu-id="5de85-120">标头</span><span class="sxs-lookup"><span data-stu-id="5de85-120">Header</span></span>       | <span data-ttu-id="5de85-121">值</span><span class="sxs-lookup"><span data-stu-id="5de85-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5de85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5de85-122">Authorization</span></span>  | <span data-ttu-id="5de85-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5de85-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5de85-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5de85-125">Content-Type</span></span>  | <span data-ttu-id="5de85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5de85-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5de85-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5de85-127">Request body</span></span>

<span data-ttu-id="5de85-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5de85-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5de85-131">属性</span><span class="sxs-lookup"><span data-stu-id="5de85-131">Property</span></span>     | <span data-ttu-id="5de85-132">类型</span><span class="sxs-lookup"><span data-stu-id="5de85-132">Type</span></span>   |<span data-ttu-id="5de85-133">说明</span><span class="sxs-lookup"><span data-stu-id="5de85-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5de85-134">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="5de85-134">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="5de85-135">布尔</span><span class="sxs-lookup"><span data-stu-id="5de85-135">Boolean</span></span>|<span data-ttu-id="5de85-136">设置为 true 禁用代理人访问的[趋势](../../beta/resources/insights_trending.md)API 或禁止用户访问 Office 深入中的文档。</span><span class="sxs-lookup"><span data-stu-id="5de85-136">Set to true do disable delegate access to the [Trending](../../beta/resources/insights_trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="5de85-137">设置为 true 还会影响的 Office 365 中显示的内容相关性-例如，建议 SharePoint 主页中的网站和中的 OneDrive for Business 的发现视图显示相关性较低的结果。</span><span class="sxs-lookup"><span data-stu-id="5de85-137">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="5de85-138">此设置反映在[Office 深入](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)的控件状态。</span><span class="sxs-lookup"><span data-stu-id="5de85-138">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="5de85-139">示例</span><span class="sxs-lookup"><span data-stu-id="5de85-139">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="5de85-140">请求</span><span class="sxs-lookup"><span data-stu-id="5de85-140">Request</span></span>

<span data-ttu-id="5de85-141">下面是一个示例请求如何选择退出 Delve 用户并禁用其上为整个组织的内容相关性的贡献。</span><span class="sxs-lookup"><span data-stu-id="5de85-141">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="5de85-142">响应</span><span class="sxs-lookup"><span data-stu-id="5de85-142">Response</span></span>

<span data-ttu-id="5de85-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5de85-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="5de85-146">批量请求</span><span class="sxs-lookup"><span data-stu-id="5de85-146">Batch request</span></span>

<span data-ttu-id="5de85-147">还有可能退出 Delve 从多个用户并禁用上为整个组织通过批处理请求的内容相关性做出贡献。</span><span class="sxs-lookup"><span data-stu-id="5de85-147">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="5de85-148">若要了解详细信息，请参阅[JSON 批处理](https://developer.microsoft.com/graph/docs/concepts/json_batching)。</span><span class="sxs-lookup"><span data-stu-id="5de85-148">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="5de85-149">**重要说明**： 仅[Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US)角色组的成员可以更新多个用户。</span><span class="sxs-lookup"><span data-stu-id="5de85-149">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



