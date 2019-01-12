---
title: 在 Microsoft Graph 中使用教育 API
description: 教育在 Microsoft Graph 中的 Api 增强 Office 365 资源和数据的教育方案，其中包括学校、 学生、 教师、 类、 注册，和工作分配的相关信息。 这使你能够轻松地构建与教育资源集成的解决方案。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f5803a5a74933bfe4f09661e68288bc11954a65b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958087"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="15ec9-104">在 Microsoft Graph 中使用教育 API</span><span class="sxs-lookup"><span data-stu-id="15ec9-104">Working with education APIs in Microsoft Graph</span></span>

> <span data-ttu-id="15ec9-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="15ec9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15ec9-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="15ec9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15ec9-107">教育在 Microsoft Graph 中的 Api 增强 Office 365 资源和数据的教育方案，其中包括学校、 学生、 教师、 类、 注册，和工作分配的相关信息。</span><span class="sxs-lookup"><span data-stu-id="15ec9-107">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="15ec9-108">这使你能够轻松地构建与教育资源集成的解决方案。</span><span class="sxs-lookup"><span data-stu-id="15ec9-108">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="15ec9-109">教育 Api 包括 rostering 资源和分配资源可用于与中的 Microsoft 团队的 rostering 和分配服务进行交互。</span><span class="sxs-lookup"><span data-stu-id="15ec9-109">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="15ec9-110">这些资源可用于管理学校名单和自动化学员。</span><span class="sxs-lookup"><span data-stu-id="15ec9-110">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="15ec9-111">授权</span><span class="sxs-lookup"><span data-stu-id="15ec9-111">Authorization</span></span>

<span data-ttu-id="15ec9-112">若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="15ec9-112">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="15ec9-113">有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="15ec9-113">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="15ec9-114">你的应用还需要具有相应的权限。</span><span class="sxs-lookup"><span data-stu-id="15ec9-114">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="15ec9-115">有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。</span><span class="sxs-lookup"><span data-stu-id="15ec9-115">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="15ec9-116">请求学校 IT 管理员许可的应用权限</span><span class="sxs-lookup"><span data-stu-id="15ec9-116">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="15ec9-117">若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。</span><span class="sxs-lookup"><span data-stu-id="15ec9-117">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="15ec9-118">仅能授权许可一次，除非权限更改。</span><span class="sxs-lookup"><span data-stu-id="15ec9-118">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="15ec9-119">管理员同意后，将对租户中的所有用户预配应用。</span><span class="sxs-lookup"><span data-stu-id="15ec9-119">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="15ec9-120">若要触发许可对话框，请使用以下 REST 调用。</span><span class="sxs-lookup"><span data-stu-id="15ec9-120">To trigger a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="15ec9-121">参数</span><span class="sxs-lookup"><span data-stu-id="15ec9-121">Parameter</span></span>|<span data-ttu-id="15ec9-122">说明</span><span class="sxs-lookup"><span data-stu-id="15ec9-122">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="15ec9-123">Tenant</span><span class="sxs-lookup"><span data-stu-id="15ec9-123">Tenant</span></span>|<span data-ttu-id="15ec9-124">学校的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="15ec9-124">Tenant ID of the school.</span></span> <span data-ttu-id="15ec9-125">使用完整 ID，其中包含 onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="15ec9-125">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="15ec9-126">clientId</span><span class="sxs-lookup"><span data-stu-id="15ec9-126">clientId</span></span>|<span data-ttu-id="15ec9-127">应用的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="15ec9-127">Client ID of the app.</span></span>|
|<span data-ttu-id="15ec9-128">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="15ec9-128">redirectUrl</span></span>|<span data-ttu-id="15ec9-129">应用重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="15ec9-129">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="15ec9-130">Rostering</span><span class="sxs-lookup"><span data-stu-id="15ec9-130">Rostering</span></span>

<span data-ttu-id="15ec9-131">借助名册 API，可以从学校的 Office 365 租户（预配了 [Microsoft 学校数据同步](https://sds.microsoft.com/)）中提取数据。这些 API 提供对有关学校、部门、教师、学生和名册的信息的访问权限。</span><span class="sxs-lookup"><span data-stu-id="15ec9-131">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="15ec9-132">API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。</span><span class="sxs-lookup"><span data-stu-id="15ec9-132">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="15ec9-133">支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。</span><span class="sxs-lookup"><span data-stu-id="15ec9-133">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="15ec9-134">这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。</span><span class="sxs-lookup"><span data-stu-id="15ec9-134">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="15ec9-135">此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。</span><span class="sxs-lookup"><span data-stu-id="15ec9-135">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="15ec9-136">可以使用名册 API 让应用用户了解：</span><span class="sxs-lookup"><span data-stu-id="15ec9-136">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="15ec9-137">我是谁</span><span class="sxs-lookup"><span data-stu-id="15ec9-137">Who I am</span></span>
- <span data-ttu-id="15ec9-138">我参加或教学的课程</span><span class="sxs-lookup"><span data-stu-id="15ec9-138">What classes I attend or teach</span></span>
- <span data-ttu-id="15ec9-139">我需要做什么以及完成时间</span><span class="sxs-lookup"><span data-stu-id="15ec9-139">What I need to do and by when</span></span>

<span data-ttu-id="15ec9-140">名册 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="15ec9-140">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="15ec9-141">[educationSchool](educationschool.md) - 表示学校。</span><span class="sxs-lookup"><span data-stu-id="15ec9-141">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="15ec9-142">[educationClass](educationclass.md) - 表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="15ec9-142">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="15ec9-143">[educationTerm](educationterm.md) - 表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="15ec9-143">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="15ec9-144">[educationTeacher](educationteacher.md) - 表示主要角色为“教师”的用户。</span><span class="sxs-lookup"><span data-stu-id="15ec9-144">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="15ec9-145">[educationStudent](educationstudent.md) - 表示主要角色为“学生”的用户。</span><span class="sxs-lookup"><span data-stu-id="15ec9-145">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="15ec9-146">名册 API 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="15ec9-146">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="15ec9-147">列出所有学校</span><span class="sxs-lookup"><span data-stu-id="15ec9-147">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="15ec9-148">列出所教授课程的学校</span><span class="sxs-lookup"><span data-stu-id="15ec9-148">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="15ec9-149">为用户列出学校</span><span class="sxs-lookup"><span data-stu-id="15ec9-149">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="15ec9-150">获取所有课程</span><span class="sxs-lookup"><span data-stu-id="15ec9-150">Get all classes</span></span>](../api/educationroot_list_classes.md )
- [<span data-ttu-id="15ec9-151">获取学校的课程</span><span class="sxs-lookup"><span data-stu-id="15ec9-151">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="15ec9-152">为用户列出课程</span><span class="sxs-lookup"><span data-stu-id="15ec9-152">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="15ec9-153">将课程添加到学校</span><span class="sxs-lookup"><span data-stu-id="15ec9-153">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="15ec9-154">获取课程的学生和教师</span><span class="sxs-lookup"><span data-stu-id="15ec9-154">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="15ec9-155">将成员添加到课程</span><span class="sxs-lookup"><span data-stu-id="15ec9-155">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="15ec9-156">列出课程的教师</span><span class="sxs-lookup"><span data-stu-id="15ec9-156">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="15ec9-157">获取学校的用户</span><span class="sxs-lookup"><span data-stu-id="15ec9-157">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="15ec9-158">作业</span><span class="sxs-lookup"><span data-stu-id="15ec9-158">Assignments</span></span> 

<span data-ttu-id="15ec9-159">您可以使用 Api 中的工作分配相关 education 集成的 Microsoft 团队中具有工作分配。</span><span class="sxs-lookup"><span data-stu-id="15ec9-159">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="15ec9-160">Office 365 教育版中的 Microsoft 团队基于相同的教育 Api，并提供使用案例使用 Api 可以执行的操作。</span><span class="sxs-lookup"><span data-stu-id="15ec9-160">Microsoft Teams in Office 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="15ec9-161">您的应用程序可以使用这些 Api 进行交互的整个生命周期工作分配的工作分配。</span><span class="sxs-lookup"><span data-stu-id="15ec9-161">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="15ec9-162">工作分配 Api 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="15ec9-162">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="15ec9-163">[educationAssignment](educationassignment.md) -分配 API 的核心对象。</span><span class="sxs-lookup"><span data-stu-id="15ec9-163">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="15ec9-164">表示任务或工作分配给类中的学生或团队成员属于其研究单位。</span><span class="sxs-lookup"><span data-stu-id="15ec9-164">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="15ec9-165">[educationSubmission](educationsubmission.md) -表示的资源的个人 （或组） 提交的工作分配关联薪等级和工作分配的反馈。</span><span class="sxs-lookup"><span data-stu-id="15ec9-165">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="15ec9-166">[educationResource](educationresource.md) -表示学习对象，它是被分配或提交。</span><span class="sxs-lookup"><span data-stu-id="15ec9-166">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="15ec9-167">**EducationResource**相关联**educationAssignment**和/或**educationSubmission**。</span><span class="sxs-lookup"><span data-stu-id="15ec9-167">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="15ec9-168">工作分配 Api 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="15ec9-168">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="15ec9-169">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="15ec9-169">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="15ec9-170">发布工作分配</span><span class="sxs-lookup"><span data-stu-id="15ec9-170">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="15ec9-171">创建工作分配资源</span><span class="sxs-lookup"><span data-stu-id="15ec9-171">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="15ec9-172">创建提交资源</span><span class="sxs-lookup"><span data-stu-id="15ec9-172">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="15ec9-173">提交的作业</span><span class="sxs-lookup"><span data-stu-id="15ec9-173">Submit assignment</span></span>](../api/educationsubmission-submit.md) 
- [<span data-ttu-id="15ec9-174">Unsubmit 工作分配</span><span class="sxs-lookup"><span data-stu-id="15ec9-174">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)   
- [<span data-ttu-id="15ec9-175">返回学生薪等级和反馈</span><span class="sxs-lookup"><span data-stu-id="15ec9-175">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md) 
- [<span data-ttu-id="15ec9-176">获取工作分配详细信息</span><span class="sxs-lookup"><span data-stu-id="15ec9-176">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="15ec9-177">以下是一些常见的使用案例工作分配相关教育版 Api。</span><span class="sxs-lookup"><span data-stu-id="15ec9-177">The following are some common use cases for the assignment-related education APIs.</span></span>

|<span data-ttu-id="15ec9-178">用例</span><span class="sxs-lookup"><span data-stu-id="15ec9-178">Use case</span></span>|<span data-ttu-id="15ec9-179">Description</span><span class="sxs-lookup"><span data-stu-id="15ec9-179">Description</span></span>|<span data-ttu-id="15ec9-180">另请参阅</span><span class="sxs-lookup"><span data-stu-id="15ec9-180">See also</span></span>|
|:-------|:----------|:-------|
|<span data-ttu-id="15ec9-181">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="15ec9-181">Create assignments</span></span>|<span data-ttu-id="15ec9-182">外部系统可以创建类的工作分配，并附加到工作分配的资源。</span><span class="sxs-lookup"><span data-stu-id="15ec9-182">An external system can create an assignment for the class and attach resources to the assignment.</span></span>|[<span data-ttu-id="15ec9-183">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="15ec9-183">Create assignment</span></span>](../api/educationassignment-post-resources.md)|
|<span data-ttu-id="15ec9-184">读取工作分配信息</span><span class="sxs-lookup"><span data-stu-id="15ec9-184">Read assignment information</span></span>|<span data-ttu-id="15ec9-185">分析应用程序可以获取有关分配和学生提交，包括多个日期和薪等级的信息。</span><span class="sxs-lookup"><span data-stu-id="15ec9-185">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span>|[<span data-ttu-id="15ec9-186">获取工作分配</span><span class="sxs-lookup"><span data-stu-id="15ec9-186">Get assignment</span></span>](../api/educationassignment-get.md)|
|<span data-ttu-id="15ec9-187">跟踪学生提交</span><span class="sxs-lookup"><span data-stu-id="15ec9-187">Track student submissions</span></span>|<span data-ttu-id="15ec9-188">您的应用程序可以提供的显示多少拾取学生需要进行评分教师仪表板。</span><span class="sxs-lookup"><span data-stu-id="15ec9-188">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>|[<span data-ttu-id="15ec9-189">提交资源</span><span class="sxs-lookup"><span data-stu-id="15ec9-189">Submission resource</span></span>](educationsubmission.md)|

## <a name="school-data-sync-management"></a><span data-ttu-id="15ec9-190">学校数据同步管理</span><span class="sxs-lookup"><span data-stu-id="15ec9-190">School data sync management</span></span>

<span data-ttu-id="15ec9-191">[学校数据同步](https://sds.microsoft.com/)可帮助自动完成的导入和与 Azure Active Directory (Azure AD) 和 Office 365 同步学生信息系统中的名单数据的过程。</span><span class="sxs-lookup"><span data-stu-id="15ec9-191">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="15ec9-192">您可以使用在 Microsoft Graph 学校数据同步管理 Api 设置从 CSV 文件或支持的 SI API 连接器的同步。</span><span class="sxs-lookup"><span data-stu-id="15ec9-192">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="15ec9-193">学校数据同步管理 Api 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="15ec9-193">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="15ec9-194">列表同步配置文件</span><span class="sxs-lookup"><span data-stu-id="15ec9-194">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="15ec9-195">获取同步配置文件</span><span class="sxs-lookup"><span data-stu-id="15ec9-195">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="15ec9-196">创建同步配置文件</span><span class="sxs-lookup"><span data-stu-id="15ec9-196">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="15ec9-197">删除同步配置文件</span><span class="sxs-lookup"><span data-stu-id="15ec9-197">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="15ec9-198">暂停正在进行同步</span><span class="sxs-lookup"><span data-stu-id="15ec9-198">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="15ec9-199">恢复暂停的同步</span><span class="sxs-lookup"><span data-stu-id="15ec9-199">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="15ec9-200">重置 sync</span><span class="sxs-lookup"><span data-stu-id="15ec9-200">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="15ec9-201">启动同步上载文件</span><span class="sxs-lookup"><span data-stu-id="15ec9-201">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) 
- [<span data-ttu-id="15ec9-202">获取一个上载 URL</span><span class="sxs-lookup"><span data-stu-id="15ec9-202">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="15ec9-203">要获取同步的状态</span><span class="sxs-lookup"><span data-stu-id="15ec9-203">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="15ec9-204">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="15ec9-204">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a><span data-ttu-id="15ec9-205">后续步骤</span><span class="sxs-lookup"><span data-stu-id="15ec9-205">Next steps</span></span>
<span data-ttu-id="15ec9-206">使用 Microsoft Graph 教育 Api 构建访问学员和学校名单的教育解决方案。</span><span class="sxs-lookup"><span data-stu-id="15ec9-206">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="15ec9-207">了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="15ec9-207">To learn more:</span></span>

- <span data-ttu-id="15ec9-208">探索对你的方案最有帮助的资源和方法。</span><span class="sxs-lookup"><span data-stu-id="15ec9-208">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="15ec9-209">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。</span><span class="sxs-lookup"><span data-stu-id="15ec9-209">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

