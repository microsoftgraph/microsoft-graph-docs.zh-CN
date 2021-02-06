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
# <a name="azure-ad-synchronization-api-overview"></a>Azure AD 同步 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 标识同步 (也称为"预配")  (允许你自动从以下任一项创建、维护) 和取消预配 () 标识：
- Active Directory 到 Azure AD
- 工作日到 Azure AD
- Azure AD 到云应用程序，如 Dropbox、Salesforce、ServiceNow 等 

可使用 Microsoft Graph 中的同步 API 以编程方式管理标识同步，包括：

- 创建、启动和停止同步作业
- 对作业的同步架构进行更改
- 验证当前同步状态

有关 Azure AD 中的同步详细信息，请参阅：

* [使用 Azure Active Directory 自动为 SaaS 应用程序设置和取消设置用户](/azure/active-directory/active-directory-saas-app-provisioning)
* [在 Azure 门户中管理企业应用的用户帐户设置](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

还可以在示例租户或你自己的租户 [中试用 Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 中的 API。

## <a name="synchronization-job"></a>同步作业

同步作业通过定期在后台运行、轮询一个目录中的更改，以及将它们推送到另一个目录来执行同步。 同步作业始终特定于租户中应用程序的特定实例。 作为同步作业设置的一部分，您需要授权读取和写入目标目录中的对象，并自定义作业的同步架构。

有关详细信息，请参阅同步 [作业](synchronization-synchronizationjob.md)。

## <a name="synchronization-schema"></a>同步架构

同步架构定义将同步哪些对象以及如何同步它们。 同步架构包含特定同步作业的多数设置信息。 通常，您将自定义某些[属性](synchronization-attributemapping.md)映射，或添加范围筛选器以仅同步满足[](synchronization-filter.md)特定条件的对象。

同步架构包括以下组件：

- 目录定义
- 同步规则
- 对象映射

有关详细信息，请参阅 [同步架构](synchronization-synchronizationschema.md)。

## <a name="synchronization-template"></a>同步模板

同步模板为特定应用程序提供预配置的同步设置。 这些设置 (，默认情况下，) 模板的任何同步作业[](synchronization-synchronizationschema.md)都将使用同步架构模板。 [](synchronization-synchronizationjob.md) 模板由应用程序开发人员指定。

有关详细信息，请参阅同步 [模板](synchronization-synchronizationtemplate.md)。

## <a name="working-with-the-synchronization-api"></a>使用同步 API

使用同步 API 主要涉及访问 [synchronizationJob 和](synchronization-synchronizationjob.md) [synchronizationSchema](synchronization-synchronizationschema.md) 资源。 若要查找 [synchronizationJob](synchronization-synchronizationjob.md) 资源，您需要知道同步作业所属的服务主体对象的 ID。 以下示例显示如何使用 **synchronizationJob** 和 **synchronizationSchema** 资源。

### <a name="authorization"></a>Authorization

Azure AD 同步 API 使用 OAuth 2.0 进行授权。 在向 API 提出任何请求之前，你需要获取访问令牌。 有关详细信息，请参阅[获取访问令牌以调用 Microsoft Graph。](/graph/auth/) 若要访问同步资源，应用程序需要 Directory.ReadWrite.All 权限。 有关详细信息，请参阅 [目录权限](/graph/permissions-reference#directory-permissions)。

### <a name="find-the-service-principal-object-by-display-name"></a>按以下方法查找服务主体显示名称

以下示例显示如何按以下方法查找服务主体显示名称。

**请求**

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

**响应**

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

### <a name="find-the-service-principal-object-by-app-id"></a>按应用 ID 查找服务主体对象

以下示例演示如何按应用 ID 查找服务主体对象。

**请求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

**响应**
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

### <a name="list-existing-synchronization-jobs"></a>列出现有同步作业

以下示例演示如何列出现有同步作业。

**请求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

**响应**
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

### <a name="get-synchronization-job-status"></a>获取同步作业状态
以下示例演示如何获取同步作业的状态。

**请求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

**响应**
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

### <a name="get-synchronization-schema"></a>获取同步架构
以下示例演示如何获取同步架构。

**请求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

**响应**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>另请参阅

* [配置与目录扩展属性的同步](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [配置与自定义目标属性的同步](../resources/synchronization-configure-with-custom-target-attributes.md)
