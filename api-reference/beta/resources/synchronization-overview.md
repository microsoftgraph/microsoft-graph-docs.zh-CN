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
# <a name="azure-ad-synchronization-api-overview"></a>Azure AD 同步 API 概述

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 标识同步 （也称为"设置"），可以自动执行创建、 维护和删除云 （软件作为服务，还是 SaaS） 中的标识收存箱、 销售队伍 ServiceNow，如应用程序等等。 您可以使用同步 Api 在 Microsoft Graph 中以编程方式管理标识同步包括：

- 创建、 启动和停止同步作业
- 更改作业的同步架构
- 验证当前的同步状态 

有关在 Azure AD 的同步的详细信息，请参阅：

* [自动化用户设置和解除设置 SaaS 与 Azure Active Directory 的应用程序](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [管理用户帐户设置 Azure 门户中的企业应用程序](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

您还可以尝试示例租户或您自己的租户中的[图资源管理器](https://developer.microsoft.com/graph/graph-explorer)中的 API。

## <a name="synchronization-job"></a>同步作业

同步作业执行同步在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改。 同步作业始终是特定于您的租户中的应用程序的特定实例。 作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。

有关详细信息，请参阅[同步作业](synchronization-synchronizationjob.md)。

## <a name="synchronization-schema"></a>同步架构

同步架构定义对象将同步和同步方式。 同步架构包含特定同步作业的设置信息的大部分。 通常情况下，您将自定义某些[属性映射](synchronization-attributemapping.md)，或添加[范围筛选器](synchronization-filter.md)以同步只有满足特定条件的对象。

同步架构包括以下组件：

- 目录定义
- 同步规则
- 对象映射

有关详细信息，请参阅[同步 schema](synchronization-synchronizationschema.md)。

## <a name="synchronization-template"></a>同步模板

同步模板提供了为特定应用程序预配置的同步设置。 将基于模板的任何[同步作业，](synchronization-synchronizationjob.md)默认情况下使用这些设置 （最重要的是[同步架构](synchronization-synchronizationschema.md)）。 由应用程序开发人员指定模板。

有关详细信息，请参阅[同步模板](synchronization-synchronizationtemplate.md)。

## <a name="working-with-the-synchronization-api"></a>使用同步 API

使用同步 API 主要涉及访问[synchronizationJob](synchronization-synchronizationjob.md)和[synchronizationSchema](synchronization-synchronizationschema.md)资源。 若要找到[synchronizationJob](synchronization-synchronizationjob.md)资源，您需要知道同步作业所属的服务主体对象 ID。 下面的示例演示如何使用**synchronizationJob**和**synchronizationSchema**资源。

### <a name="authorization"></a>Authorization

Azure AD 同步 API 使用 OAuth 2.0 授权。 Api 任何请求之前，您需要获取访问令牌。 有关详细信息，请参阅[获取访问令牌调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。 若要访问同步资源，您的应用程序需要 Directory.ReadWrite.All 权限。 有关详细信息，请参阅[目录权限](/graph/permissions-reference#directory-permissions)。

### <a name="find-the-service-principal-object-by-display-name"></a>按显示名称查找服务主体对象

下面的示例演示如何按显示名称查找服务主体对象。

请求 

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

### <a name="find-the-service-principal-object-by-app-id"></a>查找服务主体对象的应用程序 ID

下面的示例演示如何查找服务主体对象的应用程序 id。

请求
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

响应
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

下面的示例演示了如何列出现有同步作业。

请求
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

响应
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

请求
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

响应
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

请求
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

响应
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>另请参阅

* [配置与目录的扩展属性同步](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [配置与自定义目标属性同步](../resources/synchronization-configure-with-custom-target-attributes.md)



<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
