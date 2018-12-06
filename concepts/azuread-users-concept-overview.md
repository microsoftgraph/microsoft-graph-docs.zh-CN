---
title: Microsoft Graph 中用户的概述
description: 用户是 Microsoft Graph 中 Azure Active Directory (Azure AD) 工作或学校用户帐户或 Microsoft 帐户的表示形式。 Microsoft Graph 中的**用户**资源是一个中心，可以从这里访问与用户相关的关系和资源。
ms.openlocfilehash: 2f07cdea940a7fe09b034f8fb21f443447ec67d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091875"
---
# <a name="overview-of-users-in-microsoft-graph"></a><span data-ttu-id="a3367-104">Microsoft Graph 中用户的概述</span><span class="sxs-lookup"><span data-stu-id="a3367-104">Overview of users in Microsoft Graph</span></span>

<span data-ttu-id="a3367-105">用户是 Microsoft Graph 中 Azure Active Directory (Azure AD) 工作或学校用户帐户或 Microsoft 帐户的表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3367-105">Users are the representation of an Azure Active Directory (Azure AD) work or school user account or a Microsoft account in Microsoft Graph.</span></span> <span data-ttu-id="a3367-106">Microsoft Graph 中的**用户**资源是一个中心，可以从这里访问与用户相关的关系和资源。</span><span class="sxs-lookup"><span data-stu-id="a3367-106">The **user** resource in Microsoft Graph is a hub from which you can access the relationships and resources that are relevant to your users.</span></span>

![关系图显示用户连接到的日历、电子邮件、联系人、会议、任务、网站和文档](images/users.png)

## <a name="develop-user-centric-applications"></a><span data-ttu-id="a3367-108">开发以用户为中心的应用程序</span><span class="sxs-lookup"><span data-stu-id="a3367-108">Develop user-centric applications</span></span>

<span data-ttu-id="a3367-109">你可使用 Microsoft Graph 访问与登录用户上下文相关的关系、文档、联系人和首选项。</span><span class="sxs-lookup"><span data-stu-id="a3367-109">You can use Microsoft Graph to access the relationships, documents, contacts, and preferences that are contextually relevant to the signed-in user.</span></span> <span data-ttu-id="a3367-110">**用户**资源提供了无需执行其他调用即可访问和操作用户资源的简单方法，可查找特定的身份验证信息，并直接对其他 Microsoft Graph 资源发出查询。</span><span class="sxs-lookup"><span data-stu-id="a3367-110">The **user** resource provides straightforward way for you to access and manipulate user resources without having to perform additional calls, look up specific authentication information, and directly issue queries against other Microsoft Graph resources.</span></span>

<span data-ttu-id="a3367-111">若要访问用户的信息和数据，你需要[以用户身份进行访问](auth-v2-user.md)。</span><span class="sxs-lookup"><span data-stu-id="a3367-111">To access a user's information and data, you'll need to [get access on their behalf](auth-v2-user.md).</span></span> <span data-ttu-id="a3367-112">验证应用程序并获得[管理员同意](permissions-reference.md)，即可使用和更新与用户关联的更广泛的实体。</span><span class="sxs-lookup"><span data-stu-id="a3367-112">Authenticating your application with [admin consent](permissions-reference.md) enables you to work with and update a wider range of entities associated with a user.</span></span>

### <a name="manage-your-organization"></a><span data-ttu-id="a3367-113">管理组织</span><span class="sxs-lookup"><span data-stu-id="a3367-113">Manage your organization</span></span>

<span data-ttu-id="a3367-114">在组织中创建新用户或更新现有用户的资源和关系。</span><span class="sxs-lookup"><span data-stu-id="a3367-114">Create new users in your organization or update the resources and relationships for existing users.</span></span> <span data-ttu-id="a3367-115">可使用 Microsoft Graph 执行以下用户管理任务：</span><span class="sxs-lookup"><span data-stu-id="a3367-115">You can use Microsoft Graph to perform the following user management tasks:</span></span> 

- <span data-ttu-id="a3367-116">创建或删除 Azure AD 组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="a3367-116">Create or delete users in your Azure AD organization.</span></span>
- <span data-ttu-id="a3367-117">列出用户的组成员资格并确定用户是否为组的成员。</span><span class="sxs-lookup"><span data-stu-id="a3367-117">List a user's group memberships and determine whether a user is a member of a group.</span></span>
- <span data-ttu-id="a3367-118">列出向某用户报告的用户和向某用户分配经理。</span><span class="sxs-lookup"><span data-stu-id="a3367-118">List the users who report to a user and assign managers to a user.</span></span>
- <span data-ttu-id="a3367-119">上传或检索用户的照片。</span><span class="sxs-lookup"><span data-stu-id="a3367-119">Upload or retrieve a photo for the user.</span></span>

### <a name="work-with-calendars-and-tasks"></a><span data-ttu-id="a3367-120">使用日历和任务</span><span class="sxs-lookup"><span data-stu-id="a3367-120">Work with calendars and tasks</span></span>

<span data-ttu-id="a3367-121">可查看、查询和更新与某用户关联的用户日历和日历组，包括：</span><span class="sxs-lookup"><span data-stu-id="a3367-121">You can view, query, and update user calendar and calendar groups associated with a user, including:</span></span>

- <span data-ttu-id="a3367-122">在用户日历上列出和创建事件。</span><span class="sxs-lookup"><span data-stu-id="a3367-122">List and create events on a users calendar.</span></span>
- <span data-ttu-id="a3367-123">查看分配给用户的任务。</span><span class="sxs-lookup"><span data-stu-id="a3367-123">View tasks assigned to a user.</span></span>
- <span data-ttu-id="a3367-124">为一组用户查找空闲的会议时间。</span><span class="sxs-lookup"><span data-stu-id="a3367-124">Find free meeting times for a set of users.</span></span>
- <span data-ttu-id="a3367-125">获取用户日历上设置的提醒列表。</span><span class="sxs-lookup"><span data-stu-id="a3367-125">Get a list of reminders set on a user's calendar.</span></span>

### <a name="administer-mail-and-handle-contacts"></a><span data-ttu-id="a3367-126">管理邮件和处理联系人</span><span class="sxs-lookup"><span data-stu-id="a3367-126">Administer mail and handle contacts</span></span>

<span data-ttu-id="a3367-127">可配置用户邮件设置和联系人列表，并代表用户发送邮件，包括：</span><span class="sxs-lookup"><span data-stu-id="a3367-127">You can configure user mail settings and contact lists and send mail on a user's behalf, including:</span></span>

- <span data-ttu-id="a3367-128">列出邮件消息和发送新邮件。</span><span class="sxs-lookup"><span data-stu-id="a3367-128">List mail messages and send new mail.</span></span>
- <span data-ttu-id="a3367-129">创建和列出用户联系人，并组织文件夹中的联系人。</span><span class="sxs-lookup"><span data-stu-id="a3367-129">Create and list user contacts and organize contacts in folders.</span></span>
- <span data-ttu-id="a3367-130">检索并更新邮箱文件夹和设置。</span><span class="sxs-lookup"><span data-stu-id="a3367-130">Retrieve and update mailbox folders and settings.</span></span>

### <a name="enrich-your-app-with-user-insights"></a><span data-ttu-id="a3367-131">利用用户见解丰富应用</span><span class="sxs-lookup"><span data-stu-id="a3367-131">Enrich your app with user insights</span></span>

<span data-ttu-id="a3367-132">通过推广最近使用的文档或热门文档以及与用户关联的联系人，最大限度地提高应用程序的关联性。</span><span class="sxs-lookup"><span data-stu-id="a3367-132">Maximize relevance in your application by promoting recently used or trending documents and contacts associated with a user.</span></span> <span data-ttu-id="a3367-133">可以使用 Microsoft Graph：</span><span class="sxs-lookup"><span data-stu-id="a3367-133">You can use Microsoft Graph to:</span></span>

- <span data-ttu-id="a3367-134">返回用户最近查看和修改的文档。</span><span class="sxs-lookup"><span data-stu-id="a3367-134">Return documents recently viewed and modified by a user.</span></span>
- <span data-ttu-id="a3367-135">返回有关用户活动的文档和网站。</span><span class="sxs-lookup"><span data-stu-id="a3367-135">Return documents and sites trending around a user's activity.</span></span>
- <span data-ttu-id="a3367-136">列出通过电子邮件或 OneDrive for Business 与用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="a3367-136">List documents shared with a user through email or OneDrive for Business.</span></span>

## <a name="api-reference"></a><span data-ttu-id="a3367-137">API 参考</span><span class="sxs-lookup"><span data-stu-id="a3367-137">API reference</span></span>
<span data-ttu-id="a3367-138">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="a3367-138">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="a3367-139">Microsoft Graph v1.0 中的用户 API</span><span class="sxs-lookup"><span data-stu-id="a3367-139">Users API in Microsoft Graph v1.0</span></span>](/graph/api/resources/users?view=graph-rest-1.0)
- [<span data-ttu-id="a3367-140">Microsoft Graph beta 中的用户 API</span><span class="sxs-lookup"><span data-stu-id="a3367-140">Users API in Microsoft Graph beta</span></span>](/graph/api/resources/users?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="a3367-141">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a3367-141">Next steps</span></span>

- <span data-ttu-id="a3367-142">了解有关如何[使用用户](/graph/api/resources/users?view=graph-rest-1.0)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a3367-142">Learn more about how to [work with users](/graph/api/resources/users?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="a3367-143">从 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)的**用户**资源探索自己的数据。</span><span class="sxs-lookup"><span data-stu-id="a3367-143">Explore your own data from the **user** resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="a3367-144">[代表用户](auth-v2-user.md)或[作为管理员同意的守护程序或服务](auth-v2-service.md)使用 Microsoft Graph 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="a3367-144">Authenticate with Microsoft Graph [on behalf of a user](auth-v2-user.md) or [as a daemon or service by consent of an administator](auth-v2-service.md).</span></span>
- <span data-ttu-id="a3367-145">为使用 [Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0) 的用户设置访问控制和策略。</span><span class="sxs-lookup"><span data-stu-id="a3367-145">Set access control and policies for users with the [Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="a3367-146">审阅应用访问用户数据所需的[权限](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a3367-146">Review the [permissions](permissions-reference.md) your app will need to access user data.</span></span> 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](changelog.md).
-->
