---
title: 使用 OneNote REST API
description: 'Microsoft Graph 允许你的应用获取对个人或组织帐户中的用户 OneNote 笔记本、节和页面的授权访问权限。 使用适当的委派或应用程序权限, 您的应用程序可以访问已登录用户的 OneNote 数据或租户中的任何用户。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566043"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="b5172-104">使用 OneNote REST API</span><span class="sxs-lookup"><span data-stu-id="b5172-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5172-105">Microsoft Graph 允许你的应用获取对个人或组织帐户中的用户 OneNote 笔记本、节和页面的授权访问权限。</span><span class="sxs-lookup"><span data-stu-id="b5172-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="b5172-106">使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions), 您的应用程序可以访问已登录用户的 OneNote 数据或租户中的任何用户。</span><span class="sxs-lookup"><span data-stu-id="b5172-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="b5172-107">根 URL</span><span class="sxs-lookup"><span data-stu-id="b5172-107">Root URL</span></span>
<span data-ttu-id="b5172-108">onenote 服务根 URL 对 onenote API 的所有调用使用以下格式。</span><span class="sxs-lookup"><span data-stu-id="b5172-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="b5172-109">URL `version`中的段表示要使用的 Microsoft Graph 的版本:</span><span class="sxs-lookup"><span data-stu-id="b5172-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="b5172-110">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="b5172-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="b5172-111">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="b5172-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="b5172-112">beta 终结点中的特性和功能可能会发生变化;我们建议您不要在生产代码中使用它。</span><span class="sxs-lookup"><span data-stu-id="b5172-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="b5172-113">该位置可以是 office 365 上的用户笔记本, 也可以是 office 365 上的使用者 OneDrive、组笔记本或 SharePoint 网站托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="b5172-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="b5172-115">用户笔记本</span><span class="sxs-lookup"><span data-stu-id="b5172-115">User notebooks</span></span>
<span data-ttu-id="b5172-116">若要访问消费者 OneDrive 或 OneDrive for business 上的个人笔记本, 请使用下列 url 之一:</span><span class="sxs-lookup"><span data-stu-id="b5172-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="b5172-117">`me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。</span><span class="sxs-lookup"><span data-stu-id="b5172-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="b5172-118">`users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。</span><span class="sxs-lookup"><span data-stu-id="b5172-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="b5172-119">使用[用户](users.md)API。</span><span class="sxs-lookup"><span data-stu-id="b5172-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="b5172-120">**注意:** 您可以通过发出 get 请求来获取用户 id `https://graph.microsoft.com/v1.0/users`。</span><span class="sxs-lookup"><span data-stu-id="b5172-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="b5172-121">组笔记本</span><span class="sxs-lookup"><span data-stu-id="b5172-121">Group notebooks</span></span>

<span data-ttu-id="b5172-122">若要访问组拥有的笔记本, 请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="b5172-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="b5172-123">SharePoint 网站笔记本</span><span class="sxs-lookup"><span data-stu-id="b5172-123">SharePoint site notebooks</span></span>
<span data-ttu-id="b5172-124">若要访问 SharePoint 团队网站拥有的笔记本, 请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="b5172-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
