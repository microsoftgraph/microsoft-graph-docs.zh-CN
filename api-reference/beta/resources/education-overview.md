---
title: 在 Microsoft Graph 中使用教育 API
description: 教育在 Microsoft Graph 中的 Api 增强 Office 365 资源和数据的教育方案，其中包括学校、 学生、 教师、 类、 注册，和工作分配的相关信息。 这使你能够轻松地构建与教育资源集成的解决方案。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516929"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="f8183-104">在 Microsoft Graph 中使用教育 API</span><span class="sxs-lookup"><span data-stu-id="f8183-104">Working with education APIs in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8183-105">教育在 Microsoft Graph 中的 Api 增强 Office 365 资源和数据的教育方案，其中包括学校、 学生、 教师、 类、 注册，和工作分配的相关信息。</span><span class="sxs-lookup"><span data-stu-id="f8183-105">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="f8183-106">这使你能够轻松地构建与教育资源集成的解决方案。</span><span class="sxs-lookup"><span data-stu-id="f8183-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="f8183-107">教育 Api 包括 rostering 资源和分配资源可用于与中的 Microsoft 团队的 rostering 和分配服务进行交互。</span><span class="sxs-lookup"><span data-stu-id="f8183-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="f8183-108">这些资源可用于管理学校名单和自动化学员。</span><span class="sxs-lookup"><span data-stu-id="f8183-108">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="f8183-109">授权</span><span class="sxs-lookup"><span data-stu-id="f8183-109">Authorization</span></span>

<span data-ttu-id="f8183-110">若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="f8183-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="f8183-111">有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="f8183-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="f8183-112">你的应用还需要具有相应的权限。</span><span class="sxs-lookup"><span data-stu-id="f8183-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="f8183-113">有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。</span><span class="sxs-lookup"><span data-stu-id="f8183-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="f8183-114">请求学校 IT 管理员许可的应用权限</span><span class="sxs-lookup"><span data-stu-id="f8183-114">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="f8183-115">若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。</span><span class="sxs-lookup"><span data-stu-id="f8183-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="f8183-116">仅能授权许可一次，除非权限更改。</span><span class="sxs-lookup"><span data-stu-id="f8183-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="f8183-117">管理员同意后，将对租户中的所有用户预配应用。</span><span class="sxs-lookup"><span data-stu-id="f8183-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="f8183-118">若要触发许可对话框，请使用以下 REST 调用。</span><span class="sxs-lookup"><span data-stu-id="f8183-118">To trigger a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="f8183-119">参数</span><span class="sxs-lookup"><span data-stu-id="f8183-119">Parameter</span></span>|<span data-ttu-id="f8183-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8183-120">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="f8183-121">Tenant</span><span class="sxs-lookup"><span data-stu-id="f8183-121">Tenant</span></span>|<span data-ttu-id="f8183-122">学校的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="f8183-122">Tenant ID of the school.</span></span> <span data-ttu-id="f8183-123">使用完整 ID，其中包含 onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="f8183-123">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="f8183-124">clientId</span><span class="sxs-lookup"><span data-stu-id="f8183-124">clientId</span></span>|<span data-ttu-id="f8183-125">应用的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f8183-125">Client ID of the app.</span></span>|
|<span data-ttu-id="f8183-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="f8183-126">redirectUrl</span></span>|<span data-ttu-id="f8183-127">应用重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="f8183-127">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="f8183-128">Rostering</span><span class="sxs-lookup"><span data-stu-id="f8183-128">Rostering</span></span>

<span data-ttu-id="f8183-129">借助名册 API，可以从学校的 Office 365 租户（预配了 [Microsoft 学校数据同步](https://sds.microsoft.com/)）中提取数据。这些 API 提供对有关学校、部门、教师、学生和名册的信息的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f8183-129">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="f8183-130">API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。</span><span class="sxs-lookup"><span data-stu-id="f8183-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="f8183-131">支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。</span><span class="sxs-lookup"><span data-stu-id="f8183-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="f8183-132">这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。</span><span class="sxs-lookup"><span data-stu-id="f8183-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="f8183-133">此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。</span><span class="sxs-lookup"><span data-stu-id="f8183-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="f8183-134">可以使用名册 API 让应用用户了解：</span><span class="sxs-lookup"><span data-stu-id="f8183-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="f8183-135">我是谁</span><span class="sxs-lookup"><span data-stu-id="f8183-135">Who I am</span></span>
- <span data-ttu-id="f8183-136">我参加或教学的课程</span><span class="sxs-lookup"><span data-stu-id="f8183-136">What classes I attend or teach</span></span>
- <span data-ttu-id="f8183-137">我需要做什么以及完成时间</span><span class="sxs-lookup"><span data-stu-id="f8183-137">What I need to do and by when</span></span>

<span data-ttu-id="f8183-138">名册 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="f8183-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="f8183-139">[educationSchool](educationschool.md) - 表示学校。</span><span class="sxs-lookup"><span data-stu-id="f8183-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="f8183-140">[educationClass](educationclass.md) - 表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="f8183-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="f8183-141">[educationTerm](educationterm.md) - 表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="f8183-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="f8183-142">[educationTeacher](educationteacher.md) - 表示主要角色为“教师”的用户。</span><span class="sxs-lookup"><span data-stu-id="f8183-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="f8183-143">[educationStudent](educationstudent.md) - 表示主要角色为“学生”的用户。</span><span class="sxs-lookup"><span data-stu-id="f8183-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="f8183-144">名册 API 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="f8183-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="f8183-145">列出所有学校</span><span class="sxs-lookup"><span data-stu-id="f8183-145">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="f8183-146">列出所教授课程的学校</span><span class="sxs-lookup"><span data-stu-id="f8183-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="f8183-147">为用户列出学校</span><span class="sxs-lookup"><span data-stu-id="f8183-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="f8183-148">获取所有课程</span><span class="sxs-lookup"><span data-stu-id="f8183-148">Get all classes</span></span>](../api/educationroot_list_classes.md )
- [<span data-ttu-id="f8183-149">获取学校的课程</span><span class="sxs-lookup"><span data-stu-id="f8183-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="f8183-150">为用户列出课程</span><span class="sxs-lookup"><span data-stu-id="f8183-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="f8183-151">将课程添加到学校</span><span class="sxs-lookup"><span data-stu-id="f8183-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="f8183-152">获取课程的学生和教师</span><span class="sxs-lookup"><span data-stu-id="f8183-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="f8183-153">将成员添加到课程</span><span class="sxs-lookup"><span data-stu-id="f8183-153">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="f8183-154">列出课程的教师</span><span class="sxs-lookup"><span data-stu-id="f8183-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="f8183-155">获取学校的用户</span><span class="sxs-lookup"><span data-stu-id="f8183-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="f8183-156">作业</span><span class="sxs-lookup"><span data-stu-id="f8183-156">Assignments</span></span> 

<span data-ttu-id="f8183-157">您可以使用 Api 中的工作分配相关 education 集成的 Microsoft 团队中具有工作分配。</span><span class="sxs-lookup"><span data-stu-id="f8183-157">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="f8183-158">Office 365 教育版中的 Microsoft 团队基于相同的教育 Api，并提供使用案例使用 Api 可以执行的操作。</span><span class="sxs-lookup"><span data-stu-id="f8183-158">Microsoft Teams in Office 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="f8183-159">您的应用程序可以使用这些 Api 进行交互的整个生命周期工作分配的工作分配。</span><span class="sxs-lookup"><span data-stu-id="f8183-159">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="f8183-160">工作分配 Api 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="f8183-160">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="f8183-161">[educationAssignment](educationassignment.md) -分配 API 的核心对象。</span><span class="sxs-lookup"><span data-stu-id="f8183-161">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="f8183-162">表示任务或工作分配给类中的学生或团队成员属于其研究单位。</span><span class="sxs-lookup"><span data-stu-id="f8183-162">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="f8183-163">[educationSubmission](educationsubmission.md) -表示的资源的个人 （或组） 提交的工作分配关联薪等级和工作分配的反馈。</span><span class="sxs-lookup"><span data-stu-id="f8183-163">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="f8183-164">[educationResource](educationresource.md) -表示学习对象，它是被分配或提交。</span><span class="sxs-lookup"><span data-stu-id="f8183-164">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="f8183-165">**EducationResource**相关联**educationAssignment**和/或**educationSubmission**。</span><span class="sxs-lookup"><span data-stu-id="f8183-165">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="f8183-166">工作分配 Api 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="f8183-166">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="f8183-167">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="f8183-167">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="f8183-168">发布工作分配</span><span class="sxs-lookup"><span data-stu-id="f8183-168">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="f8183-169">创建工作分配资源</span><span class="sxs-lookup"><span data-stu-id="f8183-169">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="f8183-170">创建提交资源</span><span class="sxs-lookup"><span data-stu-id="f8183-170">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="f8183-171">提交的作业</span><span class="sxs-lookup"><span data-stu-id="f8183-171">Submit assignment</span></span>](../api/educationsubmission-submit.md) 
- [<span data-ttu-id="f8183-172">Unsubmit 工作分配</span><span class="sxs-lookup"><span data-stu-id="f8183-172">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)   
- [<span data-ttu-id="f8183-173">返回学生薪等级和反馈</span><span class="sxs-lookup"><span data-stu-id="f8183-173">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md) 
- [<span data-ttu-id="f8183-174">获取工作分配详细信息</span><span class="sxs-lookup"><span data-stu-id="f8183-174">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="f8183-175">以下是一些常见的使用案例工作分配相关教育版 Api。</span><span class="sxs-lookup"><span data-stu-id="f8183-175">The following are some common use cases for the assignment-related education APIs.</span></span>

|<span data-ttu-id="f8183-176">用例</span><span class="sxs-lookup"><span data-stu-id="f8183-176">Use case</span></span>|<span data-ttu-id="f8183-177">说明</span><span class="sxs-lookup"><span data-stu-id="f8183-177">Description</span></span>|<span data-ttu-id="f8183-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f8183-178">See also</span></span>|
|:-------|:----------|:-------|
|<span data-ttu-id="f8183-179">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="f8183-179">Create assignments</span></span>|<span data-ttu-id="f8183-180">外部系统可以创建类的工作分配，并附加到工作分配的资源。</span><span class="sxs-lookup"><span data-stu-id="f8183-180">An external system can create an assignment for the class and attach resources to the assignment.</span></span>|[<span data-ttu-id="f8183-181">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="f8183-181">Create assignment</span></span>](../api/educationassignment-post-resources.md)|
|<span data-ttu-id="f8183-182">读取工作分配信息</span><span class="sxs-lookup"><span data-stu-id="f8183-182">Read assignment information</span></span>|<span data-ttu-id="f8183-183">分析应用程序可以获取有关分配和学生提交，包括多个日期和薪等级的信息。</span><span class="sxs-lookup"><span data-stu-id="f8183-183">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span>|[<span data-ttu-id="f8183-184">获取工作分配</span><span class="sxs-lookup"><span data-stu-id="f8183-184">Get assignment</span></span>](../api/educationassignment-get.md)|
|<span data-ttu-id="f8183-185">跟踪学生提交</span><span class="sxs-lookup"><span data-stu-id="f8183-185">Track student submissions</span></span>|<span data-ttu-id="f8183-186">您的应用程序可以提供的显示多少拾取学生需要进行评分教师仪表板。</span><span class="sxs-lookup"><span data-stu-id="f8183-186">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>|[<span data-ttu-id="f8183-187">提交资源</span><span class="sxs-lookup"><span data-stu-id="f8183-187">Submission resource</span></span>](educationsubmission.md)|

## <a name="school-data-sync-management"></a><span data-ttu-id="f8183-188">学校数据同步管理</span><span class="sxs-lookup"><span data-stu-id="f8183-188">School data sync management</span></span>

<span data-ttu-id="f8183-189">[学校数据同步](https://sds.microsoft.com/)可帮助自动完成的导入和与 Azure Active Directory (Azure AD) 和 Office 365 同步学生信息系统中的名单数据的过程。</span><span class="sxs-lookup"><span data-stu-id="f8183-189">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="f8183-190">您可以使用在 Microsoft Graph 学校数据同步管理 Api 设置从 CSV 文件或支持的 SI API 连接器的同步。</span><span class="sxs-lookup"><span data-stu-id="f8183-190">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="f8183-191">学校数据同步管理 Api 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="f8183-191">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="f8183-192">列表同步配置文件</span><span class="sxs-lookup"><span data-stu-id="f8183-192">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="f8183-193">获取同步配置文件</span><span class="sxs-lookup"><span data-stu-id="f8183-193">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="f8183-194">创建同步配置文件</span><span class="sxs-lookup"><span data-stu-id="f8183-194">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="f8183-195">删除同步配置文件</span><span class="sxs-lookup"><span data-stu-id="f8183-195">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="f8183-196">暂停正在进行同步</span><span class="sxs-lookup"><span data-stu-id="f8183-196">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="f8183-197">恢复暂停的同步</span><span class="sxs-lookup"><span data-stu-id="f8183-197">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="f8183-198">重置 sync</span><span class="sxs-lookup"><span data-stu-id="f8183-198">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="f8183-199">启动同步上载文件</span><span class="sxs-lookup"><span data-stu-id="f8183-199">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) 
- [<span data-ttu-id="f8183-200">获取一个上载 URL</span><span class="sxs-lookup"><span data-stu-id="f8183-200">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="f8183-201">要获取同步的状态</span><span class="sxs-lookup"><span data-stu-id="f8183-201">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="f8183-202">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="f8183-202">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a><span data-ttu-id="f8183-203">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f8183-203">Next steps</span></span>
<span data-ttu-id="f8183-204">使用 Microsoft Graph 教育 Api 构建访问学员和学校名单的教育解决方案。</span><span class="sxs-lookup"><span data-stu-id="f8183-204">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="f8183-205">了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="f8183-205">To learn more:</span></span>

- <span data-ttu-id="f8183-206">探索对你的方案最有帮助的资源和方法。</span><span class="sxs-lookup"><span data-stu-id="f8183-206">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="f8183-207">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。</span><span class="sxs-lookup"><span data-stu-id="f8183-207">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
