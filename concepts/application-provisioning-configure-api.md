---
title: 使用 Microsoft Graph Api 配置预配
description: 了解如何通过使用 Microsoft Graph API 自动配置自动预配来节省时间。
author: kenwith
ms.topic: conceptual
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 626593ada6c45de18bb24f9ec107fca7d077fb67
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761861"
---
# <a name="configure-provisioning-using-microsoft-graph-apis"></a><span data-ttu-id="e431c-103">使用 Microsoft Graph Api 配置预配</span><span class="sxs-lookup"><span data-stu-id="e431c-103">Configure provisioning using Microsoft Graph APIs</span></span>

<span data-ttu-id="e431c-104">Azure 门户是一种一次配置单个应用的预配的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="e431c-104">The Azure portal is a convenient way to configure provisioning for individual apps one at a time.</span></span> <span data-ttu-id="e431c-105">但是，如果你要创建多个甚至数百个应用程序实例，则使用 Microsoft Graph API 自动创建和配置应用会更容易。</span><span class="sxs-lookup"><span data-stu-id="e431c-105">But if you're creating several—or even hundreds—of instances of an application, it can be easier to automate app creation and configuration with the Microsoft Graph APIs.</span></span> <span data-ttu-id="e431c-106">本文概述了如何通过 API 自动执行预配配置。</span><span class="sxs-lookup"><span data-stu-id="e431c-106">This article outlines how to automate provisioning configuration through APIs.</span></span> <span data-ttu-id="e431c-107">此方法通常用于应用程序，如 [Amazon Web Services](/azure/active-directory/saas-apps/amazon-web-service-tutorial#configure-azure-ad-sso)。</span><span class="sxs-lookup"><span data-stu-id="e431c-107">This method is commonly used for applications like [Amazon Web Services](/azure/active-directory/saas-apps/amazon-web-service-tutorial#configure-azure-ad-sso).</span></span>

<span data-ttu-id="e431c-108">**使用 Microsoft Graph API 自动执行预配配置的步骤概述**</span><span class="sxs-lookup"><span data-stu-id="e431c-108">**Overview of steps for using Microsoft Graph APIs to automate provisioning configuration**</span></span>


|<span data-ttu-id="e431c-109">步骤</span><span class="sxs-lookup"><span data-stu-id="e431c-109">Step</span></span>  |<span data-ttu-id="e431c-110">详细信息</span><span class="sxs-lookup"><span data-stu-id="e431c-110">Details</span></span>  |
|---------|---------|
|[<span data-ttu-id="e431c-111">步骤 1.创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="e431c-111">Step 1. Create the gallery application</span></span>](#step-1-create-the-gallery-application)     |<span data-ttu-id="e431c-112">登录到 API 客户端</span><span class="sxs-lookup"><span data-stu-id="e431c-112">Sign-in to the API client</span></span> <br> <span data-ttu-id="e431c-113">检索库应用程序模板</span><span class="sxs-lookup"><span data-stu-id="e431c-113">Retrieve the gallery application template</span></span> <br> <span data-ttu-id="e431c-114">创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="e431c-114">Create the gallery application</span></span>         |
|[<span data-ttu-id="e431c-115">步骤 2.创建基于模板的预配作业</span><span class="sxs-lookup"><span data-stu-id="e431c-115">Step 2. Create provisioning job based on template</span></span>](#step-2-create-the-provisioning-job-based-on-the-template)     |<span data-ttu-id="e431c-116">检索预配连接器的模板</span><span class="sxs-lookup"><span data-stu-id="e431c-116">Retrieve the template for the provisioning connector</span></span> <br> <span data-ttu-id="e431c-117">创建设置作业</span><span class="sxs-lookup"><span data-stu-id="e431c-117">Create the provisioning job</span></span>         |
|[<span data-ttu-id="e431c-118">步骤 3.授权访问</span><span class="sxs-lookup"><span data-stu-id="e431c-118">Step 3. Authorize access</span></span>](#step-3-authorize-access)     |<span data-ttu-id="e431c-119">测试与应用程序的连接</span><span class="sxs-lookup"><span data-stu-id="e431c-119">Test the connection to the application</span></span> <br> <span data-ttu-id="e431c-120">保存凭据</span><span class="sxs-lookup"><span data-stu-id="e431c-120">Save the credentials</span></span>         |
|[<span data-ttu-id="e431c-121">步骤 4.开始设置作业</span><span class="sxs-lookup"><span data-stu-id="e431c-121">Step 4. Start provisioning job</span></span>](#step-4-start-the-provisioning-job)     |<span data-ttu-id="e431c-122">启动作业</span><span class="sxs-lookup"><span data-stu-id="e431c-122">Start the job</span></span>         |
|[<span data-ttu-id="e431c-123">步骤 5.监视预配</span><span class="sxs-lookup"><span data-stu-id="e431c-123">Step 5. Monitor provisioning</span></span>](#step-5-monitor-provisioning)     |<span data-ttu-id="e431c-124">检查预配作业的状态</span><span class="sxs-lookup"><span data-stu-id="e431c-124">Check the status of the provisioning job</span></span> <br> <span data-ttu-id="e431c-125">检索设置日志</span><span class="sxs-lookup"><span data-stu-id="e431c-125">Retrieve the provisioning logs</span></span>         |

## <a name="step-1-create-the-gallery-application"></a><span data-ttu-id="e431c-126">第 1 步：创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="e431c-126">Step 1: Create the gallery application</span></span>

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a><span data-ttu-id="e431c-127">登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端</span><span class="sxs-lookup"><span data-stu-id="e431c-127">Sign in to Microsoft Graph Explorer (recommended), Postman, or any other API client you use</span></span>

1. <span data-ttu-id="e431c-128">启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="e431c-128">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
1. <span data-ttu-id="e431c-129">选择"使用 Microsoft 登录"按钮，然后使用 Azure AD 全局管理员或应用管理员凭据登录。</span><span class="sxs-lookup"><span data-stu-id="e431c-129">Select the "Sign-In with Microsoft" button and sign in using Azure AD global administrator or App Admin credentials.</span></span>

    ![Graph 登录](./images/application-provisioning-configure-api/wd_export_02.png)

1. <span data-ttu-id="e431c-131">成功登录后，将在左侧窗格中看到用户帐户详细信息。</span><span class="sxs-lookup"><span data-stu-id="e431c-131">Upon successful sign-in, you'll see the user account details in the left-hand pane.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="e431c-132">检索库应用程序模板标识符</span><span class="sxs-lookup"><span data-stu-id="e431c-132">Retrieve the gallery application template identifier</span></span>
<span data-ttu-id="e431c-133">Azure AD 应用程序库中的每个应用程序都有一个[应用程序模板](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta)，用于描述该应用程序的元数据。</span><span class="sxs-lookup"><span data-stu-id="e431c-133">Applications in the Azure AD application gallery each have an [application template](/graph/api/applicationtemplate-list?tabs=http&view=graph-rest-beta) that describes the metadata for that application.</span></span> <span data-ttu-id="e431c-134">使用此模板，可以在租户中创建应用程序和服务主体的实例以进行管理。</span><span class="sxs-lookup"><span data-stu-id="e431c-134">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span>

#### <a name="request"></a><span data-ttu-id="e431c-135">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e431c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e431c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="e431c-137">C#</span><span class="sxs-lookup"><span data-stu-id="e431c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e431c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e431c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e431c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e431c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e431c-140">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
    "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "Amazon Web Services (AWS)",
        "homePageUrl": "http://aws.amazon.com/",
        "supportedSingleSignOnModes": [
             "password",
             "saml",
             "external"
         ],
         "supportedProvisioningTypes": [
             "sync"
         ],
         "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
         "categories": [
             "developerServices"
         ],
         "publisher": "Amazon",
         "description": null    
  
}
```

### <a name="create-the-gallery-application"></a><span data-ttu-id="e431c-141">创建库应用程序</span><span class="sxs-lookup"><span data-stu-id="e431c-141">Create the gallery application</span></span>

<span data-ttu-id="e431c-142">使用在上一步中为应用程序检索的模板 ID，[](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta)在租户中创建应用程序和服务主体的实例。</span><span class="sxs-lookup"><span data-stu-id="e431c-142">Use the template ID retrieved for your application in the last step to [create an instance](/graph/api/applicationtemplate-instantiate?tabs=http&view=graph-rest-beta) of the application and service principal in your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="e431c-143">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e431c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e431c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```
# <a name="c"></a>[<span data-ttu-id="e431c-145">C#</span><span class="sxs-lookup"><span data-stu-id="e431c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e431c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e431c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e431c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e431c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e431c-148">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-148">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json


{
    "application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63",
        "appId": "92653dd4-aa3a-3323-80cf-e8cfefcc8d5d",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "AWS Contoso",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "logoutUrl": null,
        "samlMetadataUrl": null,
    },
    "servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e",
        "appDisplayName": "AWS Contoso",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "appRoleAssignmentRequired": true,
        "displayName": "My custom name",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "servicePrincipalNames": [
            "93653dd4-aa3a-4323-80cf-e8cfefcc8d7d"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
    }
}
```

## <a name="step-2-create-the-provisioning-job-based-on-the-template"></a><span data-ttu-id="e431c-149">步骤 2：基于模板创建预配作业</span><span class="sxs-lookup"><span data-stu-id="e431c-149">Step 2: Create the provisioning job based on the template</span></span>

### <a name="retrieve-the-template-for-the-provisioning-connector"></a><span data-ttu-id="e431c-150">检索预配连接器的模板</span><span class="sxs-lookup"><span data-stu-id="e431c-150">Retrieve the template for the provisioning connector</span></span>

<span data-ttu-id="e431c-151">库中启用了预配的应用程序具有用于简化配置的模板。</span><span class="sxs-lookup"><span data-stu-id="e431c-151">Applications in the gallery that are enabled for provisioning have templates to streamline configuration.</span></span> <span data-ttu-id="e431c-152">使用以下请求 [检索预配配置的模板](/graph/api/synchronization-synchronizationtemplate-list?tabs=http&view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="e431c-152">Use the request below to [retrieve the template for the provisioning configuration](/graph/api/synchronization-synchronizationtemplate-list?tabs=http&view=graph-rest-beta).</span></span> <span data-ttu-id="e431c-153">请注意，你将需要提供 ID。</span><span class="sxs-lookup"><span data-stu-id="e431c-153">Note that you will need to provide the ID.</span></span> <span data-ttu-id="e431c-154">ID 引用上一个资源，本例中为 servicePrincipal 资源。</span><span class="sxs-lookup"><span data-stu-id="e431c-154">The ID refers to the preceding resource, which in this case is the servicePrincipal resource.</span></span> 

#### <a name="request"></a><span data-ttu-id="e431c-155">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e431c-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="e431c-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="c"></a>[<span data-ttu-id="e431c-157">C#</span><span class="sxs-lookup"><span data-stu-id="e431c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e431c-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e431c-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e431c-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e431c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e431c-160">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-160">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "aws",
            "factoryTag": "aws",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

### <a name="create-the-provisioning-job"></a><span data-ttu-id="e431c-161">创建设置作业</span><span class="sxs-lookup"><span data-stu-id="e431c-161">Create the provisioning job</span></span>
<span data-ttu-id="e431c-162">若要启用预配，你首先需要 [创建一个作业](/graph/api/synchronization-synchronizationjob-post?tabs=http&view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="e431c-162">To enable provisioning, you'll first need to [create a job](/graph/api/synchronization-synchronizationjob-post?tabs=http&view=graph-rest-beta).</span></span> <span data-ttu-id="e431c-163">使用以下请求创建设置作业。</span><span class="sxs-lookup"><span data-stu-id="e431c-163">Use the following request to create a provisioning job.</span></span> <span data-ttu-id="e431c-164">指定要用于作业的模板时，请使用上一步中的 templateId。</span><span class="sxs-lookup"><span data-stu-id="e431c-164">Use the templateId from the previous step when specifying the template to be used for the job.</span></span>

#### <a name="request"></a><span data-ttu-id="e431c-165">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e431c-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="e431c-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "aws"
}
```
# <a name="c"></a>[<span data-ttu-id="e431c-167">C#</span><span class="sxs-lookup"><span data-stu-id="e431c-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e431c-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e431c-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e431c-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e431c-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e431c-170">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "id": "{jobId}",
    "templateId": "aws",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

## <a name="step-3-authorize-access"></a><span data-ttu-id="e431c-171">步骤 3：授权访问</span><span class="sxs-lookup"><span data-stu-id="e431c-171">Step 3: Authorize access</span></span>

### <a name="test-the-connection-to-the-application"></a><span data-ttu-id="e431c-172">测试与应用程序的连接</span><span class="sxs-lookup"><span data-stu-id="e431c-172">Test the connection to the application</span></span>

<span data-ttu-id="e431c-173">测试第三方应用程序的连接。</span><span class="sxs-lookup"><span data-stu-id="e431c-173">Test the connection with the third-party application.</span></span> <span data-ttu-id="e431c-174">下面的示例适用于需要客户端密码和密码令牌的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e431c-174">The following example is for an application that requires a client secret and secret token.</span></span> <span data-ttu-id="e431c-175">每个应用程序都有自己的要求。</span><span class="sxs-lookup"><span data-stu-id="e431c-175">Each application has its own requirements.</span></span> <span data-ttu-id="e431c-176">应用程序通常使用基地址来表示客户端密码。</span><span class="sxs-lookup"><span data-stu-id="e431c-176">Applications often use a base address in place of a client secret.</span></span> <span data-ttu-id="e431c-177">若要确定你的应用所需的凭据，请转到应用程序的预配配置页，在开发人员模式下，单击测试 **连接**。</span><span class="sxs-lookup"><span data-stu-id="e431c-177">To determine what credentials your app requires, go to the provisioning configuration page for your application, and in developer mode, click **test connection**.</span></span> <span data-ttu-id="e431c-178">网络流量将显示用于凭据的参数。</span><span class="sxs-lookup"><span data-stu-id="e431c-178">The network traffic will show the parameters used for credentials.</span></span> <span data-ttu-id="e431c-179">有关凭据的完整列表，请参阅 [synchronizationJob： validateCredentials](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="e431c-179">For a full list of credentials, see [synchronizationJob: validateCredentials](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta).</span></span> <span data-ttu-id="e431c-180">大多数应用程序（如 Azure Datab部署）都依赖于 BaseAddress 和 SecretToken。</span><span class="sxs-lookup"><span data-stu-id="e431c-180">Most applications, such as Azure Databricks, rely on a BaseAddress and SecretToken.</span></span> <span data-ttu-id="e431c-181">BaseAddress 在 Azure 门户中作为租户 URL 引用。</span><span class="sxs-lookup"><span data-stu-id="e431c-181">The BaseAddress is refered to as a tenant URL in the Azure Portal.</span></span> 

#### <a name="request"></a><span data-ttu-id="e431c-182">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-182">Request</span></span>
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
{ 
    "credentials": [ 
        { "key": "ClientSecret", "value": "xxxxxxxxxxxxxxxxxxxxx" },
        { "key": "SecretToken", "value": "xxxxxxxxxxxxxxxxxxxxx" }
    ]
}
```
#### <a name="response"></a><span data-ttu-id="e431c-183">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-183">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="save-your-credentials"></a><span data-ttu-id="e431c-184">保存凭据</span><span class="sxs-lookup"><span data-stu-id="e431c-184">Save your credentials</span></span>

<span data-ttu-id="e431c-185">配置预配需要在 Azure AD 和应用程序之间建立信任。</span><span class="sxs-lookup"><span data-stu-id="e431c-185">Configuring provisioning requires establishing a trust between Azure AD and the application.</span></span> <span data-ttu-id="e431c-186">授权访问第三方应用程序。</span><span class="sxs-lookup"><span data-stu-id="e431c-186">Authorize access to the third-party application.</span></span> <span data-ttu-id="e431c-187">下面的示例适用于需要客户端密码和密码令牌的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e431c-187">The following example is for an application that requires a client secret and a secret token.</span></span> <span data-ttu-id="e431c-188">每个应用程序都有自己的要求。</span><span class="sxs-lookup"><span data-stu-id="e431c-188">Each application has its own requirements.</span></span> <span data-ttu-id="e431c-189">查看 [API 文档](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta) 以查看可用选项。</span><span class="sxs-lookup"><span data-stu-id="e431c-189">Review the [API documentation](/graph/api/synchronization-synchronizationjob-validatecredentials?tabs=http&view=graph-rest-beta) to see the available options.</span></span> 

#### <a name="request"></a><span data-ttu-id="e431c-190">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-190">Request</span></span>
```msgraph-interactive
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/secrets 
 
{ 
    "value": [ 
        { "key": "ClientSecret", "value": "xxxxxxxxxxxxxxxxxxxxx" },
        { "key": "SecretToken", "value": "xxxxxxxxxxxxxxxxxxxxx" }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="e431c-191">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-191">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="step-4-start-the-provisioning-job"></a><span data-ttu-id="e431c-192">步骤 4：启动预配作业</span><span class="sxs-lookup"><span data-stu-id="e431c-192">Step 4: Start the provisioning job</span></span>
<span data-ttu-id="e431c-193">配置设置作业后，使用以下命令 [启动作业](/graph/api/synchronization-synchronizationjob-start?tabs=http&view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="e431c-193">Now that the provisioning job is configured, use the following command to [start the job](/graph/api/synchronization-synchronizationjob-start?tabs=http&view=graph-rest-beta).</span></span> 


#### <a name="request"></a><span data-ttu-id="e431c-194">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e431c-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="e431c-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="e431c-196">C#</span><span class="sxs-lookup"><span data-stu-id="e431c-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e431c-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e431c-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e431c-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e431c-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e431c-199">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-199">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="step-5-monitor-provisioning"></a><span data-ttu-id="e431c-200">步骤 5：监视预配</span><span class="sxs-lookup"><span data-stu-id="e431c-200">Step 5: Monitor provisioning</span></span>

### <a name="monitor-the-provisioning-job-status"></a><span data-ttu-id="e431c-201">监视设置作业状态</span><span class="sxs-lookup"><span data-stu-id="e431c-201">Monitor the provisioning job status</span></span>

<span data-ttu-id="e431c-202">现在设置作业正在运行，请使用以下命令跟踪当前设置周期的进度以及到目前为止的统计信息，例如已在目标系统中创建的用户和组数。</span><span class="sxs-lookup"><span data-stu-id="e431c-202">Now that the provisioning job is running, use the following command to track the progress of the current provisioning cycle as well as statistics to date such as the number of users and groups that have been created in the target system.</span></span> 

#### <a name="request"></a><span data-ttu-id="e431c-203">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-203">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e431c-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="e431c-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="e431c-205">C#</span><span class="sxs-lookup"><span data-stu-id="e431c-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e431c-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e431c-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e431c-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e431c-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e431c-208">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-208">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

{
    "id": "{jobId}",
    "templateId": "aws",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    },
    "synchronizationJobSettings": [
      {
          "name": "QuarantineTooManyDeletesThreshold",
          "value": "500"
      }
    ]
}
```


### <a name="monitor-provisioning-events-using-the-provisioning-logs"></a><span data-ttu-id="e431c-209">使用预配日志监视预配事件</span><span class="sxs-lookup"><span data-stu-id="e431c-209">Monitor provisioning events using the provisioning logs</span></span>
<span data-ttu-id="e431c-210">除了监视设置作业的状态之外，您还可以使用设置日志查询发生的所有事件。 [](/graph/api/provisioningobjectsummary-list?tabs=http&view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="e431c-210">In addition to monitoring the status of the provisioning job, you can use the [provisioning logs](/graph/api/provisioningobjectsummary-list?tabs=http&view=graph-rest-beta) to query for all the events that are occurring.</span></span> <span data-ttu-id="e431c-211">例如，查询特定用户并确定他们是否成功预配。</span><span class="sxs-lookup"><span data-stu-id="e431c-211">For example, query for a particular user and determine if they were successfully provisioned.</span></span>

#### <a name="request"></a><span data-ttu-id="e431c-212">请求</span><span class="sxs-lookup"><span data-stu-id="e431c-212">Request</span></span>
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```
#### <a name="response"></a><span data-ttu-id="e431c-213">响应</span><span class="sxs-lookup"><span data-stu-id="e431c-213">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "name": "list_provisioningobjectsummary_error"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/provisioning",
    "value": [
        {
            "id": "gc532ff9-r265-ec76-861e-42e2970a8218",
            "activityDateTime": "2019-06-24T20:53:08Z",
            "tenantId": "7928d5b5-7442-4a97-ne2d-66f9j9972ecn",
            "jobId": "BoxOutDelta.7928d5b574424a97ne2d66f9j9972ecn",
            "cycleId": "44576n58-v14b-70fj-8404-3d22tt46ed93",
            "changeId": "eaad2f8b-e6e3-409b-83bd-e4e2e57177d5",
            "action": "Create",
            "durationInMilliseconds": 2785,
            "sourceSystem": {
                "id": "0404601d-a9c0-4ec7-bbcd-02660120d8c9",
                "displayName": "Azure Active Directory",
                "details": {}
            },
            "targetSystem": {
                "id": "cd22f60b-5f2d-1adg-adb4-76ef31db996b",
                "displayName": "Box",
                "details": {
                    "ApplicationId": "f2764360-e0ec-5676-711e-cd6fc0d4dd61",
                    "ServicePrincipalId": "chc46a42-966b-47d7-9774-576b1c8bd0b8",
                    "ServicePrincipalDisplayName": "Box"
                }
            },
            "initiatedBy": {
                "id": "",
                "displayName": "Azure AD Provisioning Service",
                "initiatorType": "system"
            },
            "sourceIdentity": {
                "id": "5e6c9rae-ab4d-5239-8ad0-174391d110eb",
                "displayName": "Self-service Pilot",
                "identityType": "Group",
                "details": {}
            },
            "targetIdentity": {
                "id": "",
                "displayName": "",
                "identityType": "Group",
                "details": {}
            },
            "statusInfo": {
                "@odata.type": "#microsoft.graph.statusDetails",
                "status": "failure",
                "errorCode": "BoxEntryConflict",
                "reason": "Message: Box returned an error response with the HTTP status code 409.  This response indicates that a user or a group already exisits with the same name. This can be avoided by identifying and removing the conflicting user from Box via the Box administrative user interface, or removing the current user from the scope of provisioning either by removing their assignment to the Box application in Azure Active Directory or adding a scoping filter to exclude the user.",
                "additionalDetails": null,
                "errorCategory": "NonServiceFailure",
                "recommendedAction": null
            },
            "provisioningSteps": [
                {
                    "name": "EntryImportAdd",
                    "provisioningStepType": "import",
                    "status": "success",
                    "description": "Received Group 'Self-service Pilot' change of type (Add) from Azure Active Directory",
                    "details": {}
                },
                {
                    "name": "EntrySynchronizationAdd",
                    "provisioningStepType": "matching",
                    "status": "success",
                    "description": "Group 'Self-service Pilot' will be created in Box (Group is active and assigned in Azure Active Directory, but no matching Group was found in Box)",
                    "details": {}
                },
                {
                    "name": "EntryExportAdd",
                    "provisioningStepType": "export",
                    "status": "failure",
                    "description": "Failed to create Group 'Self-service Pilot' in Box",
                    "details": {
                        "ReportableIdentifier": "Self-service Pilot"
                    }
                }
            ],
            "modifiedProperties": [
                {
                    "displayName": "objectId",
                    "oldValue": null,
                    "newValue": "5e0c9eae-ad3d-4139-5ad0-174391d110eb"
                },
                {
                    "displayName": "displayName",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                },
                {
                    "displayName": "mailEnabled",
                    "oldValue": null,
                    "newValue": "False"
                },
                {
                    "displayName": "mailNickname",
                    "oldValue": null,
                    "newValue": "5ce25n9a-4c5f-45c9-8362-ef3da29c66c5"
                },
                {
                    "displayName": "securityEnabled",
                    "oldValue": null,
                    "newValue": "True"
                },
                {
                    "displayName": "Name",
                    "oldValue": null,
                    "newValue": "Self-service Pilot"
                }
            ]
       }
    ]
}

```
## <a name="see-also"></a><span data-ttu-id="e431c-214">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e431c-214">See also</span></span>

- [<span data-ttu-id="e431c-215">查看同步 Microsoft Graph 文档</span><span class="sxs-lookup"><span data-stu-id="e431c-215">Review the synchronization Microsoft Graph documentation</span></span>](/graph/api/resources/synchronization-overview?view=graph-rest-beta)
- [<span data-ttu-id="e431c-216">将自定义 SCIM 应用与 Azure AD 集成</span><span class="sxs-lookup"><span data-stu-id="e431c-216">Integrating a custom SCIM app with Azure AD</span></span>](/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups)
