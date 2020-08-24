---
title: 使用微软待办 API
description: 可使用 Microsoft Graph API 创建与微软待办中的任务连接的应用。
author: avijityadav
localization_priority: Priority
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 14dce46dbfe85883a3e9cfbe6f25efa0a04dc31d
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849876"
---
# <a name="use-the-microsoft-to-do-api"></a><span data-ttu-id="2b68b-103">使用微软待办 API</span><span class="sxs-lookup"><span data-stu-id="2b68b-103">Use the Microsoft To Do API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b68b-104">使用 Microsoft Graph 微软待办 API 创建可跨微软待办客户端与任务连接的应用。</span><span class="sxs-lookup"><span data-stu-id="2b68b-104">Use the Microsoft Graph To Do API to create an app that connects with tasks across Microsoft To Do clients.</span></span> <span data-ttu-id="2b68b-105">使用任务构建各种体验，如下所示：</span><span class="sxs-lookup"><span data-stu-id="2b68b-105">Build a variety of experiences with tasks, such as the following:</span></span>

* <span data-ttu-id="2b68b-106">从应用的工作流（例如，从电子邮件或通知）创建任务，并将其保存到微软待办中。</span><span class="sxs-lookup"><span data-stu-id="2b68b-106">Create tasks from your app’s workflow, for example, from email or notifications, and save them in To Do.</span></span> <span data-ttu-id="2b68b-107">使用 [linkedResource](linkedresource.md) 实体将链接存储回你的应用。</span><span class="sxs-lookup"><span data-stu-id="2b68b-107">Use the [linkedResource](linkedresource.md) entity to store the link back to your app.</span></span>
* <span data-ttu-id="2b68b-108">将应用的现有任务与微软待办进行同步，并创建单个任务视图，以便更好地确定优先顺序和实施管理。</span><span class="sxs-lookup"><span data-stu-id="2b68b-108">Sync your app’s existing tasks with To Do and create a single task view for better prioritization and manageability.</span></span>
* <span data-ttu-id="2b68b-109">在自定义业务应用程序中管理微软待办任务。</span><span class="sxs-lookup"><span data-stu-id="2b68b-109">Manage To Do tasks in a custom business application.</span></span>

<span data-ttu-id="2b68b-110">目前，API 仅支持由已登录用户委派的权限。</span><span class="sxs-lookup"><span data-stu-id="2b68b-110">Currently, the API supports only permissions delegated by the signed-in user.</span></span>
 
<span data-ttu-id="2b68b-111">在开始使用微软待办 API 之前，请查看资源以及它们之间的关系。</span><span class="sxs-lookup"><span data-stu-id="2b68b-111">Before starting with the To Do API, take a look at the resources and how they relate to one another.</span></span>

![微软待办 API 实体](/graph/images/todo-api-entities.png)

## <a name="task-list"></a><span data-ttu-id="2b68b-113">任务列表</span><span class="sxs-lookup"><span data-stu-id="2b68b-113">Task list</span></span>

<span data-ttu-id="2b68b-114">[todoTaskList](./todotasklist.md) 代表 [todoTask](./todotask.md) 资源的逻辑容器。</span><span class="sxs-lookup"><span data-stu-id="2b68b-114">A [todoTaskList](./todotasklist.md) represents a logical container of [todoTask](./todotask.md) resources.</span></span> <span data-ttu-id="2b68b-115">目前只能在任务列表中创建任务。</span><span class="sxs-lookup"><span data-stu-id="2b68b-115">You can currently create tasks only in a task list.</span></span> <span data-ttu-id="2b68b-116">若要[获取所有任务列表](../api/todotasklist-get.md)，请执行以下 HTTP 请求：</span><span class="sxs-lookup"><span data-stu-id="2b68b-116">To [get all your task lists](../api/todotasklist-get.md), make the following HTTP request:</span></span>

``` http
GET /me/todo/lists
```

## <a name="task"></a><span data-ttu-id="2b68b-117">任务</span><span class="sxs-lookup"><span data-stu-id="2b68b-117">Task</span></span>

<span data-ttu-id="2b68b-118">[todoTask](./todotask.md) 表示任务，即可跟踪和完成的一件工作或个人项目。</span><span class="sxs-lookup"><span data-stu-id="2b68b-118">A [todoTask](./todotask.md) represents a task, i.e. a piece of work or personal item that can be tracked and completed.</span></span> <span data-ttu-id="2b68b-119">若要从任务列表中获取任务，请执行以下 HTTP 请求：</span><span class="sxs-lookup"><span data-stu-id="2b68b-119">To get your tasks from a task list, make the following HTTP request:</span></span>
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
```

## <a name="linked-resource"></a><span data-ttu-id="2b68b-120">链接的资源</span><span class="sxs-lookup"><span data-stu-id="2b68b-120">Linked resource</span></span>

<span data-ttu-id="2b68b-121">[linkedResource](linkedresource.md) 表示与任务相关的合作伙伴应用程序中的任何项目，例如从中创建任务的项目（如电子邮件）。</span><span class="sxs-lookup"><span data-stu-id="2b68b-121">A [linkedResource](linkedresource.md) represents any item from a partner application related to the task, e.g. an item like email from where a task was created.</span></span> <span data-ttu-id="2b68b-122">可以使用它来将信息和链接存储回你的应用中的相关项。</span><span class="sxs-lookup"><span data-stu-id="2b68b-122">You can use it to store information and the link back to the related item in your app.</span></span> <span data-ttu-id="2b68b-123">若要从任务获取链接的资源，请执行以下 HTTP 请求：</span><span class="sxs-lookup"><span data-stu-id="2b68b-123">To get a linked resource from a task, make the following HTTP request:</span></span>
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a><span data-ttu-id="2b68b-124">使用 delta 查询跟踪更改</span><span class="sxs-lookup"><span data-stu-id="2b68b-124">Track changes using delta query</span></span>

<span data-ttu-id="2b68b-125">出于性能原因，可能需要维护对象的本地缓存，并使用 [delta 查询](/graph/delta-query-overview)定期将本地缓存与服务器同步。</span><span class="sxs-lookup"><span data-stu-id="2b68b-125">For performance reasons, you may want to maintain a local cache of objects, and periodically synchronize the local cache with the server, using [delta query](/graph/delta-query-overview).</span></span> 

<span data-ttu-id="2b68b-126">以下微软待办 API 资源支持 delta 查询：</span><span class="sxs-lookup"><span data-stu-id="2b68b-126">The following To Do API resources support delta query:</span></span>
* <span data-ttu-id="2b68b-127">任务列表中的 [todoTask](./todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b68b-127">[todoTask](./todotask.md) collection in a task list</span></span>
* [<span data-ttu-id="2b68b-128">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="2b68b-128">todoTaskList</span></span>](./todotasklist.md)

## <a name="whats-new"></a><span data-ttu-id="2b68b-129">最近更新</span><span class="sxs-lookup"><span data-stu-id="2b68b-129">What's new</span></span>
<span data-ttu-id="2b68b-130">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="2b68b-130">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>