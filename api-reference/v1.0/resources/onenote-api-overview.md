# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="4b64e-101">使用 OneNote REST API</span><span class="sxs-lookup"><span data-stu-id="4b64e-101">Use the OneNote REST API</span></span>

<span data-ttu-id="4b64e-102">Microsoft Graph 允许您的应用获取对用户的个人或组织帐户中的 OneNote 笔记本、节和页面的授权访问权限。</span><span class="sxs-lookup"><span data-stu-id="4b64e-102">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="4b64e-103">使用[适当的委派或应用程序权限](../../../concepts/permissions_reference.md#notes-permissions)，您的应用可以访问已登录用户或租户中的任何用户的 OneNote 数据。</span><span class="sxs-lookup"><span data-stu-id="4b64e-103">With the [appropriate delegated or application permissions](../../../concepts/permissions_reference.md#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span>

## <a name="root-url"></a><span data-ttu-id="4b64e-104">根 URL</span><span class="sxs-lookup"><span data-stu-id="4b64e-104">Root URL</span></span>
<span data-ttu-id="4b64e-105">OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。</span><span class="sxs-lookup"><span data-stu-id="4b64e-105">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
<span data-ttu-id="4b64e-106">URL 中的 `version` 段代表您希望使用的 Microsoft Graph 版本。</span><span class="sxs-lookup"><span data-stu-id="4b64e-106">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>

- <span data-ttu-id="4b64e-107">`v1.0` 用于稳定生产代码。</span><span class="sxs-lookup"><span data-stu-id="4b64e-107">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="4b64e-108">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="4b64e-108">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="4b64e-109">beta 端点中的功能可能会出现变动；我们不建议在生产代码中使用它。</span><span class="sxs-lookup"><span data-stu-id="4b64e-109">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="4b64e-110">位置可以是 Office 365 或消费者 OneDrive、团队笔记本 上的用户笔记本，也可以是 Office 365 上的 SharePoint 站点托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="4b64e-110">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="4b64e-112">用户笔记本</span><span class="sxs-lookup"><span data-stu-id="4b64e-112">User notebooks</span></span>
<span data-ttu-id="4b64e-113">要访问消费者 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="4b64e-113">User notebooks To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="4b64e-114">`me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。</span><span class="sxs-lookup"><span data-stu-id="4b64e-114">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="4b64e-115">`users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。</span><span class="sxs-lookup"><span data-stu-id="4b64e-115">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="4b64e-116">使用[用户](users.md) API。</span><span class="sxs-lookup"><span data-stu-id="4b64e-116">[Use the Planner API](users.md)</span></span>
> <span data-ttu-id="4b64e-117">**注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。</span><span class="sxs-lookup"><span data-stu-id="4b64e-117">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="4b64e-118">团队笔记本</span><span class="sxs-lookup"><span data-stu-id="4b64e-118">Group notebooks</span></span>
<span data-ttu-id="4b64e-119">要访问团队拥有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="4b64e-119">Group notebooks To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="4b64e-120">SharePoint 网站笔记本</span><span class="sxs-lookup"><span data-stu-id="4b64e-120">SharePoint site notebooks</span></span>

<span data-ttu-id="4b64e-121">要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="4b64e-121">SharePoint site notebooks To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

