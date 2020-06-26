---
title: 使用 OneNote REST API
description: 'Microsoft Graph 可让应用程序获得对个人或组织帐户中用户的 OneNote 笔记本、节和页面的授权访问权限。 使用适当的委派或应用程序权限，你的应用程序可以访问已登录用户或租户中任何用户的 OneNote 数据。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 07b8fdf5486eee041a40b7bc6dd3169ac1af8761
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896838"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="a172d-104">使用 OneNote REST API</span><span class="sxs-lookup"><span data-stu-id="a172d-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a172d-105">Microsoft Graph 可让应用程序获得对个人或组织帐户中用户的 OneNote 笔记本、节和页面的授权访问权限。</span><span class="sxs-lookup"><span data-stu-id="a172d-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="a172d-106">使用[适当的委派或应用程序权限](/graph/permissions-reference#notes-permissions)，你的应用程序可以访问已登录用户或租户中任何用户的 OneNote 数据。</span><span class="sxs-lookup"><span data-stu-id="a172d-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="a172d-107">根 URL</span><span class="sxs-lookup"><span data-stu-id="a172d-107">Root URL</span></span>
<span data-ttu-id="a172d-108">OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。</span><span class="sxs-lookup"><span data-stu-id="a172d-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="a172d-109">URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本：</span><span class="sxs-lookup"><span data-stu-id="a172d-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="a172d-110">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="a172d-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="a172d-111">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="a172d-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="a172d-112">Beta 终结点中的特性和功能可能改变；不推荐将其用于生产代码中。</span><span class="sxs-lookup"><span data-stu-id="a172d-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="a172d-113">Microsoft 365 上的位置可以是 Microsoft 365 或消费者 OneDrive、组笔记本或 SharePoint 网站托管的团队笔记本上的用户笔记本。</span><span class="sxs-lookup"><span data-stu-id="a172d-113">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

## <a name="user-notebooks"></a><span data-ttu-id="a172d-115">用户笔记本</span><span class="sxs-lookup"><span data-stu-id="a172d-115">User notebooks</span></span>
<span data-ttu-id="a172d-116">要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="a172d-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="a172d-117">`me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。</span><span class="sxs-lookup"><span data-stu-id="a172d-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="a172d-118">`users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。</span><span class="sxs-lookup"><span data-stu-id="a172d-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="a172d-119">使用 [users](users.md) API。</span><span class="sxs-lookup"><span data-stu-id="a172d-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="a172d-120">**注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。</span><span class="sxs-lookup"><span data-stu-id="a172d-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

## <a name="group-notebooks"></a><span data-ttu-id="a172d-121">组笔记本</span><span class="sxs-lookup"><span data-stu-id="a172d-121">Group notebooks</span></span>

<span data-ttu-id="a172d-122">要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="a172d-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="sharepoint-site-notebooks"></a><span data-ttu-id="a172d-123">SharePoint 网站笔记本</span><span class="sxs-lookup"><span data-stu-id="a172d-123">SharePoint site notebooks</span></span>
<span data-ttu-id="a172d-124">要访问 SharePoint 团队网站拥有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="a172d-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="whats-new"></a><span data-ttu-id="a172d-125">最近更新</span><span class="sxs-lookup"><span data-stu-id="a172d-125">What's new</span></span>
<span data-ttu-id="a172d-126">查找有关此 API 集的[最新新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="a172d-126">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>