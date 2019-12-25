---
title: Azure AD 同步 API 概述
description: ）允许您自动创建、维护和删除云（软件作为服务或 SaaS）应用程序（如 Dropbox、Salesforce、ServiceNow 等）中的标识。 您可以使用 Microsoft Graph 中的同步 Api 以编程方式管理标识同步，包括：
localization_priority: Normal
doc_type: conceptualPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7e2e64f72c52a6f571b8b97cde643441d8837eda
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866544"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="8ea86-104">Azure AD 同步 API 概述</span><span class="sxs-lookup"><span data-stu-id="8ea86-104">Azure AD synchronization API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ea86-105">Azure Active Directory （Azure AD）标识同步（也称为 "设置"）允许您自动创建、维护和删除云中的标识（软件即服务或 SaaS）应用程序（如 Dropbox、Salesforce、ServiceNow）等等。</span><span class="sxs-lookup"><span data-stu-id="8ea86-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="8ea86-106">您可以使用 Microsoft Graph 中的同步 Api 以编程方式管理标识同步，包括：</span><span class="sxs-lookup"><span data-stu-id="8ea86-106">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="8ea86-107">创建、启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="8ea86-107">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="8ea86-108">对作业的同步架构进行更改</span><span class="sxs-lookup"><span data-stu-id="8ea86-108">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="8ea86-109">验证当前同步状态</span><span class="sxs-lookup"><span data-stu-id="8ea86-109">Verify the current synchronization status</span></span>

<span data-ttu-id="8ea86-110">有关 Azure AD 中的同步的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="8ea86-110">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="8ea86-111">使用 Azure Active Directory 实现用户预配和预配到 SaaS 应用程序的自动化</span><span class="sxs-lookup"><span data-stu-id="8ea86-111">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="8ea86-112">在 Azure 门户中管理企业应用的用户帐户设置</span><span class="sxs-lookup"><span data-stu-id="8ea86-112">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="8ea86-113">您还可以在示例租户或您自己的租户中的[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中尝试 API。</span><span class="sxs-lookup"><span data-stu-id="8ea86-113">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="8ea86-114">同步作业</span><span class="sxs-lookup"><span data-stu-id="8ea86-114">Synchronization job</span></span>

<span data-ttu-id="8ea86-115">同步作业通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。</span><span class="sxs-lookup"><span data-stu-id="8ea86-115">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="8ea86-116">同步作业始终特定于租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="8ea86-116">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="8ea86-117">作为同步作业安装程序的一部分，您需要授予在目标目录中读取和写入对象的权限，并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="8ea86-117">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="8ea86-118">有关详细信息，请参阅[同步作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="8ea86-118">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="8ea86-119">同步架构</span><span class="sxs-lookup"><span data-stu-id="8ea86-119">Synchronization schema</span></span>

<span data-ttu-id="8ea86-120">同步架构定义哪些对象将被同步以及它们的同步方式。</span><span class="sxs-lookup"><span data-stu-id="8ea86-120">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="8ea86-121">同步架构包含特定同步作业的大部分安装信息。</span><span class="sxs-lookup"><span data-stu-id="8ea86-121">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="8ea86-122">通常情况下，您将自定义一些[属性映射](synchronization-attributemapping.md)，或添加[作用域筛选器](synchronization-filter.md)以仅同步满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="8ea86-122">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="8ea86-123">同步架构包括以下组件：</span><span class="sxs-lookup"><span data-stu-id="8ea86-123">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="8ea86-124">目录定义</span><span class="sxs-lookup"><span data-stu-id="8ea86-124">Directory definitions</span></span>
- <span data-ttu-id="8ea86-125">同步规则</span><span class="sxs-lookup"><span data-stu-id="8ea86-125">Synchronization rules</span></span>
- <span data-ttu-id="8ea86-126">对象映射</span><span class="sxs-lookup"><span data-stu-id="8ea86-126">Object mappings</span></span>

<span data-ttu-id="8ea86-127">有关详细信息，请参阅[同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="8ea86-127">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="8ea86-128">同步模板</span><span class="sxs-lookup"><span data-stu-id="8ea86-128">Synchronization template</span></span>

<span data-ttu-id="8ea86-129">同步模板为特定应用程序提供了预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="8ea86-129">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="8ea86-130">默认情况下，这些设置（最重要的[同步架构](synchronization-synchronizationschema.md)）将用于任何基于该模板的[同步作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="8ea86-130">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="8ea86-131">模板由应用程序开发人员指定。</span><span class="sxs-lookup"><span data-stu-id="8ea86-131">Templates are specified by the application developer.</span></span>

<span data-ttu-id="8ea86-132">有关详细信息，请参阅[同步模板](synchronization-synchronizationtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="8ea86-132">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="8ea86-133">使用同步 API</span><span class="sxs-lookup"><span data-stu-id="8ea86-133">Working with the synchronization API</span></span>

<span data-ttu-id="8ea86-134">使用同步 API 主要涉及访问[synchronizationJob](synchronization-synchronizationjob.md)和[synchronizationSchema](synchronization-synchronizationschema.md)资源。</span><span class="sxs-lookup"><span data-stu-id="8ea86-134">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="8ea86-135">若要查找您的[synchronizationJob](synchronization-synchronizationjob.md)资源，您需要知道同步作业所属的服务主体对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="8ea86-135">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="8ea86-136">下面的示例展示了如何使用**synchronizationJob**和**synchronizationSchema**资源。</span><span class="sxs-lookup"><span data-stu-id="8ea86-136">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="8ea86-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ea86-137">Authorization</span></span>

<span data-ttu-id="8ea86-138">Azure AD 同步 API 使用 OAuth 2.0 进行授权。</span><span class="sxs-lookup"><span data-stu-id="8ea86-138">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="8ea86-139">在向 API 发出任何请求之前，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="8ea86-139">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="8ea86-140">有关详细信息，请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="8ea86-140">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="8ea86-141">若要访问同步资源，应用程序需要使用目录 ReadWrite。所有权限。</span><span class="sxs-lookup"><span data-stu-id="8ea86-141">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="8ea86-142">有关详细信息，请参阅[Directory 权限](/graph/permissions-reference#directory-permissions)。</span><span class="sxs-lookup"><span data-stu-id="8ea86-142">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="8ea86-143">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="8ea86-143">Find the service principal object by display name</span></span>

<span data-ttu-id="8ea86-144">下面的示例展示了如何按显示名称查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="8ea86-144">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="8ea86-145">**请求**</span><span class="sxs-lookup"><span data-stu-id="8ea86-145">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="8ea86-146">**响应**</span><span class="sxs-lookup"><span data-stu-id="8ea86-146">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="8ea86-147">按应用 ID 查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="8ea86-147">Find the service principal object by app ID</span></span>

<span data-ttu-id="8ea86-148">下面的示例演示如何按应用 ID 查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="8ea86-148">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="8ea86-149">**请求**</span><span class="sxs-lookup"><span data-stu-id="8ea86-149">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="8ea86-150">**响应**</span><span class="sxs-lookup"><span data-stu-id="8ea86-150">**Response**</span></span>
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="8ea86-151">列出现有同步作业</span><span class="sxs-lookup"><span data-stu-id="8ea86-151">List existing synchronization jobs</span></span>

<span data-ttu-id="8ea86-152">下面的示例演示如何列出现有的同步作业。</span><span class="sxs-lookup"><span data-stu-id="8ea86-152">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="8ea86-153">**请求**</span><span class="sxs-lookup"><span data-stu-id="8ea86-153">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="8ea86-154">**响应**</span><span class="sxs-lookup"><span data-stu-id="8ea86-154">**Response**</span></span>
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="8ea86-155">获取同步作业状态</span><span class="sxs-lookup"><span data-stu-id="8ea86-155">Get synchronization job status</span></span>
<span data-ttu-id="8ea86-156">下面的示例演示如何获取同步作业的状态。</span><span class="sxs-lookup"><span data-stu-id="8ea86-156">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="8ea86-157">**请求**</span><span class="sxs-lookup"><span data-stu-id="8ea86-157">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="8ea86-158">**响应**</span><span class="sxs-lookup"><span data-stu-id="8ea86-158">**Response**</span></span>
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="8ea86-159">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="8ea86-159">Get synchronization schema</span></span>
<span data-ttu-id="8ea86-160">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="8ea86-160">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="8ea86-161">**请求**</span><span class="sxs-lookup"><span data-stu-id="8ea86-161">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="8ea86-162">**响应**</span><span class="sxs-lookup"><span data-stu-id="8ea86-162">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="8ea86-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8ea86-163">See also</span></span>

* [<span data-ttu-id="8ea86-164">配置与目录扩展属性的同步</span><span class="sxs-lookup"><span data-stu-id="8ea86-164">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="8ea86-165">配置与自定义目标属性的同步</span><span class="sxs-lookup"><span data-stu-id="8ea86-165">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



