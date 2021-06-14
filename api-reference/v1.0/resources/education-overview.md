---
title: 在 Microsoft Graph 中使用教育 API
description: Microsoft Graph 中的教育 API 可增强 Microsoft 365 资源和与教育情景（包括学校、学生、教师、课程和注册）相关的信息的数据。 这使你能够轻松地构建与教育资源集成的解决方案。
localization_priority: Priority
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: f0959157ac4f436fe47aa0164cfb4a8fb91b086b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911298"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="eae47-104">在 Microsoft Graph 中使用教育 API</span><span class="sxs-lookup"><span data-stu-id="eae47-104">Working with education APIs in Microsoft Graph</span></span>

<span data-ttu-id="eae47-105">Microsoft Graph 中的教育 API 可增强 Microsoft 365 资源和与教育情景（包括学校、学生、教师、课程和注册）相关的信息的数据。</span><span class="sxs-lookup"><span data-stu-id="eae47-105">The education APIs in Microsoft Graph enhance Microsoft 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, and enrollments.</span></span> <span data-ttu-id="eae47-106">这使你能够轻松地构建与教育资源集成的解决方案。</span><span class="sxs-lookup"><span data-stu-id="eae47-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="eae47-p103">教育 API 包含名单资源和作业资源，可用于与 Microsoft Teams 中的名单服务进行交互。可以使用这些资源管理学校名单。</span><span class="sxs-lookup"><span data-stu-id="eae47-p103">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering services in Microsoft Teams. You can use these resources to manage a school roster.</span></span>

## <a name="authorization"></a><span data-ttu-id="eae47-109">授权</span><span class="sxs-lookup"><span data-stu-id="eae47-109">Authorization</span></span>

<span data-ttu-id="eae47-110">若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="eae47-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="eae47-111">有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](/graph/auth/)。</span><span class="sxs-lookup"><span data-stu-id="eae47-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span> <span data-ttu-id="eae47-112">你的应用还需要具有相应的权限。</span><span class="sxs-lookup"><span data-stu-id="eae47-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="eae47-113">有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。</span><span class="sxs-lookup"><span data-stu-id="eae47-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span>

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="eae47-114">请求学校 IT 管理员许可的应用权限</span><span class="sxs-lookup"><span data-stu-id="eae47-114">App permissions to enable school IT admins to consent</span></span>

<span data-ttu-id="eae47-115">若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。</span><span class="sxs-lookup"><span data-stu-id="eae47-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="eae47-116">仅能授权许可一次，除非权限更改。</span><span class="sxs-lookup"><span data-stu-id="eae47-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="eae47-117">在管理员许可后，就会为租户中的所有用户预配应用。</span><span class="sxs-lookup"><span data-stu-id="eae47-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="eae47-118">若要显示许可对话框，请执行以下 REST 调用。</span><span class="sxs-lookup"><span data-stu-id="eae47-118">To show a consent dialog box, use the following REST call.</span></span>

```http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| <span data-ttu-id="eae47-119">参数</span><span class="sxs-lookup"><span data-stu-id="eae47-119">Parameter</span></span>   | <span data-ttu-id="eae47-120">说明</span><span class="sxs-lookup"><span data-stu-id="eae47-120">Description</span></span>                                                               |
| :---------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="eae47-121">Tenant</span><span class="sxs-lookup"><span data-stu-id="eae47-121">Tenant</span></span>      | <span data-ttu-id="eae47-122">学校的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="eae47-122">Tenant ID of the school.</span></span> <span data-ttu-id="eae47-123">使用完整 ID，其中包含 onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="eae47-123">Use the full ID, which includes onmicrosoft.com.</span></span> |
| <span data-ttu-id="eae47-124">clientId</span><span class="sxs-lookup"><span data-stu-id="eae47-124">clientId</span></span>    | <span data-ttu-id="eae47-125">应用的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="eae47-125">Client ID of the app.</span></span>                                                     |
| <span data-ttu-id="eae47-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="eae47-126">redirectUrl</span></span> | <span data-ttu-id="eae47-127">应用重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="eae47-127">App redirect URL.</span></span>                                                         |

## <a name="rostering"></a><span data-ttu-id="eae47-128">Rostering</span><span class="sxs-lookup"><span data-stu-id="eae47-128">Rostering</span></span>

<span data-ttu-id="eae47-129">借助名册 API，可以从学校的 Microsoft 365 租户（预配了 [Microsoft 学校数据同步](https://sds.microsoft.com/)）中提取数据。这些 API 提供对有关学校、部门、教师、学生和名册的信息的访问权限。</span><span class="sxs-lookup"><span data-stu-id="eae47-129">The rostering APIs enable you to extract data from a school's Microsoft 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="eae47-130">API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。</span><span class="sxs-lookup"><span data-stu-id="eae47-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="eae47-131">支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。</span><span class="sxs-lookup"><span data-stu-id="eae47-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="eae47-132">这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。</span><span class="sxs-lookup"><span data-stu-id="eae47-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="eae47-133">此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。</span><span class="sxs-lookup"><span data-stu-id="eae47-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="eae47-134">可以使用名册 API 让应用用户了解：</span><span class="sxs-lookup"><span data-stu-id="eae47-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="eae47-135">我是谁</span><span class="sxs-lookup"><span data-stu-id="eae47-135">Who I am</span></span>
- <span data-ttu-id="eae47-136">我参加或教学的课程</span><span class="sxs-lookup"><span data-stu-id="eae47-136">What classes I attend or teach</span></span>
- <span data-ttu-id="eae47-137">我需要做什么以及完成时间</span><span class="sxs-lookup"><span data-stu-id="eae47-137">What I need to do and by when</span></span>

<span data-ttu-id="eae47-138">名册 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="eae47-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="eae47-139">[educationSchool](educationschool.md) - 表示学校。</span><span class="sxs-lookup"><span data-stu-id="eae47-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="eae47-140">[educationClass](educationclass.md) - 表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="eae47-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="eae47-141">[educationTerm](educationterm.md) - 表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="eae47-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="eae47-142">[educationTeacher](educationteacher.md) - 表示主要角色为“教师”的用户。</span><span class="sxs-lookup"><span data-stu-id="eae47-142">[educationTeacher](educationteacher.md) - Represents a user with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="eae47-143">[educationStudent](educationstudent.md) - 表示主要角色为“学生”的用户。</span><span class="sxs-lookup"><span data-stu-id="eae47-143">[educationStudent](educationstudent.md) - Represents a user with the primary role of 'student'.</span></span>

<span data-ttu-id="eae47-144">名册 API 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="eae47-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="eae47-145">列出所有学校</span><span class="sxs-lookup"><span data-stu-id="eae47-145">List all schools</span></span>](../api/educationschool-list.md)
- [<span data-ttu-id="eae47-146">列出所教授课程的学校</span><span class="sxs-lookup"><span data-stu-id="eae47-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="eae47-147">为用户列出学校</span><span class="sxs-lookup"><span data-stu-id="eae47-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="eae47-148">获取所有课程</span><span class="sxs-lookup"><span data-stu-id="eae47-148">Get all classes</span></span>](../api/educationclass-list.md)
- [<span data-ttu-id="eae47-149">获取学校的课程</span><span class="sxs-lookup"><span data-stu-id="eae47-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="eae47-150">为用户列出课程</span><span class="sxs-lookup"><span data-stu-id="eae47-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="eae47-151">将课程添加到学校</span><span class="sxs-lookup"><span data-stu-id="eae47-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="eae47-152">获取课程的学生和教师</span><span class="sxs-lookup"><span data-stu-id="eae47-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="eae47-153">将成员添加到课程</span><span class="sxs-lookup"><span data-stu-id="eae47-153">Add members to a class</span></span>](../api/educationclass-post-members.md)
- [<span data-ttu-id="eae47-154">列出课程的教师</span><span class="sxs-lookup"><span data-stu-id="eae47-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="eae47-155">获取学校的用户</span><span class="sxs-lookup"><span data-stu-id="eae47-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="eae47-156">作业</span><span class="sxs-lookup"><span data-stu-id="eae47-156">Assignments</span></span>

<span data-ttu-id="eae47-157">可以使用与作业相关的教育 API 与 Microsoft Teams 中的作业集成。</span><span class="sxs-lookup"><span data-stu-id="eae47-157">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="eae47-158">Microsoft 365 教育版中的 Microsoft Teams 基于同一教育 API，并提供了使用 API 执行哪些操作的用例。</span><span class="sxs-lookup"><span data-stu-id="eae47-158">Microsoft Teams in Microsoft 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="eae47-159">应用可以使用这些 API 在整个作业生命周期内与作业进行交互。</span><span class="sxs-lookup"><span data-stu-id="eae47-159">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="eae47-160">作业 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="eae47-160">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="eae47-161">[educationAssignment](educationassignment.md) - 作业 API 的核心对象。</span><span class="sxs-lookup"><span data-stu-id="eae47-161">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="eae47-162">是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。</span><span class="sxs-lookup"><span data-stu-id="eae47-162">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="eae47-163">[educationSubmission](educationsubmission.md) - 是指个人（或组）提交作业的资源以及该作业的相关成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="eae47-163">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="eae47-164">[educationResource](educationresource.md) - 是指正在分配或提交的学习对象。</span><span class="sxs-lookup"><span data-stu-id="eae47-164">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="eae47-165">**educationResource** 与 **educationAssignment** 和/或 **educationSubmission** 相关联。</span><span class="sxs-lookup"><span data-stu-id="eae47-165">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="eae47-166">作业 API 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="eae47-166">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="eae47-167">创建作业</span><span class="sxs-lookup"><span data-stu-id="eae47-167">Create assignment</span></span>](../api/educationclass-post-assignment.md)
- [<span data-ttu-id="eae47-168">发布作业</span><span class="sxs-lookup"><span data-stu-id="eae47-168">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="eae47-169">创建作业资源</span><span class="sxs-lookup"><span data-stu-id="eae47-169">Create assignment resource</span></span>](../api/educationassignment-post-resource.md)
- [<span data-ttu-id="eae47-170">创建提交资源</span><span class="sxs-lookup"><span data-stu-id="eae47-170">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="eae47-171">提交作业</span><span class="sxs-lookup"><span data-stu-id="eae47-171">Submit assignment</span></span>](../api/educationsubmission-submit.md)
- [<span data-ttu-id="eae47-172">取消提交作业</span><span class="sxs-lookup"><span data-stu-id="eae47-172">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)
- [<span data-ttu-id="eae47-173">将成绩和反馈返回给学生</span><span class="sxs-lookup"><span data-stu-id="eae47-173">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md)
- [<span data-ttu-id="eae47-174">获取作业详细信息</span><span class="sxs-lookup"><span data-stu-id="eae47-174">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="eae47-175">以下是与作业相关的教育 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="eae47-175">The following are some common use cases for the assignment-related education APIs.</span></span>

| <span data-ttu-id="eae47-176">用例</span><span class="sxs-lookup"><span data-stu-id="eae47-176">Use case</span></span>                    | <span data-ttu-id="eae47-177">说明</span><span class="sxs-lookup"><span data-stu-id="eae47-177">Description</span></span>                                                                                                         | <span data-ttu-id="eae47-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eae47-178">See also</span></span>                                                          |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------- |
| <span data-ttu-id="eae47-179">创建作业</span><span class="sxs-lookup"><span data-stu-id="eae47-179">Create assignments</span></span>          | <span data-ttu-id="eae47-180">外部系统可以创建课堂作业并将资源附加到作业。</span><span class="sxs-lookup"><span data-stu-id="eae47-180">An external system can create an assignment for the class and attach resources to the assignment.</span></span>                   | [<span data-ttu-id="eae47-181">创建作业</span><span class="sxs-lookup"><span data-stu-id="eae47-181">Create assignment</span></span>](../api/educationassignment-post-resource.md) |
| <span data-ttu-id="eae47-182">阅读作业信息</span><span class="sxs-lookup"><span data-stu-id="eae47-182">Read assignment information</span></span> | <span data-ttu-id="eae47-183">分析应用可以获取有关作业和学生提交（包括日期和成绩）的信息。</span><span class="sxs-lookup"><span data-stu-id="eae47-183">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span> | [<span data-ttu-id="eae47-184">获取作业</span><span class="sxs-lookup"><span data-stu-id="eae47-184">Get assignment</span></span>](../api/educationassignment-get.md)               |
| <span data-ttu-id="eae47-185">跟踪学生作业提交</span><span class="sxs-lookup"><span data-stu-id="eae47-185">Track student submissions</span></span>   | <span data-ttu-id="eae47-186">应用可为教师提供仪表板，显示有多少学生提交的作业需要评分。</span><span class="sxs-lookup"><span data-stu-id="eae47-186">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>           | [<span data-ttu-id="eae47-187">提交资源</span><span class="sxs-lookup"><span data-stu-id="eae47-187">Submission resource</span></span>](educationsubmission.md)                     |

## <a name="whats-new"></a><span data-ttu-id="eae47-188">最近更新</span><span class="sxs-lookup"><span data-stu-id="eae47-188">What's new</span></span>

<span data-ttu-id="eae47-189">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="eae47-189">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eae47-190">后续步骤</span><span class="sxs-lookup"><span data-stu-id="eae47-190">Next steps</span></span>

<span data-ttu-id="eae47-p111">使用 Microsoft Graph 教育 API 构建访问学校名单的教育解决方案。若要了解详细信息，请：</span><span class="sxs-lookup"><span data-stu-id="eae47-p111">Use the Microsoft Graph education APIs to build education solutions that access school rosters. To learn more:</span></span>

- <span data-ttu-id="eae47-193">探索对你的方案最有帮助的资源和方法。</span><span class="sxs-lookup"><span data-stu-id="eae47-193">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="eae47-194">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。</span><span class="sxs-lookup"><span data-stu-id="eae47-194">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
