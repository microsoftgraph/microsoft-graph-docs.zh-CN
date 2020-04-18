---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 73f4bb06d15c6b2e41226e872b71ba417de1076b
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557904"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)是用户在 Azure Active DIRECTORY （AD）中进行身份验证的方法。 Azure AD 中的身份验证方法包括密码和电话（例如，SMS 和语音呼叫），这些方法可在 Microsoft Graph 中进行管理，如 FIDO2 安全密钥和 Microsoft 身份验证器应用等许多其他内容。 身份验证方法在主要、第二因素和分步身份验证以及自助密码重置（SSPR）过程中也使用。

身份验证方法 Api 用于管理用户的身份验证方法。 例如：

* 您可以向用户添加电话号码。 如果启用此电话号码，则用户可以通过策略将其用于 SMS 和语音呼叫身份验证。 
* 您可以更新该号码，也可以将其从用户中删除。
* 您可以启用或禁用用于 SMS 登录的号码。
* 您可以重置用户的密码。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>可以在 Microsoft Graph 中管理哪些身份验证方法？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[passwordAuthenticationMethod](passwordauthenticationmethod.md)| 密码当前是 Azure AD 中默认的主要身份验证方法。|重置用户密码|
|[phoneAuthenticationMethod](phoneauthenticationmethod.md)|用户可使用电话使用[短信或语音呼叫](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options)进行身份验证（如策略允许）。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用 SMS 登录的主移动电话。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。
