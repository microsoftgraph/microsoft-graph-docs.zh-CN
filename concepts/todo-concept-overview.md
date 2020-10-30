---
title: 微软待办 API 概述
description: 微软待办提供一种管理任务和计划日常工作的简单方法
author: avijityadav
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 34dc63ab14bc6cc1a2c118e6a77f9f6cc597bccc
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796743"
---
# <a name="to-do-api-overview"></a><span data-ttu-id="4b15b-103">微软待办 API 概述</span><span class="sxs-lookup"><span data-stu-id="4b15b-103">To Do API overview</span></span>
<span data-ttu-id="4b15b-104">微软待办提供了一种简单的方法便于用户管理其任务和计划日常工作。</span><span class="sxs-lookup"><span data-stu-id="4b15b-104">Microsoft To Do provides a simple way for people to manage their tasks and plan their day.</span></span> <span data-ttu-id="4b15b-105">任务以任务列表形式组织，可以从任何设备跨微软待办客户端、Outlook 和 Teams 访问。</span><span class="sxs-lookup"><span data-stu-id="4b15b-105">Tasks are organized in task lists, which can be accessed across To Do clients, Outlook and Teams from any device.</span></span>

<span data-ttu-id="4b15b-106">**微软待办 Windows 应用**</span><span class="sxs-lookup"><span data-stu-id="4b15b-106">**To Do Windows app**</span></span>

<span data-ttu-id="4b15b-107">![微软待办 Windows 应用的屏幕截图](./images/todo-windows-app.png "微软待办 Windows 应用的图像")</span><span class="sxs-lookup"><span data-stu-id="4b15b-107">![Screenshot of a Microsoft To Do Windows App](./images/todo-windows-app.png "Image of Microsoft To Do Windows App")</span></span>

## <a name="why-integrate-with-to-do"></a><span data-ttu-id="4b15b-108">为什么与微软待办集成？</span><span class="sxs-lookup"><span data-stu-id="4b15b-108">Why integrate with To Do?</span></span>

### <a name="ease-of-organizing-and-tracking-tasks"></a><span data-ttu-id="4b15b-109">轻松整理和跟踪任务</span><span class="sxs-lookup"><span data-stu-id="4b15b-109">Ease of organizing and tracking tasks</span></span>
<span data-ttu-id="4b15b-110">微软待办可帮助你为任何内容创建列表，从工作分配到家庭项目再到杂货。</span><span class="sxs-lookup"><span data-stu-id="4b15b-110">Microsoft To Do helps you create a list for anything, from work assignments to home projects to groceries.</span></span> <span data-ttu-id="4b15b-111">可通过添加提醒、截止日期和备注来跟踪最后期限。</span><span class="sxs-lookup"><span data-stu-id="4b15b-111">You can keep track of deadlines by adding reminders, due dates, and notes.</span></span> <span data-ttu-id="4b15b-112">可使用适用于 iOS、Android、Mac、Windows 和 Web 的微软待办应用从任意位置访问列表。</span><span class="sxs-lookup"><span data-stu-id="4b15b-112">You can access your lists from anywhere with the Microsoft To Do apps for iOS, Android, Mac, Windows, and the web.</span></span> 

### <a name="integrate-across-microsoft-365"></a><span data-ttu-id="4b15b-113">跨 Microsoft 365 集成</span><span class="sxs-lookup"><span data-stu-id="4b15b-113">Integrate across Microsoft 365</span></span>
<span data-ttu-id="4b15b-114">微软待办是 Microsoft 365 中唯一存放个人任务的位置。</span><span class="sxs-lookup"><span data-stu-id="4b15b-114">To Do is the single destination for personal tasks in Microsoft 365.</span></span> <span data-ttu-id="4b15b-115">因此，它与 Microsoft 365 中心、Outlook 和 Teams 紧密集成。</span><span class="sxs-lookup"><span data-stu-id="4b15b-115">So it’s deeply integrated with Microsoft 365 hubs, Outlook, and Teams.</span></span> <span data-ttu-id="4b15b-116">在这些产品中创建的任务将与微软待办同步，以便你可以跨设备访问和管理它们。</span><span class="sxs-lookup"><span data-stu-id="4b15b-116">Tasks created in those products sync with To Do so you can access and manage them across devices.</span></span> <span data-ttu-id="4b15b-117">微软待办集成可以帮助你吸引数百万使用微软待办的用户将 Outlook 和 Teams 中的任务收集到一个集成视图中。</span><span class="sxs-lookup"><span data-stu-id="4b15b-117">To Do integration can help you reach millions of users who use To Do to gather tasks from Outlook and Teams into one integrated view.</span></span>  

### <a name="support-task-completion-using-linked-resources"></a><span data-ttu-id="4b15b-118">支持使用链接的资源完成任务</span><span class="sxs-lookup"><span data-stu-id="4b15b-118">Support task completion using linked resources</span></span>
<span data-ttu-id="4b15b-119">微软待办提供了一个称为“ _链接的资源_ ”的新实体，你可以使用该实体创建可链接回其原始源的任务。</span><span class="sxs-lookup"><span data-stu-id="4b15b-119">Microsoft To Do provides a new entity called _linked resource_ , which you can use to create tasks that can link back to their original sources.</span></span> <span data-ttu-id="4b15b-120">可通过创建链接到你的产品或服务的任务，使用此功能在你的工作流中无缝集成微软待办。</span><span class="sxs-lookup"><span data-stu-id="4b15b-120">You can use this to seamlessly integrate To Do in your workflow by creating tasks that link to your product or service.</span></span> 

## <a name="common-to-do-api-operations"></a><span data-ttu-id="4b15b-121">常用微软待办 API 操作</span><span class="sxs-lookup"><span data-stu-id="4b15b-121">Common To Do API operations</span></span>

|<span data-ttu-id="4b15b-122">操作</span><span class="sxs-lookup"><span data-stu-id="4b15b-122">Operation</span></span>|<span data-ttu-id="4b15b-123">请求</span><span class="sxs-lookup"><span data-stu-id="4b15b-123">Request</span></span>|
|:--------|:--|
| <span data-ttu-id="4b15b-124">列出所有任务列表</span><span class="sxs-lookup"><span data-stu-id="4b15b-124">List all the task lists</span></span> | <span data-ttu-id="4b15b-125">获取 https://graph.microsoft.com/v1.0/me/todo/lists</span><span class="sxs-lookup"><span data-stu-id="4b15b-125">GET https://graph.microsoft.com/v1.0/me/todo/lists</span></span> |
| <span data-ttu-id="4b15b-126">列出任务列表中的所有任务</span><span class="sxs-lookup"><span data-stu-id="4b15b-126">List all tasks in a task list</span></span> | <span data-ttu-id="4b15b-127">获取 https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="4b15b-127">GET https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span></span> |
| <span data-ttu-id="4b15b-128">创建新任务</span><span class="sxs-lookup"><span data-stu-id="4b15b-128">Create a new task</span></span> | <span data-ttu-id="4b15b-129">发布 https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="4b15b-129">POST https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks</span></span> |
| <span data-ttu-id="4b15b-130">更新任务</span><span class="sxs-lookup"><span data-stu-id="4b15b-130">Update a task</span></span> | <span data-ttu-id="4b15b-131">修补 https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span><span class="sxs-lookup"><span data-stu-id="4b15b-131">PATCH https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span></span> |
| <span data-ttu-id="4b15b-132">删除任务</span><span class="sxs-lookup"><span data-stu-id="4b15b-132">Delete a task</span></span> | <span data-ttu-id="4b15b-133">删除 https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span><span class="sxs-lookup"><span data-stu-id="4b15b-133">DELETE https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span></span> |

## <a name="api-reference"></a><span data-ttu-id="4b15b-134">API 参考</span><span class="sxs-lookup"><span data-stu-id="4b15b-134">API reference</span></span>
<span data-ttu-id="4b15b-135">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="4b15b-135">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="4b15b-136">Microsoft Graph 中的微软待办 API</span><span class="sxs-lookup"><span data-stu-id="4b15b-136">To Do API in Microsoft Graph</span></span>](/graph/api/resources/todo-overview)
