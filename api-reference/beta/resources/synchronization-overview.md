---
title: Azure AD 同步 API 概述
description: ) 可自动执行创建、 维护和删除中的标识云 （软件作为服务，还是 SaaS） 应用程序，如收存箱、 销售队伍、 ServiceNow，等等。 您可以使用同步 Api 在 Microsoft Graph 中以编程方式管理标识同步包括：
localization_priority: Normal
ms.openlocfilehash: ed994b8204fdee38f558da499259538e85eacd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529556"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="44c3e-104">Azure AD 同步 API 概述</span><span class="sxs-lookup"><span data-stu-id="44c3e-104">Azure AD synchronization API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44c3e-105">Azure Active Directory (Azure AD) 标识同步 （也称为"设置"），可以自动执行创建、 维护和删除云 （软件作为服务，还是 SaaS） 中的标识收存箱、 销售队伍 ServiceNow，如应用程序等等。</span><span class="sxs-lookup"><span data-stu-id="44c3e-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="44c3e-106">您可以使用同步 Api 在 Microsoft Graph 中以编程方式管理标识同步包括：</span><span class="sxs-lookup"><span data-stu-id="44c3e-106">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="44c3e-107">创建、 启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="44c3e-107">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="44c3e-108">更改作业的同步架构</span><span class="sxs-lookup"><span data-stu-id="44c3e-108">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="44c3e-109">验证当前的同步状态</span><span class="sxs-lookup"><span data-stu-id="44c3e-109">Verify the current synchronization status</span></span> 

<span data-ttu-id="44c3e-110">有关在 Azure AD 的同步的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="44c3e-110">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="44c3e-111">自动化用户设置和解除设置 SaaS 与 Azure Active Directory 的应用程序</span><span class="sxs-lookup"><span data-stu-id="44c3e-111">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="44c3e-112">管理用户帐户设置 Azure 门户中的企业应用程序</span><span class="sxs-lookup"><span data-stu-id="44c3e-112">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="44c3e-113">您还可以尝试示例租户或您自己的租户中的[图资源管理器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="44c3e-113">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="44c3e-114">同步作业</span><span class="sxs-lookup"><span data-stu-id="44c3e-114">Synchronization job</span></span>

<span data-ttu-id="44c3e-115">同步作业执行同步在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改。</span><span class="sxs-lookup"><span data-stu-id="44c3e-115">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="44c3e-116">同步作业始终是特定于您的租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="44c3e-116">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="44c3e-117">作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。</span><span class="sxs-lookup"><span data-stu-id="44c3e-117">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="44c3e-118">有关详细信息，请参阅[同步作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="44c3e-118">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="44c3e-119">同步架构</span><span class="sxs-lookup"><span data-stu-id="44c3e-119">Synchronization schema</span></span>

<span data-ttu-id="44c3e-120">同步架构定义对象将同步和同步方式。</span><span class="sxs-lookup"><span data-stu-id="44c3e-120">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="44c3e-121">同步架构包含特定同步作业的设置信息的大部分。</span><span class="sxs-lookup"><span data-stu-id="44c3e-121">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="44c3e-122">通常情况下，您将自定义某些[属性映射](synchronization-attributemapping.md)，或添加[范围筛选器](synchronization-filter.md)以同步只有满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="44c3e-122">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="44c3e-123">同步架构包括以下组件：</span><span class="sxs-lookup"><span data-stu-id="44c3e-123">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="44c3e-124">目录定义</span><span class="sxs-lookup"><span data-stu-id="44c3e-124">Directory definitions</span></span>
- <span data-ttu-id="44c3e-125">同步规则</span><span class="sxs-lookup"><span data-stu-id="44c3e-125">Synchronization rules</span></span>
- <span data-ttu-id="44c3e-126">对象映射</span><span class="sxs-lookup"><span data-stu-id="44c3e-126">Object mappings</span></span>

<span data-ttu-id="44c3e-127">有关详细信息，请参阅[同步 schema](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="44c3e-127">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="44c3e-128">同步模板</span><span class="sxs-lookup"><span data-stu-id="44c3e-128">Synchronization template</span></span>

<span data-ttu-id="44c3e-129">同步模板提供了为特定应用程序预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="44c3e-129">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="44c3e-130">将基于模板的任何[同步作业，](synchronization-synchronizationjob.md)默认情况下使用这些设置 （最重要的是[同步架构](synchronization-synchronizationschema.md)）。</span><span class="sxs-lookup"><span data-stu-id="44c3e-130">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="44c3e-131">由应用程序开发人员指定模板。</span><span class="sxs-lookup"><span data-stu-id="44c3e-131">Templates are specified by the application developer.</span></span>

<span data-ttu-id="44c3e-132">有关详细信息，请参阅[同步模板](synchronization-synchronizationtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="44c3e-132">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="44c3e-133">使用同步 API</span><span class="sxs-lookup"><span data-stu-id="44c3e-133">Working with the synchronization API</span></span>

<span data-ttu-id="44c3e-134">使用同步 API 主要涉及访问[synchronizationJob](synchronization-synchronizationjob.md)和[synchronizationSchema](synchronization-synchronizationschema.md)资源。</span><span class="sxs-lookup"><span data-stu-id="44c3e-134">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="44c3e-135">若要找到[synchronizationJob](synchronization-synchronizationjob.md)资源，您需要知道同步作业所属的服务主体对象 ID。</span><span class="sxs-lookup"><span data-stu-id="44c3e-135">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="44c3e-136">下面的示例演示如何使用**synchronizationJob**和**synchronizationSchema**资源。</span><span class="sxs-lookup"><span data-stu-id="44c3e-136">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="44c3e-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="44c3e-137">Authorization</span></span>

<span data-ttu-id="44c3e-138">Azure AD 同步 API 使用 OAuth 2.0 授权。</span><span class="sxs-lookup"><span data-stu-id="44c3e-138">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="44c3e-139">Api 任何请求之前，您需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="44c3e-139">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="44c3e-140">有关详细信息，请参阅[获取访问令牌调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="44c3e-140">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="44c3e-141">若要访问同步资源，您的应用程序需要 Directory.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="44c3e-141">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="44c3e-142">有关详细信息，请参阅[目录权限](/graph/permissions-reference#directory-permissions)。</span><span class="sxs-lookup"><span data-stu-id="44c3e-142">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="44c3e-143">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="44c3e-143">Find the service principal object by display name</span></span>

<span data-ttu-id="44c3e-144">下面的示例演示如何按显示名称查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="44c3e-144">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="44c3e-145">请求</span><span class="sxs-lookup"><span data-stu-id="44c3e-145">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="44c3e-146">**响应**</span><span class="sxs-lookup"><span data-stu-id="44c3e-146">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="44c3e-147">查找服务主体对象的应用程序 ID</span><span class="sxs-lookup"><span data-stu-id="44c3e-147">Find the service principal object by app ID</span></span>

<span data-ttu-id="44c3e-148">下面的示例演示如何查找服务主体对象的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="44c3e-148">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="44c3e-149">请求</span><span class="sxs-lookup"><span data-stu-id="44c3e-149">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="44c3e-150">响应</span><span class="sxs-lookup"><span data-stu-id="44c3e-150">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="44c3e-151">列出现有同步作业</span><span class="sxs-lookup"><span data-stu-id="44c3e-151">List existing synchronization jobs</span></span>

<span data-ttu-id="44c3e-152">下面的示例演示了如何列出现有同步作业。</span><span class="sxs-lookup"><span data-stu-id="44c3e-152">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="44c3e-153">请求</span><span class="sxs-lookup"><span data-stu-id="44c3e-153">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="44c3e-154">响应</span><span class="sxs-lookup"><span data-stu-id="44c3e-154">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="44c3e-155">获取同步作业状态</span><span class="sxs-lookup"><span data-stu-id="44c3e-155">Get synchronization job status</span></span>
<span data-ttu-id="44c3e-156">下面的示例演示如何获取同步作业的状态。</span><span class="sxs-lookup"><span data-stu-id="44c3e-156">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="44c3e-157">请求</span><span class="sxs-lookup"><span data-stu-id="44c3e-157">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="44c3e-158">响应</span><span class="sxs-lookup"><span data-stu-id="44c3e-158">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="44c3e-159">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="44c3e-159">Get synchronization schema</span></span>
<span data-ttu-id="44c3e-160">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="44c3e-160">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="44c3e-161">请求</span><span class="sxs-lookup"><span data-stu-id="44c3e-161">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="44c3e-162">响应</span><span class="sxs-lookup"><span data-stu-id="44c3e-162">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="44c3e-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="44c3e-163">See also</span></span>

* [<span data-ttu-id="44c3e-164">配置与目录的扩展属性同步</span><span class="sxs-lookup"><span data-stu-id="44c3e-164">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="44c3e-165">配置与自定义目标属性同步</span><span class="sxs-lookup"><span data-stu-id="44c3e-165">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
