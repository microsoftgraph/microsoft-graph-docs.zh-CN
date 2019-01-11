---
title: 使用 OneNote REST API
description: 'Microsoft Graph 允许您获取授权的访问用户的 OneNote 笔记本、 节和页面中的个人或组织帐户的应用程序。 使用适当委派或应用程序权限，您的应用程序可以访问已登录的用户或租户中的任何用户的 OneNote 数据。 '
localization_priority: Normal
ms.openlocfilehash: 25817280fff570f0d87722fc8f3fadc9cf1c24d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815233"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="c825a-104">使用 OneNote REST API</span><span class="sxs-lookup"><span data-stu-id="c825a-104">Use the OneNote REST API</span></span>

> <span data-ttu-id="c825a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c825a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c825a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c825a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c825a-107">Microsoft Graph 允许您获取授权的访问用户的 OneNote 笔记本、 节和页面中的个人或组织帐户的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c825a-107">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="c825a-108">使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions)，您的应用程序可以访问已登录的用户或租户中的任何用户的 OneNote 数据。</span><span class="sxs-lookup"><span data-stu-id="c825a-108">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="c825a-109">根 URL</span><span class="sxs-lookup"><span data-stu-id="c825a-109">Root URL</span></span>
<span data-ttu-id="c825a-110">OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。</span><span class="sxs-lookup"><span data-stu-id="c825a-110">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="c825a-111">`version` URL 中的段代表您想要使用的 Microsoft Graph 的版本：</span><span class="sxs-lookup"><span data-stu-id="c825a-111">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="c825a-112">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="c825a-112">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="c825a-113">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="c825a-113">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="c825a-114">功能和 beta 终结点中的功能可能会更改;我们建议不要在生产代码中使用它。</span><span class="sxs-lookup"><span data-stu-id="c825a-114">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="c825a-115">位置可以是在 Office 365 或使用者 OneDrive 用户笔记本、 组笔记本或在 Office 365 上的 SharePoint 网站承载团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="c825a-115">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="c825a-117">用户笔记本</span><span class="sxs-lookup"><span data-stu-id="c825a-117">User notebooks</span></span>
<span data-ttu-id="c825a-118">若要访问 OneDrive 或 OneDrive for Business 的使用者上的个人笔记本，请使用以下 Url 之一：</span><span class="sxs-lookup"><span data-stu-id="c825a-118">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="c825a-119">`me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。</span><span class="sxs-lookup"><span data-stu-id="c825a-119">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="c825a-120">`users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。</span><span class="sxs-lookup"><span data-stu-id="c825a-120">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c825a-121">使用[用户](users.md)API。</span><span class="sxs-lookup"><span data-stu-id="c825a-121">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="c825a-122">**注意：** 您可以通过 GET 请求上获取用户 Id `https://graph.microsoft.com/v1.0/users`。</span><span class="sxs-lookup"><span data-stu-id="c825a-122">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="c825a-123">组笔记本</span><span class="sxs-lookup"><span data-stu-id="c825a-123">Group notebooks</span></span>

<span data-ttu-id="c825a-124">若要访问一组由拥有的笔记本，请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="c825a-124">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="c825a-125">SharePoint 网站笔记本</span><span class="sxs-lookup"><span data-stu-id="c825a-125">SharePoint site notebooks</span></span>
<span data-ttu-id="c825a-126">若要访问笔记本所拥有的 SharePoint 工作组网站，请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="c825a-126">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
