# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="6226c-101">在 Microsoft Graph 中使用教育 API</span><span class="sxs-lookup"><span data-stu-id="6226c-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="6226c-102">Microsoft Graph 中的教育 API 可增强 Office 365 资源和与教育情景（包括学校、学生、教师、课程和注册）相关的信息的数据。</span><span class="sxs-lookup"><span data-stu-id="6226c-102">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, and enrollments.</span></span> <span data-ttu-id="6226c-103">这使你能够轻松地构建与教育资源集成的解决方案。</span><span class="sxs-lookup"><span data-stu-id="6226c-103">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="6226c-104">教育 API 包含名册资源和作业资源，可以使用这些资源与 Microsoft Teams 中的名册服务进行交互。</span><span class="sxs-lookup"><span data-stu-id="6226c-104">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering services in Microsoft Teams.</span></span> <span data-ttu-id="6226c-105">可以使用这些资源来管理学校名册。</span><span class="sxs-lookup"><span data-stu-id="6226c-105">You can use these resources to manage a school roster.</span></span>

## <a name="authorization"></a><span data-ttu-id="6226c-106">授权</span><span class="sxs-lookup"><span data-stu-id="6226c-106">Authorization</span></span>

<span data-ttu-id="6226c-107">若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6226c-107">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="6226c-108">有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](https://developer.microsoft.com/zh-CN/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="6226c-108">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/zh-CN/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="6226c-109">你的应用还需要具有相应的权限。</span><span class="sxs-lookup"><span data-stu-id="6226c-109">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="6226c-110">有关详细信息，请参阅[教育权限](../../../concepts/permissions_reference.md#education-permissions)。</span><span class="sxs-lookup"><span data-stu-id="6226c-110">For more information, see [Microsoft Graph permissions](../../../concepts/permissions_reference.md#education-permissions)</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="6226c-111">请求学校 IT 管理员许可的应用权限</span><span class="sxs-lookup"><span data-stu-id="6226c-111">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="6226c-112">若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。</span><span class="sxs-lookup"><span data-stu-id="6226c-112">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="6226c-113">仅能授权许可一次，除非权限更改。</span><span class="sxs-lookup"><span data-stu-id="6226c-113">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="6226c-114">在管理员许可后，就会为租户中的所有用户预配应用。</span><span class="sxs-lookup"><span data-stu-id="6226c-114">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="6226c-115">若要显示许可对话框，请执行以下 REST 调用。</span><span class="sxs-lookup"><span data-stu-id="6226c-115">To show a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="6226c-116">参数</span><span class="sxs-lookup"><span data-stu-id="6226c-116">Parameter</span></span>|<span data-ttu-id="6226c-117">说明</span><span class="sxs-lookup"><span data-stu-id="6226c-117">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="6226c-118">Tenant</span><span class="sxs-lookup"><span data-stu-id="6226c-118">Tenant</span></span>|<span data-ttu-id="6226c-119">学校的租户 ID。</span><span class="sxs-lookup"><span data-stu-id="6226c-119">Tenant ID of the school.</span></span> <span data-ttu-id="6226c-120">使用完整 ID，其中包含 onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="6226c-120">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="6226c-121">clientId</span><span class="sxs-lookup"><span data-stu-id="6226c-121">client_id</span></span>|<span data-ttu-id="6226c-122">应用的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="6226c-122">Client ID - the app ID</span></span>|
|<span data-ttu-id="6226c-123">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="6226c-123">redirectUrl</span></span>|<span data-ttu-id="6226c-124">应用重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="6226c-124">App redirect URL</span></span>|


## <a name="rostering"></a><span data-ttu-id="6226c-125">Rostering</span><span class="sxs-lookup"><span data-stu-id="6226c-125">Rostering</span></span>

<span data-ttu-id="6226c-126">借助名册 API，可以从学校的 Office 365 租户（预配了 [Microsoft 学校数据同步](https://sds.microsoft.com/)）中提取数据。这些 API 提供对有关学校、部门、教师、学生和名册的信息的访问权限。</span><span class="sxs-lookup"><span data-stu-id="6226c-126">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="6226c-127">API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。</span><span class="sxs-lookup"><span data-stu-id="6226c-127">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="6226c-128">支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。</span><span class="sxs-lookup"><span data-stu-id="6226c-128">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="6226c-129">这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。</span><span class="sxs-lookup"><span data-stu-id="6226c-129">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="6226c-130">此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。</span><span class="sxs-lookup"><span data-stu-id="6226c-130">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="6226c-131">可以使用名册 API 让应用用户了解：</span><span class="sxs-lookup"><span data-stu-id="6226c-131">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="6226c-132">我是谁</span><span class="sxs-lookup"><span data-stu-id="6226c-132">Who I am</span></span>
- <span data-ttu-id="6226c-133">我参加或教学的课程</span><span class="sxs-lookup"><span data-stu-id="6226c-133">What classes I attend or teach</span></span>
- <span data-ttu-id="6226c-134">我需要做什么以及完成时间</span><span class="sxs-lookup"><span data-stu-id="6226c-134">What I need to do and by when</span></span>

<span data-ttu-id="6226c-135">名册 API 提供以下关键资源：</span><span class="sxs-lookup"><span data-stu-id="6226c-135">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="6226c-136">[educationSchool](educationschool.md) - 表示学校。</span><span class="sxs-lookup"><span data-stu-id="6226c-136">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="6226c-137">[educationClass](educationclass.md) - 表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="6226c-137">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="6226c-138">[educationTerm](educationterm.md) - 表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="6226c-138">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="6226c-139">[educationTeacher](educationteacher.md) - 表示主要角色为“教师”的用户。</span><span class="sxs-lookup"><span data-stu-id="6226c-139">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="6226c-140">[educationStudent](educationstudent.md) - 表示主要角色为“学生”的用户。</span><span class="sxs-lookup"><span data-stu-id="6226c-140">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="6226c-141">名册 API 支持以下方案：</span><span class="sxs-lookup"><span data-stu-id="6226c-141">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="6226c-142">列出所有学校</span><span class="sxs-lookup"><span data-stu-id="6226c-142">List all schools</span></span>](../api/educationroot_list_schools.md) 
- [<span data-ttu-id="6226c-143">列出所教授课程的学校</span><span class="sxs-lookup"><span data-stu-id="6226c-143">List schools in which a class is taught</span></span>](../api/educationclass_list_schools.md)
- [<span data-ttu-id="6226c-144">为用户列出学校</span><span class="sxs-lookup"><span data-stu-id="6226c-144">List schools for a user</span></span>](../api/educationuser_list_schools.md)
- [<span data-ttu-id="6226c-145">获取所有课程</span><span class="sxs-lookup"><span data-stu-id="6226c-145">Get all classes</span></span>](../api/educationroot_list_classes.md )
- [<span data-ttu-id="6226c-146">获取学校的课程</span><span class="sxs-lookup"><span data-stu-id="6226c-146">Get classes in a school</span></span>](../api/educationschool_list_classes.md)
- [<span data-ttu-id="6226c-147">为用户列出课程</span><span class="sxs-lookup"><span data-stu-id="6226c-147">List classes for a user</span></span>](../api/educationuser_list_classes.md)
- [<span data-ttu-id="6226c-148">将课程添加到学校</span><span class="sxs-lookup"><span data-stu-id="6226c-148">Add classes to a school</span></span>](../api/educationschool_post_classes.md)
- [<span data-ttu-id="6226c-149">获取课程的学生和教师</span><span class="sxs-lookup"><span data-stu-id="6226c-149">Get students and teachers for a class</span></span>](../api/educationclass_list_members.md)
- [<span data-ttu-id="6226c-150">将成员添加到课程</span><span class="sxs-lookup"><span data-stu-id="6226c-150">Add members to a class</span></span>](../api/educationclass_post_members.md) 
- [<span data-ttu-id="6226c-151">列出课程的教师</span><span class="sxs-lookup"><span data-stu-id="6226c-151">List teachers for a class</span></span>](../api/educationclass_list_teachers.md)
- [<span data-ttu-id="6226c-152">获取学校的用户</span><span class="sxs-lookup"><span data-stu-id="6226c-152">Get users in a school</span></span>](../api/educationschool_list_users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="next-steps"></a><span data-ttu-id="6226c-153">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6226c-153">Next steps</span></span>
<span data-ttu-id="6226c-154">使用 Microsoft Graph 教育 API 构建访问学校名册的教育解决方案。</span><span class="sxs-lookup"><span data-stu-id="6226c-154">Use the Microsoft Graph education APIs to build education solutions that access school rosters.</span></span> <span data-ttu-id="6226c-155">了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="6226c-155">To learn more:</span></span>

- <span data-ttu-id="6226c-156">探索对你的方案最有帮助的资源和方法。</span><span class="sxs-lookup"><span data-stu-id="6226c-156">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="6226c-157">尝试在 [Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)中使用 API。</span><span class="sxs-lookup"><span data-stu-id="6226c-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/zh-CN/graph/graph-explorer).</span></span>

