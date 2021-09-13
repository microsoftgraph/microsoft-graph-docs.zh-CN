---
title: 应用程序 API 概述
description: 向 Azure AD 注册应用程序，以为其创建标识配置，允许其与 Azure AD 集成。
author: davidmu1
ms.localizationpriority: high
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: 6aef637d7e24e1d023012d81a365766cd7b6625e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028749"
---
# <a name="applications-api-overview"></a>应用程序 API 概述

为将标识和访问管理功能委派给 Azure AD，必须向 Azure AD 租户注册应用程序。 向 Azure AD 注册应用程序时，将为应用程序创建标识配置，允许其与 Azure AD 集成。

## <a name="why-use-applications-and-associated-resources"></a>为什么要使用应用程序和相关的资源？

Microsoft Graph API 使你能够管理与 Azure Active Directory 中的应用程序相关的这些资源和操作：
- **应用程序管理** - Azure AD 必须配置为与应用程序集成。 换言之，需要了解哪些应用程序将其用作标识系统。 让 Azure AD 了解这些应用程序，以及应该如何处理这些应用程序的过程称为应用程序管理。
- **本地发布** - 可将租户管理员安装的本地代理（或应用程序代理的连接器）配置为请求转接到特定的已发布资源。
- **服务主体管理** - 单个租户或目录中的全局应用程序对象的本地表示或应用程序实例。 服务主体是通过应用程序对象创建的具体实例，并从该应用程序对象继承某些属性。
- **同步** - Azure Active Directory (Azure AD) 标识同步（也称为 *预配*）使你能够自动化云中的标识的创建、维护和删除。

## <a name="application-management"></a>应用管理

应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。 可使用 Microsoft Graph 中的[应用程序 API](/graph/api/resources/application?view=graph-rest-1.0) 以编程方式管理应用程序。

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

有关应用程序的更多信息，请参阅以下文章：
- [应用程序模型](/azure/active-directory/develop/application-model)
- [Azure Active Directory 中的应用程序和服务主体对象](/azure/active-directory/develop/app-objects-and-service-principals)
- [Microsoft 标识平台的应用程序类型](/azure/active-directory/develop/v2-app-types)

有关应用程序管理的更多信息，请参阅以下文章：
- [什么是应用程序管理？](/azure/active-directory/manage-apps/what-is-application-management)
- [身份验证流程和应用程序方案](/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a>本地发布（预览版）

创建和管理本地发布配置文件，其中包括创建本地代理和代理组。 可使用 Microsoft Graph 中的[本地发布 API](/graph/api/resources/onpremisespublishingprofile-root) 以编程方式管理本地发布配置文件。

有关本地发布的详细信息，请参阅以下文章：
- [通过 Azure Active Directory 的应用程序代理对本地应用程序进行远程访问](/azure/active-directory/manage-apps/application-proxy)
- [使用 Azure AD 应用程序代理为远程用户发布本地应用](/azure/active-directory/manage-apps/what-is-application-proxy)

若要了解如何使用本地发布 API，请参阅以下教程及其相关的 API：
- [使用 Microsoft Graph API 自动化应用程序代理的配置](./application-proxy-configure-api.md)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [onPremisesPublishing](/graph/api/resources/onpremisespublishingprofile-root)
    - [connector](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a>服务主体管理

若要访问受 Azure AD 租户保护的资源，需要访问的实体必须由安全主体表示。 可使用 Microsoft Graph 中的[服务主体 API](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 以编程方式管理服务主体。

有关服务主体的详细信息，请参阅 [Azure Active Directory 中的应用程序和服务主体对象](/azure/active-directory/develop/app-objects-and-service-principals)。

## <a name="synchronization"></a>同步

可使用 Microsoft Graph 中的[同步 API](/graph/api/resources/synchronization-overview) 以编程方式管理标识同步，包括：
- 创建、启动和停止同步作业
- 对作业的同步架构进行更改
- 验证当前同步状态

有关同步的详细信息，请参阅以下文章：
- [使用 Azure AD 为应用程序自动预配和取消用户](/azure/active-directory/app-provisioning/user-provisioning)
- [预配的工作原理](/azure/active-directory/app-provisioning/how-provisioning-works)

若要了解有关使用同步 API 的信息，请参阅以下教程及其相关联的 API：
- [使用 Microsoft Graph Api 配置预配](/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [synchronizationTemplate](/graph/api/resources/synchronization-synchronizationtemplate)
    - [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob)
- [使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置](/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a>后续步骤
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 Microsoft Graph API。
- 了解如何使用[这些示例](/azure/active-directory/develop/sample-v2-code)将身份验证和授权添加到 web 应用程序和 web API。
