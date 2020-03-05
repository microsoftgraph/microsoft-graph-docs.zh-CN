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
# <a name="azure-ad-synchronization-api-overview"></a>Azure AD 同步 API 概述

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory （Azure AD）标识同步（也称为 "设置"）允许您自动创建、维护和删除云中的标识（软件即服务或 SaaS）应用程序（如 Dropbox、Salesforce、ServiceNow）等等。 您可以使用 Microsoft Graph 中的同步 Api 以编程方式管理标识同步，包括：

- 创建、启动和停止同步作业
- 对作业的同步架构进行更改
- 验证当前同步状态

有关 Azure AD 中的同步的详细信息，请参阅：

* [使用 Azure Active Directory 实现用户预配和预配到 SaaS 应用程序的自动化](/azure/active-directory/active-directory-saas-app-provisioning)
* [在 Azure 门户中管理企业应用的用户帐户设置](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

您还可以在示例租户或您自己的租户中的[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中尝试 API。

## <a name="synchronization-job"></a>同步作业

同步作业通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。 同步作业始终特定于租户中的应用程序的特定实例。 作为同步作业安装程序的一部分，您需要授予在目标目录中读取和写入对象的权限，并自定义作业的同步架构。

有关详细信息，请参阅[同步作业](synchronization-synchronizationjob.md)。

## <a name="synchronization-schema"></a>同步架构

同步架构定义哪些对象将被同步以及它们的同步方式。 同步架构包含特定同步作业的大部分安装信息。 通常情况下，您将自定义一些[属性映射](synchronization-attributemapping.md)，或添加[作用域筛选器](synchronization-filter.md)以仅同步满足特定条件的对象。

同步架构包括以下组件：

- 目录定义
- 同步规则
- 对象映射

有关详细信息，请参阅[同步架构](synchronization-synchronizationschema.md)。

## <a name="synchronization-template"></a>同步模板

同步模板为特定应用程序提供了预配置的同步设置。 默认情况下，这些设置（最重要的[同步架构](synchronization-synchronizationschema.md)）将用于任何基于该模板的[同步作业](synchronization-synchronizationjob.md)。 模板由应用程序开发人员指定。

有关详细信息，请参阅[同步模板](synchronization-synchronizationtemplate.md)。

## <a name="working-with-the-synchronization-api"></a>使用同步 API

使用同步 API 主要涉及访问[synchronizationJob](synchronization-synchronizationjob.md)和[synchronizationSchema](synchronization-synchronizationschema.md)资源。 若要查找您的[synchronizationJob](synchronization-synchronizationjob.md)资源，您需要知道同步作业所属的服务主体对象的 ID。 下面的示例展示了如何使用**synchronizationJob**和**synchronizationSchema**资源。

### <a name="authorization"></a>Authorization

Azure AD 同步 API 使用 OAuth 2.0 进行授权。 在向 API 发出任何请求之前，你需要获取访问令牌。 有关详细信息，请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。 若要访问同步资源，应用程序需要使用目录 ReadWrite。所有权限。 有关详细信息，请参阅[Directory 权限](/graph/permissions-reference#directory-permissions)。

### <a name="find-the-service-principal-object-by-display-name"></a>按显示名称查找服务主体对象

下面的示例展示了如何按显示名称查找服务主体对象。

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

下面的示例演示如何按应用 ID 查找服务主体对象。

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

下面的示例演示如何列出现有的同步作业。

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
下面的示例演示如何获取同步作业的状态。

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
下面的示例演示如何获取同步架构。

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



