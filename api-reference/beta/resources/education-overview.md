---
title: 在 Microsoft Graph 中使用教育 API
description: Microsoft Graph 中的教育 Api 使用与教育方案相关的信息（包括学校、学生、教师、课程、注册和工作分配）来增强 Microsoft 365 的资源和数据。 这使你能够轻松地构建与教育资源集成的解决方案。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 6169037891c4f54a75e4cd1f6b07053a099d5766
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055713"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="4e6f8-104">在 Microsoft Graph 中使用教育 API</span><span class="sxs-lookup"><span data-stu-id="4e6f8-104">Working with education APIs in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6f8-105">Microsoft Graph 中的教育 Api 使用与教育方案相关的信息（包括学校、学生、教师、课程、注册和工作分配）来增强 Microsoft 365 的资源和数据。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-105">The education APIs in Microsoft Graph enhance Microsoft 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="4e6f8-106">这使你能够轻松地构建与教育资源集成的解决方案。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="4e6f8-107">教育 Api 包括名册资源和工作分配资源，您可以使用这些资源与 Microsoft 团队中的名册和工作分配服务进行交互。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="4e6f8-108">您可以使用这些资源管理学校名单并自动完成学生作业。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-108">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="4e6f8-109">授权</span><span class="sxs-lookup"><span data-stu-id="4e6f8-109">Authorization</span></span>

<span data-ttu-id="4e6f8-110">若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="4e6f8-111">有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="4e6f8-112">你的应用还需要具有相应的权限。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="4e6f8-113">有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span>

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="4e6f8-114">请求学校 IT 管理员许可的应用权限</span><span class="sxs-lookup"><span data-stu-id="4e6f8-114">App permissions to enable school IT admins to consent</span></span>

<span data-ttu-id="4e6f8-115">若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="4e6f8-116">仅能授权许可一次，除非权限更改。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="4e6f8-117">在管理员许可后，就会为租户中的所有用户预配应用。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="4e6f8-118">若要触发许可对话框，请使用以下 REST 调用。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-118">To trigger a consent dialog box, use the following REST call.</span></span>

```http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| <span data-ttu-id="4e6f8-119">参数</span><span class="sxs-lookup"><span data-stu-id="4e6f8-119">Parameter</span></span>   | <span data-ttu-id="4e6f8-120">说明</span><span class="sxs-lookup"><span data-stu-id="4e6f8-120">Description</span></span>                                                               |
| :---------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="4e6f8-121">Tenant</span><span class="sxs-lookup"><span data-stu-id="4e6f8-121">Tenant</span></span>      | <span data-ttu-id="4e6f8-122">学校的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-122">Tenant ID of the school.</span></span> <span data-ttu-id="4e6f8-123">使用完整 ID，其中包含 onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-123">Use the full ID, which includes onmicrosoft.com.</span></span> |
| <span data-ttu-id="4e6f8-124">clientId</span><span class="sxs-lookup"><span data-stu-id="4e6f8-124">clientId</span></span>    | <span data-ttu-id="4e6f8-125">应用的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-125">Client ID of the app.</span></span>                                                     |
| <span data-ttu-id="4e6f8-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="4e6f8-126">redirectUrl</span></span> | <span data-ttu-id="4e6f8-127">应用重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-127">App redirect URL.</span></span>                                                         |

## <a name="rostering"></a><span data-ttu-id="4e6f8-128">Rostering</span><span class="sxs-lookup"><span data-stu-id="4e6f8-128">Rostering</span></span>

<span data-ttu-id="4e6f8-129">通过名册 Api，你可以从学校的 Microsoft 365 租户（使用 [Microsoft School Data Sync](https://sds.microsoft.com/)预配）中提取数据。这些 Api 提供了对学校、节、教师、学生和名册的信息的访问。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-129">The rostering APIs enable you to extract data from a school's Microsoft 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="4e6f8-130">API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="4e6f8-131">支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="4e6f8-132">这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="4e6f8-133">此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="4e6f8-134">可以使用名册 API 让应用用户了解：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="4e6f8-135">我是谁</span><span class="sxs-lookup"><span data-stu-id="4e6f8-135">Who I am</span></span>
- <span data-ttu-id="4e6f8-136">我参加或教学的课程</span><span class="sxs-lookup"><span data-stu-id="4e6f8-136">What classes I attend or teach</span></span>
- <span data-ttu-id="4e6f8-137">我需要做什么以及完成时间</span><span class="sxs-lookup"><span data-stu-id="4e6f8-137">What I need to do and by when</span></span>

<span data-ttu-id="4e6f8-138">名册 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="4e6f8-139">[educationSchool](educationschool.md) - 表示学校。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="4e6f8-140">[educationClass](educationclass.md) - 表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="4e6f8-141">[educationTerm](educationterm.md) - 表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="4e6f8-142">[educationTeacher](educationteacher.md) - 表示主要角色为“教师”的用户。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="4e6f8-143">[educationStudent](educationstudent.md) - 表示主要角色为“学生”的用户。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="4e6f8-144">名册 API 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="4e6f8-145">列出所有学校</span><span class="sxs-lookup"><span data-stu-id="4e6f8-145">List all schools</span></span>](../api/educationroot-list-schools.md)
- [<span data-ttu-id="4e6f8-146">列出所教授课程的学校</span><span class="sxs-lookup"><span data-stu-id="4e6f8-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="4e6f8-147">为用户列出学校</span><span class="sxs-lookup"><span data-stu-id="4e6f8-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="4e6f8-148">获取所有课程</span><span class="sxs-lookup"><span data-stu-id="4e6f8-148">Get all classes</span></span>](../api/educationroot-list-classes.md)
- [<span data-ttu-id="4e6f8-149">获取学校的课程</span><span class="sxs-lookup"><span data-stu-id="4e6f8-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="4e6f8-150">为用户列出课程</span><span class="sxs-lookup"><span data-stu-id="4e6f8-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="4e6f8-151">将课程添加到学校</span><span class="sxs-lookup"><span data-stu-id="4e6f8-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="4e6f8-152">获取课程的学生和教师</span><span class="sxs-lookup"><span data-stu-id="4e6f8-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="4e6f8-153">将成员添加到课程</span><span class="sxs-lookup"><span data-stu-id="4e6f8-153">Add members to a class</span></span>](../api/educationclass-post-members.md)
- [<span data-ttu-id="4e6f8-154">列出课程的教师</span><span class="sxs-lookup"><span data-stu-id="4e6f8-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="4e6f8-155">获取学校的用户</span><span class="sxs-lookup"><span data-stu-id="4e6f8-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="4e6f8-156">作业</span><span class="sxs-lookup"><span data-stu-id="4e6f8-156">Assignments</span></span>

<span data-ttu-id="4e6f8-157">您可以使用与工作分配相关的教育 Api 与 Microsoft 团队中的工作分配集成。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-157">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="4e6f8-158">Microsoft 365 for 教育版的 microsoft 团队基于相同的教育 Api，并为使用 Api 时可以执行的操作提供了一个用例。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-158">Microsoft Teams in Microsoft 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="4e6f8-159">您的应用程序可以使用这些 Api 与工作分配生命周期中的工作分配进行交互。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-159">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="4e6f8-160">分配 Api 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-160">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="4e6f8-161">[educationAssignment](educationassignment.md) -工作分配 API 的核心对象。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-161">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="4e6f8-162">表示分配给课程中的学生或团队成员的任务或工作单元，作为其研究的一部分。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-162">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="4e6f8-163">[educationSubmission](educationsubmission.md) -表示单个 (或组) 为工作分配提交的资源，以及该工作分配的相关评分和反馈。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-163">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="4e6f8-164">[educationResource](educationresource.md) -表示要分配或提交的学习对象。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-164">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="4e6f8-165">**EducationResource**与**educationAssignment**和/或**educationSubmission**相关联。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-165">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="4e6f8-166">分配 Api 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-166">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="4e6f8-167">创建作业</span><span class="sxs-lookup"><span data-stu-id="4e6f8-167">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="4e6f8-168">发布作业</span><span class="sxs-lookup"><span data-stu-id="4e6f8-168">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="4e6f8-169">创建作业资源</span><span class="sxs-lookup"><span data-stu-id="4e6f8-169">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="4e6f8-170">创建提交资源</span><span class="sxs-lookup"><span data-stu-id="4e6f8-170">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="4e6f8-171">提交分配</span><span class="sxs-lookup"><span data-stu-id="4e6f8-171">Submit assignment</span></span>](../api/educationsubmission-submit.md)
- [<span data-ttu-id="4e6f8-172">Unsubmit 分配</span><span class="sxs-lookup"><span data-stu-id="4e6f8-172">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)
- [<span data-ttu-id="4e6f8-173">将成绩和反馈返回给学生</span><span class="sxs-lookup"><span data-stu-id="4e6f8-173">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md)
- [<span data-ttu-id="4e6f8-174">获取工作分配详细信息</span><span class="sxs-lookup"><span data-stu-id="4e6f8-174">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="4e6f8-175">以下是与工作分配相关的教育 Api 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-175">The following are some common use cases for the assignment-related education APIs.</span></span>

| <span data-ttu-id="4e6f8-176">用例</span><span class="sxs-lookup"><span data-stu-id="4e6f8-176">Use case</span></span>                    | <span data-ttu-id="4e6f8-177">说明</span><span class="sxs-lookup"><span data-stu-id="4e6f8-177">Description</span></span>                                                                                                         | <span data-ttu-id="4e6f8-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4e6f8-178">See also</span></span>                                                          |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------- |
| <span data-ttu-id="4e6f8-179">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="4e6f8-179">Create assignments</span></span>          | <span data-ttu-id="4e6f8-180">外部系统可以为类创建分配并将资源附加到工作分配。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-180">An external system can create an assignment for the class and attach resources to the assignment.</span></span>                   | [<span data-ttu-id="4e6f8-181">创建作业</span><span class="sxs-lookup"><span data-stu-id="4e6f8-181">Create assignment</span></span>](../api/educationassignment-post-resources.md) |
| <span data-ttu-id="4e6f8-182">读取工作分配信息</span><span class="sxs-lookup"><span data-stu-id="4e6f8-182">Read assignment information</span></span> | <span data-ttu-id="4e6f8-183">分析应用程序可以获取有关工作分配和学生提交的信息，包括日期和成绩。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-183">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span> | [<span data-ttu-id="4e6f8-184">获取作业</span><span class="sxs-lookup"><span data-stu-id="4e6f8-184">Get assignment</span></span>](../api/educationassignment-get.md)               |
| <span data-ttu-id="4e6f8-185">跟踪学生提交</span><span class="sxs-lookup"><span data-stu-id="4e6f8-185">Track student submissions</span></span>   | <span data-ttu-id="4e6f8-186">您的应用程序可以提供一个教师仪表板，以显示学生的提交次数需要进行评分。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-186">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>           | [<span data-ttu-id="4e6f8-187">提交资源</span><span class="sxs-lookup"><span data-stu-id="4e6f8-187">Submission resource</span></span>](educationsubmission.md)                     |

## <a name="school-data-sync-management"></a><span data-ttu-id="4e6f8-188">学校数据同步管理</span><span class="sxs-lookup"><span data-stu-id="4e6f8-188">School data sync management</span></span>

<span data-ttu-id="4e6f8-189">[学校数据同步](https://sds.microsoft.com/) 可帮助您自动执行从学生信息系统中导入和同步名单数据的过程，该过程与 Azure Active Directory (azure AD) 和 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-189">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Microsoft 365.</span></span> <span data-ttu-id="4e6f8-190">您可以使用 Microsoft Graph 中的学校数据同步管理 Api 设置 CSV 文件或受支持的 SIS API 连接器的同步。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-190">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="4e6f8-191">学校数据同步管理 Api 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-191">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="4e6f8-192">列出同步配置文件</span><span class="sxs-lookup"><span data-stu-id="4e6f8-192">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="4e6f8-193">获取同步配置文件</span><span class="sxs-lookup"><span data-stu-id="4e6f8-193">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="4e6f8-194">创建同步配置文件</span><span class="sxs-lookup"><span data-stu-id="4e6f8-194">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="4e6f8-195">删除同步配置文件</span><span class="sxs-lookup"><span data-stu-id="4e6f8-195">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="4e6f8-196">暂停正在进行的同步</span><span class="sxs-lookup"><span data-stu-id="4e6f8-196">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="4e6f8-197">恢复暂停的同步</span><span class="sxs-lookup"><span data-stu-id="4e6f8-197">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="4e6f8-198">重置同步</span><span class="sxs-lookup"><span data-stu-id="4e6f8-198">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="4e6f8-199">开始同步上载的文件</span><span class="sxs-lookup"><span data-stu-id="4e6f8-199">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md)
- [<span data-ttu-id="4e6f8-200">获取上载 URL</span><span class="sxs-lookup"><span data-stu-id="4e6f8-200">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="4e6f8-201">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="4e6f8-201">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="4e6f8-202">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="4e6f8-202">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)

## <a name="whats-new"></a><span data-ttu-id="4e6f8-203">最近更新</span><span class="sxs-lookup"><span data-stu-id="4e6f8-203">What's new</span></span>

<span data-ttu-id="4e6f8-204">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-204">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4e6f8-205">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4e6f8-205">Next steps</span></span>

<span data-ttu-id="4e6f8-206">使用 Microsoft Graph 教育 Api 生成可访问学生工作分配和学校名册的教育解决方案。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-206">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="4e6f8-207">了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="4e6f8-207">To learn more:</span></span>

- <span data-ttu-id="4e6f8-208">探索对你的方案最有帮助的资源和方法。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-208">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="4e6f8-209">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。</span><span class="sxs-lookup"><span data-stu-id="4e6f8-209">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


