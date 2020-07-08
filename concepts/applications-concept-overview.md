---
title: 应用程序 API 概述
description: 向 Azure AD 注册应用程序，以便为其创建可与 Azure AD 集成的标识配置。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: ff38e14182d2e38fbc2203241da911dec07f9846
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081192"
---
# <a name="applications-api-overview"></a>应用程序 API 概述

为了将 identity and access management 函数委派给 Azure AD，必须向 Azure AD 租户注册应用程序。 当您向 Azure AD 注册应用程序时，您正在为应用程序创建标识配置，使其能够与 Azure AD 集成。

## <a name="why-use-applications-and-associated-resources"></a>为什么要使用应用程序和相关联的资源？

使用 Microsoft Graph Api，您可以管理与 Azure Active Directory 中的应用程序相关的这些资源和操作：
- **应用程序管理**-Azure AD 必须配置为与应用程序集成。 换句话说，它需要知道哪些应用程序正在将其用作标识系统。 阻止 Azure AD 识别这些应用程序以及它如何处理它们的过程称为 "应用程序管理"。
- 可将租户管理员安装的本地**发布**代理（或应用程序代理的连接器）配置为将请求路由到特定的已发布资源。
- **服务主体管理**-单个租户或目录中全局应用程序对象的本地表示形式或应用程序实例。 服务主体是从 application 对象创建的具体实例，并继承该 application 对象的某些属性。
- **同步**-Azure Active Directory （azure AD）标识同步（也称为*设置*）允许您自动创建、维护和删除云中的标识。

## <a name="application-management"></a>应用管理

应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。 您可以使用 Microsoft Graph 中的[应用程序 api](/graph/api/resources/application?view=graph-rest-1.0)以编程方式管理应用程序。

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

有关应用程序的详细信息，请参阅以下文章：
- [应用程序模型](https://docs.microsoft.com/azure/active-directory/develop/application-model)
- [Azure Active Directory 中的应用程序和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
- [Microsoft identity platform 的应用程序类型](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types)

有关应用程序管理的详细信息，请参阅以下文章：
- [什么是应用程序管理？](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-management)
- [身份验证流和应用程序方案](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a>本地发布（预览）

创建和管理本地发布配置文件，其中包括创建本地代理和代理组。 您可以使用 Microsoft Graph 中的[本地发布 api](/graph/api/resources/onpremisespublishingprofile-root)以编程方式管理本地发布配置文件。

有关本地发布的详细信息，请参阅以下文章：
- [通过 Azure Active Directory 的应用程序代理远程访问本地应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy)
- [使用 Azure AD 应用程序代理为远程用户发布内部部署应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-proxy)

若要了解如何使用内部部署发布 Api，请参阅以下教程及其关联的 Api：
- [使用 Microsoft Graph API 自动配置应用程序代理](https://docs.microsoft.com/graph/application-proxy-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [onPremisesPublishing](/graph/api/resources/onpremisespublishingprofile-root)
    - [连接器](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a>服务主体管理

若要访问受 Azure AD 租户保护的资源，需要访问的实体必须由安全主体表示。 您可以使用 Microsoft Graph 中的[服务主体 api](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)以编程方式管理服务主体。

有关服务主体的详细信息，请参阅[Azure Active Directory 中的应用程序和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。

## <a name="synchronization"></a>同步

您可以使用 Microsoft Graph 中的[同步 api](/graph/api/resources/synchronization-overview)以编程方式管理标识同步，包括：
- 创建、启动和停止同步作业
- 对作业的同步架构进行更改
- 验证当前同步状态

有关同步的详细信息，请参阅以下文章：
- [使用 Azure AD 自动化用户预配和预配到应用程序](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)
- [预配的工作原理](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)

若要了解如何使用同步 Api，请参阅以下教程及其关联的 Api：
- [使用 Microsoft Graph Api 配置设置](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [synchronizationTemplate](/graph/api/resources/synchronization-synchronizationtemplate)
    - [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob)
- [使用 Microsoft Graph API 自动执行基于 SAML 的 SSO 应用配置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a>后续步骤
- 在[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中试用 MICROSOFT Graph API。
- 了解如何使用[这些示例](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code)向 web 应用程序和 web api 添加身份验证和授权。
