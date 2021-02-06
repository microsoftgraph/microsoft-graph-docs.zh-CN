---
title: Azure AD 同步 API 概述
description: 自动设置从 HR 系统、Active Directory 和 Azure Active Directory 到云应用程序的标识。
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a08be511c3752e27f2e86415aee62d112d2c5262
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133159"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="da7ba-103">Azure AD 同步 API 概述</span><span class="sxs-lookup"><span data-stu-id="da7ba-103">Azure AD synchronization API overview</span></span>

<span data-ttu-id="da7ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da7ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da7ba-105">Azure Active Directory (Azure AD) 标识同步 (也称为"预配")  (允许你自动从以下任一项创建、维护) 和取消预配 () 标识：</span><span class="sxs-lookup"><span data-stu-id="da7ba-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the provisioning (creation, maintenance) and de-provisioning (removal) of identities from any of the following:</span></span>
- <span data-ttu-id="da7ba-106">Active Directory 到 Azure AD</span><span class="sxs-lookup"><span data-stu-id="da7ba-106">Active Directory to Azure AD</span></span>
- <span data-ttu-id="da7ba-107">工作日到 Azure AD</span><span class="sxs-lookup"><span data-stu-id="da7ba-107">Workday to Azure AD</span></span>
- <span data-ttu-id="da7ba-108">Azure AD 到云应用程序，如 Dropbox、Salesforce、ServiceNow 等</span><span class="sxs-lookup"><span data-stu-id="da7ba-108">Azure AD to cloud applications such as Dropbox, Salesforce, ServiceNow, and more</span></span> 

<span data-ttu-id="da7ba-109">可使用 Microsoft Graph 中的同步 API 以编程方式管理标识同步，包括：</span><span class="sxs-lookup"><span data-stu-id="da7ba-109">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="da7ba-110">创建、启动和停止同步作业</span><span class="sxs-lookup"><span data-stu-id="da7ba-110">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="da7ba-111">对作业的同步架构进行更改</span><span class="sxs-lookup"><span data-stu-id="da7ba-111">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="da7ba-112">验证当前同步状态</span><span class="sxs-lookup"><span data-stu-id="da7ba-112">Verify the current synchronization status</span></span>

<span data-ttu-id="da7ba-113">有关 Azure AD 中的同步详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="da7ba-113">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="da7ba-114">使用 Azure Active Directory 自动为 SaaS 应用程序设置和取消设置用户</span><span class="sxs-lookup"><span data-stu-id="da7ba-114">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="da7ba-115">在 Azure 门户中管理企业应用的用户帐户设置</span><span class="sxs-lookup"><span data-stu-id="da7ba-115">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="da7ba-116">还可以在示例租户或你自己的租户 [中试用 Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 中的 API。</span><span class="sxs-lookup"><span data-stu-id="da7ba-116">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="da7ba-117">同步作业</span><span class="sxs-lookup"><span data-stu-id="da7ba-117">Synchronization job</span></span>

<span data-ttu-id="da7ba-118">同步作业通过定期在后台运行、轮询一个目录中的更改，以及将它们推送到另一个目录来执行同步。</span><span class="sxs-lookup"><span data-stu-id="da7ba-118">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="da7ba-119">同步作业始终特定于租户中应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="da7ba-119">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="da7ba-120">作为同步作业设置的一部分，您需要授权读取和写入目标目录中的对象，并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="da7ba-120">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="da7ba-121">有关详细信息，请参阅同步 [作业](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="da7ba-121">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="da7ba-122">同步架构</span><span class="sxs-lookup"><span data-stu-id="da7ba-122">Synchronization schema</span></span>

<span data-ttu-id="da7ba-123">同步架构定义将同步哪些对象以及如何同步它们。</span><span class="sxs-lookup"><span data-stu-id="da7ba-123">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="da7ba-124">同步架构包含特定同步作业的多数设置信息。</span><span class="sxs-lookup"><span data-stu-id="da7ba-124">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="da7ba-125">通常，您将自定义某些[属性](synchronization-attributemapping.md)映射，或添加范围筛选器以仅同步满足[](synchronization-filter.md)特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="da7ba-125">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="da7ba-126">同步架构包括以下组件：</span><span class="sxs-lookup"><span data-stu-id="da7ba-126">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="da7ba-127">目录定义</span><span class="sxs-lookup"><span data-stu-id="da7ba-127">Directory definitions</span></span>
- <span data-ttu-id="da7ba-128">同步规则</span><span class="sxs-lookup"><span data-stu-id="da7ba-128">Synchronization rules</span></span>
- <span data-ttu-id="da7ba-129">对象映射</span><span class="sxs-lookup"><span data-stu-id="da7ba-129">Object mappings</span></span>

<span data-ttu-id="da7ba-130">有关详细信息，请参阅 [同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="da7ba-130">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="da7ba-131">同步模板</span><span class="sxs-lookup"><span data-stu-id="da7ba-131">Synchronization template</span></span>

<span data-ttu-id="da7ba-132">同步模板为特定应用程序提供预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="da7ba-132">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="da7ba-133">这些设置 (，默认情况下，) 模板的任何同步作业[](synchronization-synchronizationschema.md)都将使用同步架构模板。 [](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="da7ba-133">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="da7ba-134">模板由应用程序开发人员指定。</span><span class="sxs-lookup"><span data-stu-id="da7ba-134">Templates are specified by the application developer.</span></span>

<span data-ttu-id="da7ba-135">有关详细信息，请参阅同步 [模板](synchronization-synchronizationtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="da7ba-135">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="da7ba-136">使用同步 API</span><span class="sxs-lookup"><span data-stu-id="da7ba-136">Working with the synchronization API</span></span>

<span data-ttu-id="da7ba-137">使用同步 API 主要涉及访问 [synchronizationJob 和](synchronization-synchronizationjob.md) [synchronizationSchema](synchronization-synchronizationschema.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="da7ba-137">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="da7ba-138">若要查找 [synchronizationJob](synchronization-synchronizationjob.md) 资源，您需要知道同步作业所属的服务主体对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="da7ba-138">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="da7ba-139">以下示例显示如何使用 **synchronizationJob** 和 **synchronizationSchema** 资源。</span><span class="sxs-lookup"><span data-stu-id="da7ba-139">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="da7ba-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="da7ba-140">Authorization</span></span>

<span data-ttu-id="da7ba-141">Azure AD 同步 API 使用 OAuth 2.0 进行授权。</span><span class="sxs-lookup"><span data-stu-id="da7ba-141">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="da7ba-142">在向 API 提出任何请求之前，你需要获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="da7ba-142">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="da7ba-143">有关详细信息，请参阅[获取访问令牌以调用 Microsoft Graph。](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="da7ba-143">For more information, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span> <span data-ttu-id="da7ba-144">若要访问同步资源，应用程序需要 Directory.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="da7ba-144">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="da7ba-145">有关详细信息，请参阅 [目录权限](/graph/permissions-reference#directory-permissions)。</span><span class="sxs-lookup"><span data-stu-id="da7ba-145">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="da7ba-146">按以下方法查找服务主体显示名称</span><span class="sxs-lookup"><span data-stu-id="da7ba-146">Find the service principal object by display name</span></span>

<span data-ttu-id="da7ba-147">以下示例显示如何按以下方法查找服务主体显示名称。</span><span class="sxs-lookup"><span data-stu-id="da7ba-147">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="da7ba-148">**请求**</span><span class="sxs-lookup"><span data-stu-id="da7ba-148">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="da7ba-149">**响应**</span><span class="sxs-lookup"><span data-stu-id="da7ba-149">**Response**</span></span>

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

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="da7ba-150">按应用 ID 查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="da7ba-150">Find the service principal object by app ID</span></span>

<span data-ttu-id="da7ba-151">以下示例演示如何按应用 ID 查找服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="da7ba-151">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="da7ba-152">**请求**</span><span class="sxs-lookup"><span data-stu-id="da7ba-152">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="da7ba-153">**响应**</span><span class="sxs-lookup"><span data-stu-id="da7ba-153">**Response**</span></span>
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

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="da7ba-154">列出现有同步作业</span><span class="sxs-lookup"><span data-stu-id="da7ba-154">List existing synchronization jobs</span></span>

<span data-ttu-id="da7ba-155">以下示例演示如何列出现有同步作业。</span><span class="sxs-lookup"><span data-stu-id="da7ba-155">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="da7ba-156">**请求**</span><span class="sxs-lookup"><span data-stu-id="da7ba-156">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="da7ba-157">**响应**</span><span class="sxs-lookup"><span data-stu-id="da7ba-157">**Response**</span></span>
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

### <a name="get-synchronization-job-status"></a><span data-ttu-id="da7ba-158">获取同步作业状态</span><span class="sxs-lookup"><span data-stu-id="da7ba-158">Get synchronization job status</span></span>
<span data-ttu-id="da7ba-159">以下示例演示如何获取同步作业的状态。</span><span class="sxs-lookup"><span data-stu-id="da7ba-159">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="da7ba-160">**请求**</span><span class="sxs-lookup"><span data-stu-id="da7ba-160">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="da7ba-161">**响应**</span><span class="sxs-lookup"><span data-stu-id="da7ba-161">**Response**</span></span>
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

### <a name="get-synchronization-schema"></a><span data-ttu-id="da7ba-162">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="da7ba-162">Get synchronization schema</span></span>
<span data-ttu-id="da7ba-163">以下示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="da7ba-163">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="da7ba-164">**请求**</span><span class="sxs-lookup"><span data-stu-id="da7ba-164">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="da7ba-165">**响应**</span><span class="sxs-lookup"><span data-stu-id="da7ba-165">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="da7ba-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="da7ba-166">See also</span></span>

* [<span data-ttu-id="da7ba-167">配置与目录扩展属性的同步</span><span class="sxs-lookup"><span data-stu-id="da7ba-167">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="da7ba-168">配置与自定义目标属性的同步</span><span class="sxs-lookup"><span data-stu-id="da7ba-168">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)
