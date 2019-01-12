---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6d9841d4957d5330fc966f60a24582e101831b6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969028"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。

## <a name="derived-types"></a>派生的类型
| 类型 | 说明 | 
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | 使用此类型来匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | 使用此类型在 Azure AD 中创建新的用户帐户。 |
