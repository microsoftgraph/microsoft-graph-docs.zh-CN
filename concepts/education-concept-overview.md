---
title: 教育版 API 概述
description: Microsoft Graph 中的教育版 API 可增强 Microsoft 365 资源和与教育情景相关的信息，其中包括有关学校、课程、用户（学生和教师）、作业以及订阅信息。 这使你能够轻松构建与各种学校和课堂情景的教育资源集成的解决方案。
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.custom: scenarios:getting-started
ms.openlocfilehash: 258659da2ad842971043d76ec52888bfd15a236e
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010183"
---
# <a name="education-api-overview"></a><span data-ttu-id="87c65-104">教育版 API 概述</span><span class="sxs-lookup"><span data-stu-id="87c65-104">Education API overview</span></span>

<span data-ttu-id="87c65-105">Microsoft Graph 中的教育版 API 可增强 Microsoft 365 资源和与教育情景相关的信息，其中包括有关学校、课程、用户（学生和教师）、作业以及订阅信息。</span><span class="sxs-lookup"><span data-stu-id="87c65-105">The education API in Microsoft Graph enhances Microsoft 365 resources with information that is relevant for education scenarios, including information about schools, classes, users (students and teachers), assignments, and submissions.</span></span> <span data-ttu-id="87c65-106">这使你能够轻松构建与各种学校和课堂情景的教育资源集成的解决方案。</span><span class="sxs-lookup"><span data-stu-id="87c65-106">This makes it easy for you to build solutions that integrate with educational resources for various school and classroom scenarios.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/EnDM7KMTEqQ]

## <a name="why-integrate-with-education-scenarios"></a><span data-ttu-id="87c65-107">为什么与教育情景集成？</span><span class="sxs-lookup"><span data-stu-id="87c65-107">Why integrate with education scenarios?</span></span>

### <a name="build-applications-that-are-aware-of-class-roster"></a><span data-ttu-id="87c65-108">构建了解班级名册的应用程序</span><span class="sxs-lookup"><span data-stu-id="87c65-108">Build applications that are aware of class roster</span></span>

<span data-ttu-id="87c65-109">大多数教育软件开发人员在早期便了解到，此班级名册是运行其应用程序所需的关键信息之一，而且它通常被锁定在学校的学生信息系统 (SIS) 中。</span><span class="sxs-lookup"><span data-stu-id="87c65-109">Most education software developers learn early on that class roster is one of the key pieces of information they need to run their application, and it's typically locked away inside a school Student Information System (SIS).</span></span> <span data-ttu-id="87c65-110">只要教师将新应用程序引入其课堂，他们就需要花时间手动将名单数据导入到该应用。</span><span class="sxs-lookup"><span data-stu-id="87c65-110">Any time teachers bring a new application into their classroom, they spend time manually importing roster data into the app.</span></span> <span data-ttu-id="87c65-111">许多独立软件供应商 (ISV) 通过连接 SIS 导入名单数据来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="87c65-111">Many independent software vendors (ISVs) address this by connecting with a SIS to import roster data.</span></span> <span data-ttu-id="87c65-112">在具备专有格式的数百个学生信息系统中，这将成为一个挑战。</span><span class="sxs-lookup"><span data-stu-id="87c65-112">With hundreds of Student Information Systems with proprietary formats, this can become a challenge.</span></span> <span data-ttu-id="87c65-113">将 [Microsoft 学校数据同步](https://sds.microsoft.com/)与名单 API 结合使用，可为应用程序开发人员以及学校解决这一难题。</span><span class="sxs-lookup"><span data-stu-id="87c65-113">[Microsoft School Data Sync](https://sds.microsoft.com/), combined with roster APIs, addresses this challenge for application developers and schools.</span></span>

<span data-ttu-id="87c65-114">以下是名单 API 启用的一些情况：</span><span class="sxs-lookup"><span data-stu-id="87c65-114">The following are some of the scenarios that the roster APIs enable:</span></span>

- [<span data-ttu-id="87c65-115">获取学校的所有课程</span><span class="sxs-lookup"><span data-stu-id="87c65-115">Get all classes in a school</span></span>](/graph/api/educationschool-list-classes?view=graph-rest-1.0)
- [<span data-ttu-id="87c65-116">获取课程的所有用户</span><span class="sxs-lookup"><span data-stu-id="87c65-116">Get all users in a class</span></span>](/graph/api/educationclass-list-members?view=graph-rest-1.0)
- [<span data-ttu-id="87c65-117">获取我讲授的所有课程</span><span class="sxs-lookup"><span data-stu-id="87c65-117">Get all the classes I teach</span></span>](/graph/api/educationuser-list-classes?view=graph-rest-1.0)


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a><span data-ttu-id="87c65-118">使用 Microsoft Teams 在“作业”选项卡中创建课程作业</span><span class="sxs-lookup"><span data-stu-id="87c65-118">Use Microsoft Teams to create class assignments in an assignments tab</span></span>

<span data-ttu-id="87c65-119">可以使用与作业相关的教育 API 与 Microsoft Teams 中的作业集成。</span><span class="sxs-lookup"><span data-stu-id="87c65-119">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="87c65-120">Microsoft 365 教育版中的 Microsoft Teams 基于同一教育 API，并提供了使用 API 执行哪些操作的用例。</span><span class="sxs-lookup"><span data-stu-id="87c65-120">Microsoft Teams in Microsoft 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="87c65-121">应用可以使用这些 API 在整个作业生命周期内与作业进行交互。</span><span class="sxs-lookup"><span data-stu-id="87c65-121">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span>

<span data-ttu-id="87c65-122">作业 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="87c65-122">The assignment APIs provide the following key resources:</span></span>

<span data-ttu-id="87c65-123">[educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-1.0) - 作业 API 的核心对象。</span><span class="sxs-lookup"><span data-stu-id="87c65-123">•   [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-1.0) - The core object of the assignments API.</span></span> <span data-ttu-id="87c65-124">是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。</span><span class="sxs-lookup"><span data-stu-id="87c65-124">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
<span data-ttu-id="87c65-125">•   [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-1.0) - 是指个人（或组）提交作业的资源以及该作业的相关成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="87c65-125">•   [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-1.0) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
<span data-ttu-id="87c65-126">•   [educationResource](/graph/api/resources/educationresource?view=graph-rest-1.0) - 是指正在分配或提交的学习对象。</span><span class="sxs-lookup"><span data-stu-id="87c65-126">•   [educationResource](/graph/api/resources/educationresource?view=graph-rest-1.0) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="87c65-127">**educationResource** 与 **educationAssignment** 和/或 **educationSubmission** 相关联。</span><span class="sxs-lookup"><span data-stu-id="87c65-127">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>


<span data-ttu-id="87c65-128">通过作业 API，你的应用可以与 Microsoft Teams 之外的作业服务进行交互。</span><span class="sxs-lookup"><span data-stu-id="87c65-128">With the assignment API, your app can interact with the assignment service outside of Microsoft Teams.</span></span> <span data-ttu-id="87c65-129">Microsoft Teams 将处理分发、截止日期和评分，而系统可以为学生提供丰富的学习体验。</span><span class="sxs-lookup"><span data-stu-id="87c65-129">Microsoft Teams will handle distribution, due dates, and grading while your system can provide a rich learning experience to students.</span></span>
<span data-ttu-id="87c65-130">以下是由作业 API 启用的几个方案示例：</span><span class="sxs-lookup"><span data-stu-id="87c65-130">The following are examples of a few scenarios enabled by the assignments API:</span></span>

- [<span data-ttu-id="87c65-131">添加到应用程序的作业链接</span><span class="sxs-lookup"><span data-stu-id="87c65-131">Add an assignment that links to your application</span></span>](/graph/api/educationclass-post-assignments?view=graph-rest-1.0) 
- [<span data-ttu-id="87c65-132">对于链接到应用程序的作业，将成绩等结果分配给各个学生</span><span class="sxs-lookup"><span data-stu-id="87c65-132">Assign outcomes like grades to individual students for assignments linked to your application</span></span>](/graph/api/educationoutcome-update?view=graph-rest-1.0)
- [<span data-ttu-id="87c65-133">创建学生仪表板以显示哪些作业何时截止</span><span class="sxs-lookup"><span data-stu-id="87c65-133">Create a student dashboard to show which assignments are due by when</span></span>](/graph/api/educationclass-list-assignments?view=graph-rest-1.0)


### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a><span data-ttu-id="87c65-134">使学校管理员能够使用学校数据同步管理（预览版）管理标识和名单同步</span><span class="sxs-lookup"><span data-stu-id="87c65-134">Enable school admins to manage identity and roster sync using School Data Sync Management (preview)</span></span>

<span data-ttu-id="87c65-135">[学校数据同步](https://sds.microsoft.com/)可帮助自动执行从使用 Azure Active Directory (Azure AD) 和 Microsoft 365 的学生信息系统中导入和同步学生标识及名单数据的过程。</span><span class="sxs-lookup"><span data-stu-id="87c65-135">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing student identity and roster data from student information systems with Azure Active Directory (Azure AD) and Microsoft 365.</span></span> <span data-ttu-id="87c65-136">当同步信息时，可以使用名单 API 将名单信息读入应用程序。</span><span class="sxs-lookup"><span data-stu-id="87c65-136">When the information is synchronized, you can use the roster APIs to read the roster information into the applications.</span></span> <span data-ttu-id="87c65-137">如果你是建立学校学生信息系统和学校数据同步整合关系的系统集成者，则可以使用 Microsoft Graph 中的 [SDS 管理 API](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) 从 CSV 文件或受支持的 SIS API 连接器设置同步。</span><span class="sxs-lookup"><span data-stu-id="87c65-137">If you're a system integrator setting up integration of a school's Student Information System with School Data Sync, you can use the [SDS management APIs](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="87c65-138">学校数据同步管理 API 支持用于管理同步的端到端方案；例如：</span><span class="sxs-lookup"><span data-stu-id="87c65-138">School Data Sync management APIs support end-to-end scenarios for managing sync; for example:</span></span>

- [<span data-ttu-id="87c65-139">创建自动启动同步的同步配置文件</span><span class="sxs-lookup"><span data-stu-id="87c65-139">Create a synchronization profile that automatically starts a sync</span></span>](/graph/api/educationsynchronizationprofile-post?view=graph-rest-beta)
- <span data-ttu-id="87c65-140">通过[暂停](/graph/api/educationsynchronizationprofile-pause?view=graph-rest-beta)、[继续](/graph/api/educationsynchronizationprofile-resume?view=graph-rest-beta)和[重置](/graph/api/educationsynchronizationprofile-reset?view=graph-rest-beta)操作管理同步生命周期</span><span class="sxs-lookup"><span data-stu-id="87c65-140">Manage sync lifecycle with [pause](/graph/api/educationsynchronizationprofile-pause?view=graph-rest-beta), [resume](/graph/api/educationsynchronizationprofile-resume?view=graph-rest-beta) and [reset](/graph/api/educationsynchronizationprofile-reset?view=graph-rest-beta) operations</span></span>

## <a name="api-reference"></a><span data-ttu-id="87c65-141">API 参考</span><span class="sxs-lookup"><span data-stu-id="87c65-141">API reference</span></span>
<span data-ttu-id="87c65-142">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="87c65-142">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="87c65-143">Microsoft Graph v1.0 中的教育版 API</span><span class="sxs-lookup"><span data-stu-id="87c65-143">Education API in Microsoft Graph v1.0</span></span>](/graph/api/resources/education-overview?view=graph-rest-1.0)
- [<span data-ttu-id="87c65-144">Microsoft Graph beta 中的教育版 API</span><span class="sxs-lookup"><span data-stu-id="87c65-144">Education API in Microsoft Graph beta</span></span>](/graph/api/resources/education-overview?view=graph-rest-beta)


## <a name="next-steps"></a><span data-ttu-id="87c65-145">后续步骤</span><span class="sxs-lookup"><span data-stu-id="87c65-145">Next Steps</span></span>

- <span data-ttu-id="87c65-146">若要开始使用教育版 API，请参阅：</span><span class="sxs-lookup"><span data-stu-id="87c65-146">To start using the education APIs, see:</span></span>
  - [<span data-ttu-id="87c65-147">使用名单 API</span><span class="sxs-lookup"><span data-stu-id="87c65-147">Use the roster APIs</span></span>](/graph/api/resources/education-overview?view=graph-rest-1.0)
  - [<span data-ttu-id="87c65-148">使用作业 API</span><span class="sxs-lookup"><span data-stu-id="87c65-148">Use the assignment APIs</span></span>](/graph/api/resources/educationassignment?view=graph-rest-1.0)
  - [<span data-ttu-id="87c65-149">使用 SDS 管理 API</span><span class="sxs-lookup"><span data-stu-id="87c65-149">Use the SDS management APIs</span></span>](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta)
- <span data-ttu-id="87c65-150">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中试用教育版 API。</span><span class="sxs-lookup"><span data-stu-id="87c65-150">Try the education APIs in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="87c65-151">浏览下面的教育相关示例：</span><span class="sxs-lookup"><span data-stu-id="87c65-151">Explore the following education-related samples:</span></span>
  - [<span data-ttu-id="87c65-152">SSO 和排班 .NET 示例</span><span class="sxs-lookup"><span data-stu-id="87c65-152">.NET sample for SSO & Rostering</span></span>](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
  - [<span data-ttu-id="87c65-153">配置文件管理 API 示例</span><span class="sxs-lookup"><span data-stu-id="87c65-153">Sample for profile management APIs</span></span>](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples) 



