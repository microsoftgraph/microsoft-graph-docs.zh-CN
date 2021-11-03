---
title: '预览版中的联合标识Azure Active Directory (概述) '
description: 联合身份凭据允许你访问 Azure 和 Microsoft Graph，而无需管理密钥。 这是 Azure AD 中工作负荷联合的一Azure AD。
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: conceptualPageType
ms.openlocfilehash: 58ad41d9d0277eabf39c2e830fb15f302f3813be
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697238"
---
# <a name="overview-of-federated-identity-credentials-in-azure-active-directory-preview"></a>预览版中的联合标识Azure Active Directory (概述) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通常，开发人员使用证书或客户端密码来验证应用程序凭据并访问 Azure AD 中的服务。 若要访问其 Azure AD 中的服务，开发人员必须存储和管理 Azure 外部的应用程序凭据，这引入了以下瓶颈：

+ 证书和密码的维护负担。
+ 泄露密码的风险。
+ 由于身份验证失败，证书过期和服务中断。

**联合身份凭据** 是一种新的凭据类型，可启用软件工作负荷的工作负荷联合身份验证。 利用工作负载联合身份验证，Azure Active Directory (Azure AD) 受保护的资源，而无需管理受支持 (应用程序密钥) 。 通过配置联合标识凭据，您可以在外部标识提供程序Azure AD应用程序之间创建信任关系。 联合标识凭据用于指示应用程序应信任来自外部 IdP 的令牌。 创建信任关系后，软件工作负载可以从外部标识提供程序交换受信任的令牌，以从外部标识Microsoft 标识平台。  然后，软件工作负载使用该访问令牌访问Azure AD已授予工作负荷访问权限的受保护资源。 这消除了手动管理凭据的维护负担，并消除了泄露密码或使证书过期的风险。 有关详细信息和支持的方案，请阅读有关 [工作负荷联合身份验证的信息](/azure/active-directory/develop/workload-identity-federation)。

[federatedIdentityCredential](federatedidentitycredential.md)资源表示通过 Microsoft Graph API 配置联合标识凭据。 以下属性是联合身份凭据的构建基块：

+ **audiences**— 列出可在外部令牌中显示访问群体。 此字段是必需的，默认为"api://AzureADTokenExchange"。 它指出Microsoft 标识平台令牌中的 aud 声明应接受哪些信息。 此值表示Azure AD标识提供程序中的令牌，并且未跨标识固定值 - 可能需要在 IdP 中创建新的应用程序注册，以用作此令牌的受众。
+ **issuer**— 外部标识提供程序的 URL，且必须与要 `issuer` 交换的外部令牌声明匹配。
+ **subject**- 外部标识提供程序中的外部软件工作负荷的标识符。 与访问群体值一样，它没有固定格式，因为每个 IdP 都使用其自己的格式，有时使用 GUID，有时是冒号分隔的标识符，有时是任意字符串。 此处的值必须与向用户呈现的令牌中的子声明Azure AD。

颁发者和 **主题**    **的组合在**   应用中必须是唯一的。  当外部软件工作负荷请求Microsoft 标识平台令牌交换访问令牌时，将针对 外部令牌中提供的 和声明检查联合身份凭据的颁发者和 `issuer` `subject` 主题值。 如果该验证检查通过，Microsoft 标识平台外部软件工作负载颁发访问令牌。

只有应用程序才支持联合身份凭据。 每个应用程序对象最多可以添加 20 个联合标识凭据。

联合身份凭据 API 不适用于国家 [云](/graph/deployments) 部署。

## <a name="see-also"></a>另请参阅

+ [federatedIdentityCredential 资源类型](federatedidentitycredential.md)
+ [工作负荷联合身份验证](/azure/active-directory/develop/workload-identity-federation)
+ [什么是 Azure 资源的托管标识？](/azure/active-directory/managed-identities-azure-resources/overview)
<!--
Future: add links to articles that use federated identity credentials to access Azure AD resources.
>
