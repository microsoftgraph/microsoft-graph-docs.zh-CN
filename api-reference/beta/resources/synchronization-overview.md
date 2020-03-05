---
title: Azure AD 同步 API 概述
description: ）允许您自动创建、维护和删除云（软件作为服务或 SaaS）应用程序（如 Dropbox、Salesforce、ServiceNow 等）中的标识。 您可以使用 Microsoft Graph 中的同步 Api 以编程方式管理标识同步，包括：
localization_priority: Normal
doc_type: conceptualPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62c127b632277a93312afd7682939049b1e9de68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520140"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="562f0-104">Azure AD 同步 API 概述</span><span class="sxs-lookup"><span data-stu-id="562f0-104">Azure AD synchronization API overview</span></span>

<span data-ttu-id="562f0-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="562f0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="562f0-106">Azure Active Directory （Azure AD）标识同步（也称为 "设置"）允许您自动创建、维护和删除云中的标识（软件即服务或 SaaS）应用程序（如 Dropbox、Salesforce、ServiceNow）等等。</span><span class="sxs-lookup"><span data-stu-id="562f0-106">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="562f0-107">您可以使用 Microsoft Graph 中的同步 Api 以编程方式管理标识同步，包括：</span><span class="sxs-lookup"><span data-stu-id="562f0-107">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="562f0-108">创建、启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="562f0-108">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="562f0-109">对作业的同步架构进行更改</span><span class="sxs-lookup"><span data-stu-id="562f0-109">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="562f0-110">验证当前同步状态</span><span class="sxs-lookup"><span data-stu-id="562f0-110">Verify the current synchronization status</span></span>

<span data-ttu-id="562f0-111">有关 Azure AD 中的同步的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="562f0-111">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="562f0-112">使用 Azure Active Directory 实现用户预配和预配到 SaaS 应用程序的自动化</span><span class="sxs-lookup"><span data-stu-id="562f0-112">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="562f0-113">在 Azure 门户中管理企业应用的用户帐户设置</span><span class="sxs-lookup"><span data-stu-id="562f0-113">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="562f0-114">您还可以在示例租户或您自己的租户中的[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中尝试 API。</span><span class="sxs-lookup"><span data-stu-id="562f0-114">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="562f0-115">同步作业</span><span class="sxs-lookup"><span data-stu-id="562f0-115">Synchronization job</span></span>

<span data-ttu-id="562f0-116">同步作业通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。</span><span class="sxs-lookup"><span data-stu-id="562f0-116">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="562f0-117">同步作业始终特定于租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="562f0-117">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="562f0-118">作为同步作业安装程序的一部分，您需要授予在目标目录中读取和写入对象的权限，并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="562f0-118">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="562f0-119">有关详细信息，请参阅[同步作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="562f0-119">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="562f0-120">同步架构</span><span class="sxs-lookup"><span data-stu-id="562f0-120">Synchronization schema</span></span>

<span data-ttu-id="562f0-121">同步架构定义哪些对象将被同步以及它们的同步方式。</span><span class="sxs-lookup"><span data-stu-id="562f0-121">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="562f0-122">同步架构包含特定同步作业的大部分安装信息。</span><span class="sxs-lookup"><span data-stu-id="562f0-122">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="562f0-123">通常情况下，您将自定义一些[属性映射](synchronization-attributemapping.md)，或添加[作用域筛选器](synchronization-filter.md)以仅同步满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="562f0-123">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="562f0-124">同步架构包括以下组件：</span><span class="sxs-lookup"><span data-stu-id="562f0-124">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="562f0-125">目录定义</span><span class="sxs-lookup"><span data-stu-id="562f0-125">Directory definitions</span></span>
- <span data-ttu-id="562f0-126">同步规则</span><span class="sxs-lookup"><span data-stu-id="562f0-126">Synchronization rules</span></span>
- <span data-ttu-id="562f0-127">对象映射</span><span class="sxs-lookup"><span data-stu-id="562f0-127">Object mappings</span></span>

<span data-ttu-id="562f0-128">有关详细信息，请参阅[同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="562f0-128">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="562f0-129">同步模板</span><span class="sxs-lookup"><span data-stu-id="562f0-129">Synchronization template</span></span>

<span data-ttu-id="562f0-130">同步模板为特定应用程序提供了预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="562f0-130">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="562f0-131">默认情况下，这些设置（最重要的[同步架构](synchronization-synchronizationschema.md)）将用于任何基于该模板的[同步作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="562f0-131">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="562f0-132">模板由应用程序开发人员指定。</span><span class="sxs-lookup"><span data-stu-id="562f0-132">Templates are specified by the application developer.</span></span>

<span data-ttu-id="562f0-133">有关详细信息，请参阅[同步模板](synchronization-synchronizationtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="562f0-133">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="562f0-134">使用同步 API</span><span class="sxs-lookup"><span data-stu-id="562f0-134">Working with the synchronization API</span></span>

<span data-ttu-id="562f0-135">使用同步 API 主要涉及访问[synchronizationJob](synchronization-synchronizationjob.md)和[synchronizationSchema](synchronization-synchronizationschema.md)资源。</span><span class="sxs-lookup"><span data-stu-id="562f0-135">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="562f0-136">若要查找您的[synchronizationJob](synchronization-synchronizationjob.md)资源，您需要知道同步作业所属的服务主体对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="562f0-136">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="562f0-137">下面的示例展示了如何使用**synchronizationJob**和**synchronizationSchema**资源。</span><span class="sxs-lookup"><span data-stu-id="562f0-137">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="562f0-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="562f0-138">Authorization</span></span>

<span data-ttu-id="562f0-139">Azure AD 同步 API 使用 OAuth 2.0 进行授权。</span><span class="sxs-lookup"><span data-stu-id="562f0-139">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="562f0-140">在向 API 发出任何请求之前，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="562f0-140">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="562f0-141">有关详细信息，请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="562f0-141">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="562f0-142">若要访问同步资源，应用程序需要使用目录 ReadWrite。所有权限。</span><span class="sxs-lookup"><span data-stu-id="562f0-142">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="562f0-143">有关详细信息，请参阅[Directory 权限](/graph/permissions-reference#directory-permissions)。</span><span class="sxs-lookup"><span data-stu-id="562f0-143">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="562f0-144">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="562f0-144">Find the service principal object by display name</span></span>

<span data-ttu-id="562f0-145">下面的示例展示了如何按显示名称查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="562f0-145">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="562f0-146">**请求**</span><span class="sxs-lookup"><span data-stu-id="562f0-146">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="562f0-147">**响应**</span><span class="sxs-lookup"><span data-stu-id="562f0-147">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="562f0-148">按应用 ID 查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="562f0-148">Find the service principal object by app ID</span></span>

<span data-ttu-id="562f0-149">下面的示例演示如何按应用 ID 查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="562f0-149">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="562f0-150">**请求**</span><span class="sxs-lookup"><span data-stu-id="562f0-150">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="562f0-151">**响应**</span><span class="sxs-lookup"><span data-stu-id="562f0-151">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="562f0-152">列出现有同步作业</span><span class="sxs-lookup"><span data-stu-id="562f0-152">List existing synchronization jobs</span></span>

<span data-ttu-id="562f0-153">下面的示例演示如何列出现有的同步作业。</span><span class="sxs-lookup"><span data-stu-id="562f0-153">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="562f0-154">**请求**</span><span class="sxs-lookup"><span data-stu-id="562f0-154">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="562f0-155">**响应**</span><span class="sxs-lookup"><span data-stu-id="562f0-155">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="562f0-156">获取同步作业状态</span><span class="sxs-lookup"><span data-stu-id="562f0-156">Get synchronization job status</span></span>
<span data-ttu-id="562f0-157">下面的示例演示如何获取同步作业的状态。</span><span class="sxs-lookup"><span data-stu-id="562f0-157">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="562f0-158">**请求**</span><span class="sxs-lookup"><span data-stu-id="562f0-158">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="562f0-159">**响应**</span><span class="sxs-lookup"><span data-stu-id="562f0-159">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="562f0-160">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="562f0-160">Get synchronization schema</span></span>
<span data-ttu-id="562f0-161">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="562f0-161">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="562f0-162">**请求**</span><span class="sxs-lookup"><span data-stu-id="562f0-162">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="562f0-163">**响应**</span><span class="sxs-lookup"><span data-stu-id="562f0-163">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="562f0-164">另请参阅</span><span class="sxs-lookup"><span data-stu-id="562f0-164">See also</span></span>

* [<span data-ttu-id="562f0-165">配置与目录扩展属性的同步</span><span class="sxs-lookup"><span data-stu-id="562f0-165">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="562f0-166">配置与自定义目标属性的同步</span><span class="sxs-lookup"><span data-stu-id="562f0-166">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



