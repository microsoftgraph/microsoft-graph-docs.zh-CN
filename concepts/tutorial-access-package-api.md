---
title: 教程：使用 Microsoft Graph Api 创建访问包
description: 了解如何创建访问包并请求使用 Microsoft Graph Api 对其进行访问。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c276289b4e71c96386afd7e2502021249025965b
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288838"
---
# <a name="tutorial-create-an-access-package-using-microsoft-graph-apis"></a><span data-ttu-id="486c3-103">教程：使用 Microsoft Graph Api 创建访问包</span><span class="sxs-lookup"><span data-stu-id="486c3-103">Tutorial: Create an access package using Microsoft Graph APIs</span></span>

<span data-ttu-id="486c3-104">管理对员工所需的所有资源（如组、应用程序和网站）的访问是组织的重要功能。</span><span class="sxs-lookup"><span data-stu-id="486c3-104">Managing access to all the resources that employees need, such as groups, applications, and sites, is an important function for organizations.</span></span> <span data-ttu-id="486c3-105">您希望向员工授予适当级别的访问权限，以提高其生产效率，并在不再需要时删除他们的访问权限。</span><span class="sxs-lookup"><span data-stu-id="486c3-105">You want to grant employees the right level of access they need to be productive and remove their access when it is no longer needed.</span></span> <span data-ttu-id="486c3-106">[Azure Active Directory (AZURE AD) ](/azure/active-directory/governance/entitlement-management-overview) 使用 Microsoft Graph api 的权限管理使您能够管理此类型的访问。</span><span class="sxs-lookup"><span data-stu-id="486c3-106">[Azure Active Directory (Azure AD) entitlement management](/azure/active-directory/governance/entitlement-management-overview) using Microsoft Graph APIs enables you to manage this type of access.</span></span>

<span data-ttu-id="486c3-107">在本教程中，系统将要求您开发代码，以创建市场营销活动的资源包，内部用户可以提供自助服务请求。</span><span class="sxs-lookup"><span data-stu-id="486c3-107">In this tutorial, you've been asked to develop code to create a package of resources for a marketing campaign that internal users can self-service request.</span></span> <span data-ttu-id="486c3-108">请求不需要审批，用户的访问将在30天后过期。</span><span class="sxs-lookup"><span data-stu-id="486c3-108">Requests do not require approval and user's access expires after 30 days.</span></span> <span data-ttu-id="486c3-109">对于本教程，市场营销活动资源只是单个组中的成员身份，但可以是组、应用程序或 SharePoint Online 网站的集合。</span><span class="sxs-lookup"><span data-stu-id="486c3-109">For this tutorial, the marketing campaign resources are just membership in a single group, but it could be a collection of groups, applications, or SharePoint Online sites.</span></span>

><span data-ttu-id="486c3-110">**注意：** 为了提高可读性，此教程中显示的响应对象可能会缩短。</span><span class="sxs-lookup"><span data-stu-id="486c3-110">**Note:** The response objects shown in this tutorial might be shortened for readability.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="486c3-111">先决条件</span><span class="sxs-lookup"><span data-stu-id="486c3-111">Prerequisites</span></span>

<span data-ttu-id="486c3-112">若要成功完成本教程，请确保您具有所需的先决条件：</span><span class="sxs-lookup"><span data-stu-id="486c3-112">To successfully complete this tutorial, make sure that you have the required prerequisites:</span></span>
- <span data-ttu-id="486c3-113">Azure AD 权限管理需要特定的许可证。</span><span class="sxs-lookup"><span data-stu-id="486c3-113">Azure AD entitlement management requires specific licenses.</span></span> <span data-ttu-id="486c3-114">有关详细信息，请参阅 [许可证要求](/azure/active-directory/governance/entitlement-management-overview#license-requirements)。</span><span class="sxs-lookup"><span data-stu-id="486c3-114">For more information, see [License requirements](/azure/active-directory/governance/entitlement-management-overview#license-requirements).</span></span> <span data-ttu-id="486c3-115">你的租户中需要以下许可证：</span><span class="sxs-lookup"><span data-stu-id="486c3-115">The following licenses are required in your tenant:</span></span>
    - <span data-ttu-id="486c3-116">Azure AD 高级 P2</span><span class="sxs-lookup"><span data-stu-id="486c3-116">Azure AD Premium P2</span></span>
    - <span data-ttu-id="486c3-117">企业移动性 + 安全性 (EMS) E5 许可证</span><span class="sxs-lookup"><span data-stu-id="486c3-117">Enterprise Mobility + Security (EMS) E5 license</span></span>
- <span data-ttu-id="486c3-118">本教程假定您使用的是 Microsoft Graph 资源管理器，但您可以使用 Postman 或创建自己的客户端应用程序来调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="486c3-118">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="486c3-119">若要在本教程中调用 Microsoft Graph Api，您需要使用具有全局管理员角色和相应权限的帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-119">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="486c3-120">在本教程中， `User.ReadWrite.All` `Group.ReadWrite.All` 需要、和 `EntitlementManagement.ReadWrite.All` 委派权限。</span><span class="sxs-lookup"><span data-stu-id="486c3-120">For this tutorial, the `User.ReadWrite.All`, `Group.ReadWrite.All`, and `EntitlementManagement.ReadWrite.All` delegated permissions are needed.</span></span> <span data-ttu-id="486c3-121">完成以下步骤以在 Microsoft Graph 资源管理器中设置权限：</span><span class="sxs-lookup"><span data-stu-id="486c3-121">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="486c3-122">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="486c3-122">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="486c3-123">选择 **"使用 Microsoft 登录"** ，并使用 Azure AD 全局管理员帐户登录。</span><span class="sxs-lookup"><span data-stu-id="486c3-123">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="486c3-124">成功登录后，可以在左侧窗格中看到用户帐户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="486c3-124">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="486c3-125">选择用户帐户详细信息右侧的 "设置" 图标，然后选择 " **选择权限**"。</span><span class="sxs-lookup"><span data-stu-id="486c3-125">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![选择 Microsoft Graph 权限](./images/tutorial-access-package-api/set-permissions.png)
        
    4. <span data-ttu-id="486c3-127">在权限列表中浏览 `Group` 权限，展开 " \*\*组 (2") \*\*，选择 **Group. ReadWrite。 "All** " 权限。</span><span class="sxs-lookup"><span data-stu-id="486c3-127">Scroll through the list of permissions to the `Group` permissions, expand **Group (2)**, select the **Group.ReadWrite.All** permission.</span></span> <span data-ttu-id="486c3-128">向下滚动到 `User` 权限列表，展开 " \*\*用户 (8") \*\*，然后选择 "用户" " **全部** " 权限。</span><span class="sxs-lookup"><span data-stu-id="486c3-128">Scroll further down the list of permissions to the `User` permissions, expand **User (8)**, and select the **User.ReadWrite.All** permission.</span></span>

        ![搜索用户、组和 entitlementmanagement 权限](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. <span data-ttu-id="486c3-130">选择 " **同意**"，然后选择 " **接受** " 接受权限许可。</span><span class="sxs-lookup"><span data-stu-id="486c3-130">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="486c3-131">您无需代表组织同意这些权限。</span><span class="sxs-lookup"><span data-stu-id="486c3-131">You do not need to consent on behalf of your organization for these permissions.</span></span>
    6. <span data-ttu-id="486c3-132">搜索 `EntitlementManagement` 权限，展开 " \*\*EntitlementManagement (2") \*\*，选择 "权限" " **全部** " 权限，然后选择 " **同意**"。</span><span class="sxs-lookup"><span data-stu-id="486c3-132">Search for the `EntitlementManagement` permissions, expand **EntitlementManagement (2)**, select the **Entitlement.ReadWrite.All** permission, and then select **Consent**.</span></span> <span data-ttu-id="486c3-133">由于此权限需要管理员同意，并且您在本教程中创建的用户帐户是必需的，因此必须 **在代表组织时选择 "同意"**。</span><span class="sxs-lookup"><span data-stu-id="486c3-133">Because this permission requires admin consent and is needed by a user account that you create in this tutorial, you must select **Consent on behalf of your organization**.</span></span>

        ![同意组织](./images/tutorial-access-package-api/consent-for-organization.png)

    7. <span data-ttu-id="486c3-135">选择 " **接受** " 接受权限许可。</span><span class="sxs-lookup"><span data-stu-id="486c3-135">Select **Accept** to accept the consent of the permissions.</span></span>

## <a name="step-1-create-a-user-account-and-a-group"></a><span data-ttu-id="486c3-136">步骤1：创建用户帐户和组</span><span class="sxs-lookup"><span data-stu-id="486c3-136">Step 1: Create a user account and a group</span></span>

<span data-ttu-id="486c3-137">在此步骤中，您将在目录中创建名为 " **营销资源** " 的组，作为用于资格管理的目标资源。</span><span class="sxs-lookup"><span data-stu-id="486c3-137">In this step, you create a group named **Marketing resources** in the directory that is the target resource for entitlement management.</span></span> <span data-ttu-id="486c3-138">您还可以创建设置为内部请求程序的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-138">You also create a user account that is set up as an internal requestor.</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="486c3-139">创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="486c3-139">Create a user account</span></span>

<span data-ttu-id="486c3-140">在本教程中，您将创建用于请求访问访问包中的资源的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-140">For this tutorial, you create a user account that is used to request access to the resources in the access package.</span></span> <span data-ttu-id="486c3-141">在进行这些调用时，请转 `contoso.onmicrosoft.com` 到租户的域名。</span><span class="sxs-lookup"><span data-stu-id="486c3-141">When you make these calls, change `contoso.onmicrosoft.com` to the domain name of your tenant.</span></span> <span data-ttu-id="486c3-142">您可以在 Azure Active Directory 概述页面上找到租户信息。</span><span class="sxs-lookup"><span data-stu-id="486c3-142">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="486c3-143">记录返回的 **id** 属性的值，该属性将在本教程后面的部分中使用。</span><span class="sxs-lookup"><span data-stu-id="486c3-143">Record the value of the **id** property that is returned to be used later in the tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-144">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-144">Request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"Requestor1",
  "mailNickname":"Requestor1",
  "userPrincipalName":"Requestor1@contoso.onmicrosoft.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="486c3-145">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-145">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
  "deletedDateTime": null,
  "accountEnabled": true,
  "ageGroup": null,
  "businessPhones": [],
  "city": null,
  "createdDateTime": null,
  "creationType": null,
  "companyName": null,
  "consentProvidedForMinor": null,
  "country": null,
  "department": null,
  "displayName": "Requestor1",
  "employeeId": null,
  "faxNumber": null,
  "givenName": null,
  "imAddresses": [],
  "infoCatalogs": [],
  "isResourceAccount": null,
  "jobTitle": null,
  "legalAgeGroupClassification": null,
  "mail": null,
  "mailNickname": "Requestor1",
}
```

### <a name="create-a-group"></a><span data-ttu-id="486c3-146">创建组</span><span class="sxs-lookup"><span data-stu-id="486c3-146">Create a group</span></span>

<span data-ttu-id="486c3-147">在本教程中，您将创建一个名为 " **营销资源** " 的组，该组是用于获得资格管理的目标资源。</span><span class="sxs-lookup"><span data-stu-id="486c3-147">In this tutorial, you create a group named **Marketing resources** that is the target resource for entitlement management.</span></span> <span data-ttu-id="486c3-148">您可以使用现有的组（如果已经有的话）。</span><span class="sxs-lookup"><span data-stu-id="486c3-148">You can use an existing group if you already have one.</span></span> <span data-ttu-id="486c3-149">记录返回的 **id** 属性的值，此属性将在本教程后面的部分中使用。</span><span class="sxs-lookup"><span data-stu-id="486c3-149">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="486c3-150">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-150">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
  "description":"Marketing group",
  "displayName":"Marketing resources",
  "mailEnabled":false,
  "mailNickname":"markres",
  "securityEnabled":true
}
```

#### <a name="response"></a><span data-ttu-id="486c3-151">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-151">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
  "id": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2020-06-24T16:47:37Z",
  "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
  "description": "Marketing group",
  "displayName": "Marketing resources",
  "expirationDateTime": null,
  "groupTypes": [],
  "infoCatalogs": [],
  "isAssignableToRole": null,
  "mail": null,
  "mailEnabled": false,
  "mailNickname": "markres"
}
```

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a><span data-ttu-id="486c3-152">步骤2：向目录中添加资源并创建访问包</span><span class="sxs-lookup"><span data-stu-id="486c3-152">Step 2: Add resources to a catalog and create an access package</span></span>

<span data-ttu-id="486c3-153">*访问包*是团队或项目所需并受策略管辖的资源的捆绑。</span><span class="sxs-lookup"><span data-stu-id="486c3-153">An *access package* is a bundle of resources that a team or project needs and is governed with policies.</span></span> <span data-ttu-id="486c3-154">访问包在名为 "目录" 的容器中定义。</span><span class="sxs-lookup"><span data-stu-id="486c3-154">Access packages are defined in containers called catalogs.</span></span> <span data-ttu-id="486c3-155">目录可以引用在 access 程序包中使用的资源，如组、应用程序和网站。</span><span class="sxs-lookup"><span data-stu-id="486c3-155">Catalogs can reference resources, such as groups, apps and sites, that are used in the access package.</span></span> <span data-ttu-id="486c3-156">在此步骤中，您将在 "常规" 目录中创建一个 **市场营销活动** 访问包。</span><span class="sxs-lookup"><span data-stu-id="486c3-156">In this step, you create a **Marketing Campaign** access package in the General catalog.</span></span> <span data-ttu-id="486c3-157">如果您有一个不同的目录，请在下一节中使用它的名称。</span><span class="sxs-lookup"><span data-stu-id="486c3-157">If you have a different catalog, use its name in the next section.</span></span>

### <a name="get-the-catalog-identifier"></a><span data-ttu-id="486c3-158">获取目录标识符</span><span class="sxs-lookup"><span data-stu-id="486c3-158">Get the catalog identifier</span></span>

<span data-ttu-id="486c3-159">若要将资源添加到目录，必须首先获取它的标识符。</span><span class="sxs-lookup"><span data-stu-id="486c3-159">To add resources to the catalog, you must first get the identifier of it.</span></span> <span data-ttu-id="486c3-160">如果使用的是常规目录，请运行以下请求获取其标识符。</span><span class="sxs-lookup"><span data-stu-id="486c3-160">If you are using the General catalog, run the following request to get its identifier.</span></span> <span data-ttu-id="486c3-161">如果您使用的是其他 calalog，请将请求中的筛选器值更改为您的目录的名称。</span><span class="sxs-lookup"><span data-stu-id="486c3-161">If you are using a different calalog, change the filter value in the request to the name of your catalog.</span></span> <span data-ttu-id="486c3-162">记录返回的 **id** 属性的值，此属性将在本教程后面的部分中使用。</span><span class="sxs-lookup"><span data-stu-id="486c3-162">Record the value of the **id** property that is returned to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-163">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-163">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a><span data-ttu-id="486c3-164">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-164">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageCatalogs",
  "value": [ 
    {
      "id": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "displayName": "General",
      "description": "Built-in catalog.",
      "catalogType": "ServiceDefault",
      "catalogStatus": "Published",
      "isExternallyVisible": true,
      "createdBy": "Azure AD",
      "createdDateTime": "2020-05-30T10:58:05.363Z",
      "modifiedBy": "Azure AD",
      "modifiedDateTime": "2020-05-30T10:58:05.363Z"
    }
  ]
}
```

<span data-ttu-id="486c3-165">响应应仅包含您在请求中提供其名称的目录。</span><span class="sxs-lookup"><span data-stu-id="486c3-165">The response should only contain the catalog whose name you provided in the request.</span></span> <span data-ttu-id="486c3-166">如果没有返回任何值，请先检查目录的名称是否正确，然后再继续。</span><span class="sxs-lookup"><span data-stu-id="486c3-166">If there are no values returned, check that the name of the catalog is correct before you proceed.</span></span>

### <a name="add-the-group-to-the-catalog"></a><span data-ttu-id="486c3-167">将组添加到目录</span><span class="sxs-lookup"><span data-stu-id="486c3-167">Add the group to the catalog</span></span>

<span data-ttu-id="486c3-168">若要将您创建的组添加到目录中，请提供以下属性值：</span><span class="sxs-lookup"><span data-stu-id="486c3-168">To add the group that you created to the catalog, provide the following property values:</span></span>
- <span data-ttu-id="486c3-169">**catalogId** -你正在使用的目录的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-169">**catalogId** - the **id** of the catalog that you are using</span></span>
- <span data-ttu-id="486c3-170">**displayName** -组的名称</span><span class="sxs-lookup"><span data-stu-id="486c3-170">**displayName** - the name of the group</span></span>
- <span data-ttu-id="486c3-171">**description** -组的说明</span><span class="sxs-lookup"><span data-stu-id="486c3-171">**description** - the description of the group</span></span>
- <span data-ttu-id="486c3-172">**originId** -你创建的组的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-172">**originId** - the **id** of the group that you created</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-173">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-173">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
    "displayName": "Marketing resources",
    "description": "Marketing group",
    "resourceType": "AadGroup",
    "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="486c3-174">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-174">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "executeImmediately": false,
  "id": "44e521e0-fb6b-4d5e-a282-e7e68dc59493",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": ""
}
```

### <a name="get-catalog-resources"></a><span data-ttu-id="486c3-175">获取目录资源</span><span class="sxs-lookup"><span data-stu-id="486c3-175">Get catalog resources</span></span>

<span data-ttu-id="486c3-176">在本教程后面的步骤中，您需要在目录中分配给组资源的 **id** 。</span><span class="sxs-lookup"><span data-stu-id="486c3-176">In later steps in this tutorial, you need the **id** that was assigned to the group resource in the catalog.</span></span> <span data-ttu-id="486c3-177">此标识符将组表示为目录中的资源，与 Microsoft Graph 中的组本身的标识符不同。</span><span class="sxs-lookup"><span data-stu-id="486c3-177">This identifier, which represents the group as a resource in the catalog, is different than the identifier of the group itself in Microsoft Graph.</span></span> <span data-ttu-id="486c3-178">这是因为目录可以包含未在 Microsoft Graph 中表示的资源。</span><span class="sxs-lookup"><span data-stu-id="486c3-178">This is because a catalog can have resources which aren't represented in Microsoft Graph.</span></span>

<span data-ttu-id="486c3-179">在请求中，提供您正在使用的目录的 **id** 。</span><span class="sxs-lookup"><span data-stu-id="486c3-179">In the request, provide the **id** of the catalog that you are using.</span></span> <span data-ttu-id="486c3-180">记录组目录资源的 **id** 属性的值。</span><span class="sxs-lookup"><span data-stu-id="486c3-180">Record the value of the **id** property for the group catalog resource.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-181">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-181">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a><span data-ttu-id="486c3-182">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-182">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResources",
  "value": [
    {
      "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
      "displayName": "Marketing resources",
      "description": "Marketing group",
      "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "resourceType": "Security Group",
      "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "originSystem": "AadGroup",
      "isPendingOnboarding": false,
      "addedBy": "admin@contoso.onmicrosoft.com",
      "addedOn": "2020-08-21T19:27:29.967Z"
    }
  ]
}
```

### <a name="get-resources-roles"></a><span data-ttu-id="486c3-183">获取资源角色</span><span class="sxs-lookup"><span data-stu-id="486c3-183">Get resources roles</span></span>

<span data-ttu-id="486c3-184">访问包将用户分配给资源的角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-184">The access package assigns users to the roles of a resource.</span></span> <span data-ttu-id="486c3-185">组的典型角色是成员角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-185">The typical role of a group is the member role.</span></span> <span data-ttu-id="486c3-186">其他资源（例如，SharePoint Online 网站和应用程序）可能具有许多角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-186">Other resources, such as SharePoint Online sites and applications, might have many roles.</span></span> <span data-ttu-id="486c3-187">访问包中使用的组的典型角色是成员角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-187">The typical role of a group used in an access package is the member role.</span></span> <span data-ttu-id="486c3-188">在本教程后面的访问包中添加资源角色时，将需要 member 角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-188">You'll need the member role when you add a resource role to the access package later in this tutorial.</span></span> 

<span data-ttu-id="486c3-189">在请求中，使用目录的 **id** 和在您记录的目录中的组资源 **id** ，以获取成员资源角色的 **originId** 。</span><span class="sxs-lookup"><span data-stu-id="486c3-189">In the request, use the **id** of the catalog and the **id** of the group resource in the catalog that you recorded to get the **originId** of the Member resource role.</span></span> <span data-ttu-id="486c3-190">记录 **originId** 属性的值，以便在本教程后面的部分中使用。</span><span class="sxs-lookup"><span data-stu-id="486c3-190">Record the value of the **originId** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-191">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-191">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a><span data-ttu-id="486c3-192">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-192">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('ede67938-cda7-4127-a9ca-7c7bf86a19b7')/accessPackageResourceRoles(accessPackageResource())",
  "value": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "displayName": "Member",
      "description": null,
      "originSystem": "AadGroup",
      "originId": "Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "accessPackageResource@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/$entity",
      "accessPackageResource": {
        "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
        "displayName": "Marketing resources",
        "description": "Marketing group",
        "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "resourceType": "Security Group",
        "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "originSystem": "AadGroup",
        "isPendingOnboarding": false,
        "addedBy": "admin@contoso.onmicrosoft.com",
        "addedOn": "2020-06-26T17:13:23.723Z",
        "accessPackageResourceScopes@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/accessPackageResourceScopes",
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

<span data-ttu-id="486c3-193">如果成功，则返回单个值，表示该组的成员角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-193">If successful, a single value is returned, which represents the Member role of that group.</span></span> <span data-ttu-id="486c3-194">如果未返回任何角色，请检查目录的 **id** 值和访问包资源。</span><span class="sxs-lookup"><span data-stu-id="486c3-194">If no roles are returned, check the **id** values of the catalog and the access package resource.</span></span>

### <a name="create-the-access-package"></a><span data-ttu-id="486c3-195">创建访问包</span><span class="sxs-lookup"><span data-stu-id="486c3-195">Create the access package</span></span>

<span data-ttu-id="486c3-196">此时，您有一个包含组资源的目录，并且您知道您将使用访问包中的组成员的资源角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-196">At this point, you have a catalog with a group resource, and you know that you'll use the resource role of group member in the access package.</span></span> <span data-ttu-id="486c3-197">下一步是创建访问包。</span><span class="sxs-lookup"><span data-stu-id="486c3-197">The next step is to create the access package.</span></span> <span data-ttu-id="486c3-198">拥有访问包后，可以向其添加资源角色，并创建一个策略，用于用户如何请求访问该资源角色。</span><span class="sxs-lookup"><span data-stu-id="486c3-198">After you have the access package, you can add the resource role to it, and create a policy for how users can request access to that resource role.</span></span> <span data-ttu-id="486c3-199">使用之前记录的目录 **id** 创建访问包。</span><span class="sxs-lookup"><span data-stu-id="486c3-199">You use the **id** of the catalog that you recorded earlier to create the access package.</span></span> <span data-ttu-id="486c3-200">记录此教程后面要使用的访问包的 **id** 。</span><span class="sxs-lookup"><span data-stu-id="486c3-200">Record the **id** of the access package to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-201">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-201">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a><span data-ttu-id="486c3-202">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-202">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages/$entity",
  "id": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign",
  "isHidden": false,
  "isRoleScopesVisible": false,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:45:33.2042281Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:45:33.2042281Z"
}
```

### <a name="add-a-resource-role-to-the-access-package"></a><span data-ttu-id="486c3-203">向访问包中添加资源角色</span><span class="sxs-lookup"><span data-stu-id="486c3-203">Add a resource role to the access package</span></span>

<span data-ttu-id="486c3-204">将组资源的 Member 角色添加到访问包中。</span><span class="sxs-lookup"><span data-stu-id="486c3-204">Add the Member role of the group resource to the access package.</span></span> <span data-ttu-id="486c3-205">在请求中，提供访问包的 **id** 。</span><span class="sxs-lookup"><span data-stu-id="486c3-205">In the request, provide the **id** of the access package.</span></span> <span data-ttu-id="486c3-206">在请求正文中，提供 accessPackageResource 的组目录资源的 **id** ，并提供以前记录的成员角色的 **originId** 。</span><span class="sxs-lookup"><span data-stu-id="486c3-206">In the request body provide the **id** of the group catalog resource for accessPackageResource, and provide the **originId** of the Member role that you previously recorded.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-207">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-207">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/88203d16-0e31-41d4-87b2-dd402f1435e9/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole": {
    "originId":"Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource": {
      "id":"4a1e21c5-8a76-4578-acb1-641160e076e8","resourceType":"Security Group",  
      "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
    }
  },
  "accessPackageResourceScope": {
    "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="486c3-208">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-208">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages('88203d16-0e31-41d4-87b2-dd402f1435e9')/accessPackageResourceRoleScopes/$entity",
  "id": "e081321b-2802-4834-a6ca-6f598ce3cdf7_6dbd2209-9d14-4c76-b92b-fcb00e835fe1",
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:56:00.6320729Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:56:00.6320729Z"
}
```

<span data-ttu-id="486c3-209">访问包现在具有一个资源角色，这是组成员身份。</span><span class="sxs-lookup"><span data-stu-id="486c3-209">The access package now has one resource role, which is group membership.</span></span> <span data-ttu-id="486c3-210">将角色分配给具有访问包的任何用户。</span><span class="sxs-lookup"><span data-stu-id="486c3-210">The role is assigned to any user who has the access package.</span></span>

### <a name="create-an-access-package-policy"></a><span data-ttu-id="486c3-211">创建访问包策略</span><span class="sxs-lookup"><span data-stu-id="486c3-211">Create an access package policy</span></span>

<span data-ttu-id="486c3-212">现在，您已创建了访问包并添加了资源和角色，您可以通过创建 access 程序包策略来决定谁可以访问它。</span><span class="sxs-lookup"><span data-stu-id="486c3-212">Now that you created the access package and added resources and roles, you can decide who can access it by creating an access package policy.</span></span> <span data-ttu-id="486c3-213">在本教程中，您将启用您创建的 **Requestor1** 帐户，以请求访问访问包中的资源。</span><span class="sxs-lookup"><span data-stu-id="486c3-213">In this tutorial, you enable the **Requestor1** account that you created to request access to the resources in the access package.</span></span> <span data-ttu-id="486c3-214">对于此任务，您需要以下这些值：</span><span class="sxs-lookup"><span data-stu-id="486c3-214">For this task, you need these values:</span></span>
- <span data-ttu-id="486c3-215">**accessPackageId**属性值的访问包的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-215">**id** of the access package for the value of the **accessPackageId** property</span></span>
- <span data-ttu-id="486c3-216">**allowedRequestors**中**id**属性值的**Requestor1**用户帐户的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-216">**id** of the **Requestor1** user account for the value of the **id** property in **allowedRequestors**</span></span>
 
<span data-ttu-id="486c3-217">**DurationInDays**属性的值使**Requestor1**帐户能够访问访问包中的资源，最长可达30天。</span><span class="sxs-lookup"><span data-stu-id="486c3-217">The value of the **durationInDays** property enables the **Requestor1** account to access the resources in the access package for up to 30 days.</span></span> <span data-ttu-id="486c3-218">记录返回的 **id** 属性的值，此属性将在本教程后面的部分中使用。</span><span class="sxs-lookup"><span data-stu-id="486c3-218">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="486c3-219">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-219">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "accessReviewSettings": null,
  "durationInDays": 30,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.singleUser",
         "isBackup": false,
         "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
         "description": "Requestor1"
       }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

#### <a name="response"></a><span data-ttu-id="486c3-220">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-220">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentPolicies/$entity",
  "id": "db440482-1210-4a60-9b55-3ac7a72f63ba",
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "canExtend": false,
  "durationInDays": 30,
  "expirationDateTime": null,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-06-29T19:47:44.7399675Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-06-29T19:47:44.7555489Z",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
      {
        "@odata.type": "#microsoft.graph.singleUser",
        "isBackup": false,
        "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
        "description": "Requestor1"
      }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

## <a name="step-3-request-access"></a><span data-ttu-id="486c3-221">步骤3：请求访问</span><span class="sxs-lookup"><span data-stu-id="486c3-221">Step 3: Request access</span></span>

<span data-ttu-id="486c3-222">在此步骤中， **Requestor1** 用户帐户请求访问访问包中的资源。</span><span class="sxs-lookup"><span data-stu-id="486c3-222">In this step, the **Requestor1** user account requests access to the resources in the access package.</span></span>

<span data-ttu-id="486c3-223">若要请求对访问包中的资源的访问权限，需要提供以下值：</span><span class="sxs-lookup"><span data-stu-id="486c3-223">To request access to resources in the access package, you need to provide these values:</span></span>
- <span data-ttu-id="486c3-224">为**targetId**属性的值创建的**Requestor1**用户帐户的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-224">**id** of the **Requestor1** user account that you created for the value of the **targetId** property</span></span>
- <span data-ttu-id="486c3-225">**assignmentPolicyId**属性值的分配策略的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-225">**id** of the assignment policy for the value of the **assignmentPolicyId** property</span></span>
- <span data-ttu-id="486c3-226">**accessPackageId**属性值的访问包的**id**</span><span class="sxs-lookup"><span data-stu-id="486c3-226">**id** of the access package for the value of **accessPackageId** property</span></span>

<span data-ttu-id="486c3-227">在响应中，可以看到 "已 **接受** " 和 "已 **提交**" 状态。</span><span class="sxs-lookup"><span data-stu-id="486c3-227">In the response you can see the status of **Accepted** and a state of **Submitted**.</span></span> <span data-ttu-id="486c3-228">记录稍后返回的 **id** 属性的值，以获取请求的状态。</span><span class="sxs-lookup"><span data-stu-id="486c3-228">Record the value of the **id** property that is returned to get the status of the request later.</span></span>

<span data-ttu-id="486c3-229">如果尚未执行此操作，请注销您在 Microsoft Graph 资源管理器中使用的管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-229">If you haven't done so already, sign out of the administrator account that you were using in Microsoft Graph Explorer.</span></span> <span data-ttu-id="486c3-230">登录到您创建的 **Requestor1** 用户帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-230">Sign in to the **Requestor1** user account that you created.</span></span> <span data-ttu-id="486c3-231">如果您是首次登录，系统会提示您更改密码。</span><span class="sxs-lookup"><span data-stu-id="486c3-231">You will be asked to change the password if it is the first time you are signing in.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-232">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-232">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "UserAdd",
  "accessPackageAssignment":{
     "targetId":"007d1c7e-7fa8-4e33-b678-5e437acdcddc",
     "assignmentPolicyId":"db440482-1210-4a60-9b55-3ac7a72f63ba",
     "accessPackageId":"88203d16-0e31-41d4-87b2-dd402f1435e9"
  }
}
```

#### <a name="response"></a><span data-ttu-id="486c3-233">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-233">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

## <a name="step-4-validate-that-access-has-been-assigned"></a><span data-ttu-id="486c3-234">步骤4：验证是否已分配访问权限</span><span class="sxs-lookup"><span data-stu-id="486c3-234">Step 4: Validate that access has been assigned</span></span>

<span data-ttu-id="486c3-235">在此步骤中，您确认已为 **Requestor1** 用户帐户分配了访问包，并且它们现在是 " **营销资源** " 组的成员。</span><span class="sxs-lookup"><span data-stu-id="486c3-235">In this step, you confirm that the **Requestor1** user account was assigned the access package and that they are now a member of the **Marketing resources** group.</span></span>

<span data-ttu-id="486c3-236">注销 Requestor1 帐户并重新登录到管理员帐户，以查看请求的状态。</span><span class="sxs-lookup"><span data-stu-id="486c3-236">Sign out of the Requestor1 account and sign back in to the administrator account to see the status of the request.</span></span>

### <a name="get-the-status-of-the-request"></a><span data-ttu-id="486c3-237">获取请求的状态</span><span class="sxs-lookup"><span data-stu-id="486c3-237">Get the status of the request</span></span>

<span data-ttu-id="486c3-238">使用请求的 **id** 属性的值获取其当前状态。</span><span class="sxs-lookup"><span data-stu-id="486c3-238">Use the value of the **id** property of the request to get the current status of it.</span></span> <span data-ttu-id="486c3-239">在响应中，可以看到状态已更改为 "已 **完成** "，状态更改为 "已 **传递**"。</span><span class="sxs-lookup"><span data-stu-id="486c3-239">In the response, you can see the status changed to **Fulfilled** and the state changed to **Delivered**.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-240">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-240">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a><span data-ttu-id="486c3-241">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-241">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
  "createdDateTime": "2020-06-29T20:24:24.683Z",
  "completedDate": "2020-06-29T20:24:47.937Z",
  "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": null
}
```

### <a name="get-access-package-assignments"></a><span data-ttu-id="486c3-242">获取访问包分配</span><span class="sxs-lookup"><span data-stu-id="486c3-242">Get access package assignments</span></span>

<span data-ttu-id="486c3-243">您还可以使用您创建的 access 程序包策略的 **id** ，以查看是否已将资源分配给 **Requestor1** 用户帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-243">You can also use the **id** of the access package policy that you created to see that resources have been assigned to the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-244">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-244">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
```

#### <a name="response"></a><span data-ttu-id="486c3-245">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-245">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignments",
  "value": [
    {
      "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
      "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
      "assignmentPolicyId": "db440482-1210-4a60-9b55-3ac7a72f63ba",
      "targetId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0",
      "assignmentStatus": "Delivered",
      "assignmentState": "Delivered",
      "isExtended": false,
      "expiredDateTime": null
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a><span data-ttu-id="486c3-246">获取组的成员</span><span class="sxs-lookup"><span data-stu-id="486c3-246">Get the members of the group</span></span>

<span data-ttu-id="486c3-247">在请求被授予之后，可以使用您为 "**营销资源**" 组记录的**id** ，以查看是否已向其添加了**Requestor1**用户帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-247">After the request has been granted, you can use the **id** that you recorded for the **Marketing resources** group to see that the **Requestor1** user account has been added to it.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-248">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-248">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a><span data-ttu-id="486c3-249">响应：</span><span class="sxs-lookup"><span data-stu-id="486c3-249">Response:</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "businessPhones": [],
      "city": null,
      "createdDateTime": "2020-06-23T18:43:24Z",
      "creationType": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "department": null,
      "displayName": "Requestor1",
      "employeeId": null,
      "faxNumber": null,
      "givenName": null,
      "imAddresses": [],
      "infoCatalogs": [],
      "isResourceAccount": null,
      "jobTitle": null,
      "legalAgeGroupClassification": null,
      "mail": null,
      "mailNickname": "Requestor1"
    }
  ]
}
```

## <a name="step-5-clean-up-resources"></a><span data-ttu-id="486c3-250">步骤5：清理资源</span><span class="sxs-lookup"><span data-stu-id="486c3-250">Step 5: Clean up resources</span></span>

<span data-ttu-id="486c3-251">在此步骤中，您将删除所做的更改并删除 **市场营销活动** 访问包。</span><span class="sxs-lookup"><span data-stu-id="486c3-251">In this step, you remove the changes you made and delete the **Marketing Campaign** access package.</span></span>

### <a name="remove-an-access-package-assignment"></a><span data-ttu-id="486c3-252">删除访问包分配</span><span class="sxs-lookup"><span data-stu-id="486c3-252">Remove an access package assignment</span></span>

<span data-ttu-id="486c3-253">必须删除对访问包的所有分配，然后才能将其删除。</span><span class="sxs-lookup"><span data-stu-id="486c3-253">You must remove any assignments to the access package before you can delete it.</span></span> <span data-ttu-id="486c3-254">使用之前录制的工作分配请求的 **id** 将其删除。</span><span class="sxs-lookup"><span data-stu-id="486c3-254">Use the **id** of the assignment request that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-255">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-255">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminRemove",
  "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
  }
}
```

#### <a name="response"></a><span data-ttu-id="486c3-256">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-256">Response</span></span>

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="delete-the-access-package-assignment-policy"></a><span data-ttu-id="486c3-257">删除访问包分配策略</span><span class="sxs-lookup"><span data-stu-id="486c3-257">Delete the access package assignment policy</span></span>

<span data-ttu-id="486c3-258">使用之前已录制的分配策略的 **id** 将其删除。</span><span class="sxs-lookup"><span data-stu-id="486c3-258">Use the **id** of the assignment policy that you previously recorded to delete it.</span></span> <span data-ttu-id="486c3-259">请确保先删除所有分配。</span><span class="sxs-lookup"><span data-stu-id="486c3-259">Make sure all assignments are removed first.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-260">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-260">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a><span data-ttu-id="486c3-261">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-261">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-access-package"></a><span data-ttu-id="486c3-262">删除访问包</span><span class="sxs-lookup"><span data-stu-id="486c3-262">Delete the access package</span></span>

<span data-ttu-id="486c3-263">使用您以前录制的访问包的 **id** 将其删除。</span><span class="sxs-lookup"><span data-stu-id="486c3-263">Use the **id** of the access package that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-264">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-264">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a><span data-ttu-id="486c3-265">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-265">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="486c3-266">删除用户帐户</span><span class="sxs-lookup"><span data-stu-id="486c3-266">Delete the user account</span></span>

<span data-ttu-id="486c3-267">删除 **Requestor1** 用户帐户。</span><span class="sxs-lookup"><span data-stu-id="486c3-267">Delete the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-268">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-268">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a><span data-ttu-id="486c3-269">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-269">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-group"></a><span data-ttu-id="486c3-270">添加或删除组成员</span><span class="sxs-lookup"><span data-stu-id="486c3-270">Delete the group</span></span>

<span data-ttu-id="486c3-271">删除 " **营销资源** " 组。</span><span class="sxs-lookup"><span data-stu-id="486c3-271">Delete the **Marketing resources** group.</span></span>

#### <a name="request"></a><span data-ttu-id="486c3-272">请求</span><span class="sxs-lookup"><span data-stu-id="486c3-272">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a><span data-ttu-id="486c3-273">响应</span><span class="sxs-lookup"><span data-stu-id="486c3-273">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="486c3-274">另请参阅</span><span class="sxs-lookup"><span data-stu-id="486c3-274">See also</span></span>

<span data-ttu-id="486c3-275">在本教程中，你使用了许多 Api 来完成任务。</span><span class="sxs-lookup"><span data-stu-id="486c3-275">In this tutorial, you used many APIs to accomplish tasks.</span></span> <span data-ttu-id="486c3-276">浏览这些 Api 的 API 参考，了解有关 Api 可以执行的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="486c3-276">Explore the API reference for these APIs to learn more about what the APIs can do.</span></span>


- [<span data-ttu-id="486c3-277">使用 Azure AD 权限管理 API</span><span class="sxs-lookup"><span data-stu-id="486c3-277">Working with the Azure AD entitlement management API</span></span>](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [<span data-ttu-id="486c3-278">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="486c3-278">accessPackageCatalog</span></span>](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [<span data-ttu-id="486c3-279">accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="486c3-279">accessPackageResourceRequest</span></span>](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [<span data-ttu-id="486c3-280">accessPackage</span><span class="sxs-lookup"><span data-stu-id="486c3-280">accessPackage</span></span>](/graph/api/resources/accesspackage?view=graph-rest-beta)
- [<span data-ttu-id="486c3-281">accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="486c3-281">accessPackageResourceRoleScope</span></span>](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [<span data-ttu-id="486c3-282">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="486c3-282">accessPackageAssignmentPolicy</span></span>](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [<span data-ttu-id="486c3-283">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="486c3-283">accessPackageAssignmentRequest</span></span>](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [<span data-ttu-id="486c3-284">组</span><span class="sxs-lookup"><span data-stu-id="486c3-284">group</span></span>](/graph/api/resources/group?view=graph-rest-1.0)
- [<span data-ttu-id="486c3-285">用户</span><span class="sxs-lookup"><span data-stu-id="486c3-285">user</span></span>](/graph/api/resources/user?view=graph-rest-1.0)