---
title: Azure AD 同步 API 概述
description: ) 可自动执行创建、 维护和删除中的标识云 （软件作为服务，还是 SaaS） 应用程序，如收存箱、 销售队伍、 ServiceNow，等等。 您可以使用同步 Api 在 Microsoft Graph 中以编程方式管理标识同步包括：
localization_priority: Normal
ms.openlocfilehash: aada94f39c67fb1174924d49c6e57650f4961cc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884684"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="381fb-104">Azure AD 同步 API 概述</span><span class="sxs-lookup"><span data-stu-id="381fb-104">Azure AD synchronization API overview</span></span>

> <span data-ttu-id="381fb-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="381fb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="381fb-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="381fb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="381fb-107">Azure Active Directory (Azure AD) 标识同步 （也称为"设置"），可以自动执行创建、 维护和删除云 （软件作为服务，还是 SaaS） 中的标识收存箱、 销售队伍 ServiceNow，如应用程序等等。</span><span class="sxs-lookup"><span data-stu-id="381fb-107">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="381fb-108">您可以使用同步 Api 在 Microsoft Graph 中以编程方式管理标识同步包括：</span><span class="sxs-lookup"><span data-stu-id="381fb-108">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="381fb-109">创建、 启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="381fb-109">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="381fb-110">更改作业的同步架构</span><span class="sxs-lookup"><span data-stu-id="381fb-110">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="381fb-111">验证当前的同步状态</span><span class="sxs-lookup"><span data-stu-id="381fb-111">Verify the current synchronization status</span></span> 

<span data-ttu-id="381fb-112">有关在 Azure AD 的同步的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="381fb-112">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="381fb-113">自动化用户设置和解除设置 SaaS 与 Azure Active Directory 的应用程序</span><span class="sxs-lookup"><span data-stu-id="381fb-113">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="381fb-114">管理用户帐户设置 Azure 门户中的企业应用程序</span><span class="sxs-lookup"><span data-stu-id="381fb-114">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="381fb-115">您还可以尝试示例租户或您自己的租户中的[图资源管理器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="381fb-115">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="381fb-116">同步作业</span><span class="sxs-lookup"><span data-stu-id="381fb-116">Synchronization job</span></span>

<span data-ttu-id="381fb-117">同步作业执行同步在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改。</span><span class="sxs-lookup"><span data-stu-id="381fb-117">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="381fb-118">同步作业始终是特定于您的租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="381fb-118">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="381fb-119">作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。</span><span class="sxs-lookup"><span data-stu-id="381fb-119">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="381fb-120">有关详细信息，请参阅[同步作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="381fb-120">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="381fb-121">同步架构</span><span class="sxs-lookup"><span data-stu-id="381fb-121">Synchronization schema</span></span>

<span data-ttu-id="381fb-122">同步架构定义对象将同步和同步方式。</span><span class="sxs-lookup"><span data-stu-id="381fb-122">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="381fb-123">同步架构包含特定同步作业的设置信息的大部分。</span><span class="sxs-lookup"><span data-stu-id="381fb-123">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="381fb-124">通常情况下，您将自定义某些[属性映射](synchronization-attributemapping.md)，或添加[范围筛选器](synchronization-filter.md)以同步只有满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="381fb-124">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="381fb-125">同步架构包括以下组件：</span><span class="sxs-lookup"><span data-stu-id="381fb-125">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="381fb-126">目录定义</span><span class="sxs-lookup"><span data-stu-id="381fb-126">Directory definitions</span></span>
- <span data-ttu-id="381fb-127">同步规则</span><span class="sxs-lookup"><span data-stu-id="381fb-127">Synchronization rules</span></span>
- <span data-ttu-id="381fb-128">对象映射</span><span class="sxs-lookup"><span data-stu-id="381fb-128">Object mappings</span></span>

<span data-ttu-id="381fb-129">有关详细信息，请参阅[同步 schema](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="381fb-129">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="381fb-130">同步模板</span><span class="sxs-lookup"><span data-stu-id="381fb-130">Synchronization template</span></span>

<span data-ttu-id="381fb-131">同步模板提供了为特定应用程序预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="381fb-131">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="381fb-132">将基于模板的任何[同步作业，](synchronization-synchronizationjob.md)默认情况下使用这些设置 （最重要的是[同步架构](synchronization-synchronizationschema.md)）。</span><span class="sxs-lookup"><span data-stu-id="381fb-132">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="381fb-133">由应用程序开发人员指定模板。</span><span class="sxs-lookup"><span data-stu-id="381fb-133">Templates are specified by the application developer.</span></span>

<span data-ttu-id="381fb-134">有关详细信息，请参阅[同步模板](synchronization-synchronizationtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="381fb-134">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="381fb-135">使用同步 API</span><span class="sxs-lookup"><span data-stu-id="381fb-135">Working with the synchronization API</span></span>

<span data-ttu-id="381fb-136">使用同步 API 主要涉及访问[synchronizationJob](synchronization-synchronizationjob.md)和[synchronizationSchema](synchronization-synchronizationschema.md)资源。</span><span class="sxs-lookup"><span data-stu-id="381fb-136">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="381fb-137">若要找到[synchronizationJob](synchronization-synchronizationjob.md)资源，您需要知道同步作业所属的服务主体对象 ID。</span><span class="sxs-lookup"><span data-stu-id="381fb-137">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="381fb-138">下面的示例演示如何使用**synchronizationJob**和**synchronizationSchema**资源。</span><span class="sxs-lookup"><span data-stu-id="381fb-138">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="381fb-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="381fb-139">Authorization</span></span>

<span data-ttu-id="381fb-140">Azure AD 同步 API 使用 OAuth 2.0 授权。</span><span class="sxs-lookup"><span data-stu-id="381fb-140">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="381fb-141">Api 任何请求之前，您需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="381fb-141">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="381fb-142">有关详细信息，请参阅[获取访问令牌调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="381fb-142">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="381fb-143">若要访问同步资源，您的应用程序需要 Directory.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="381fb-143">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="381fb-144">有关详细信息，请参阅[目录权限](/graph/permissions-reference#directory-permissions)。</span><span class="sxs-lookup"><span data-stu-id="381fb-144">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="381fb-145">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="381fb-145">Find the service principal object by display name</span></span>

<span data-ttu-id="381fb-146">下面的示例演示如何按显示名称查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="381fb-146">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="381fb-147">**请求**</span><span class="sxs-lookup"><span data-stu-id="381fb-147">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="381fb-148">**响应**</span><span class="sxs-lookup"><span data-stu-id="381fb-148">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="381fb-149">查找服务主体对象的应用程序 ID</span><span class="sxs-lookup"><span data-stu-id="381fb-149">Find the service principal object by app ID</span></span>

<span data-ttu-id="381fb-150">下面的示例演示如何查找服务主体对象的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="381fb-150">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="381fb-151">**请求** 
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-151">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="381fb-152">**响应**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-152">**Response**
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="381fb-153">列出现有同步作业</span><span class="sxs-lookup"><span data-stu-id="381fb-153">List existing synchronization jobs</span></span>

<span data-ttu-id="381fb-154">下面的示例演示了如何列出现有同步作业。</span><span class="sxs-lookup"><span data-stu-id="381fb-154">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="381fb-155">**请求**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-155">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="381fb-156">**响应**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-156">**Response**
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="381fb-157">获取同步作业状态</span><span class="sxs-lookup"><span data-stu-id="381fb-157">Get synchronization job status</span></span>
<span data-ttu-id="381fb-158">下面的示例演示如何获取同步作业的状态。</span><span class="sxs-lookup"><span data-stu-id="381fb-158">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="381fb-159">**请求**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-159">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="381fb-160">**响应**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-160">**Response**
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="381fb-161">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="381fb-161">Get synchronization schema</span></span>
<span data-ttu-id="381fb-162">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="381fb-162">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="381fb-163">**请求**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-163">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="381fb-164">**响应**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="381fb-164">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="381fb-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="381fb-165">See also</span></span>

* [<span data-ttu-id="381fb-166">配置与目录的扩展属性同步</span><span class="sxs-lookup"><span data-stu-id="381fb-166">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="381fb-167">配置与自定义目标属性同步</span><span class="sxs-lookup"><span data-stu-id="381fb-167">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



