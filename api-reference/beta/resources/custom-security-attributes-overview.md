---
title: '使用 Microsoft Graph API 预览版 (自定义) '
description: 了解如何使用 Microsoft Graph API 以编程方式定义自己的自定义安全属性并将其分配给Azure AD对象。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: conceptualPageType
ms.openlocfilehash: 45e3ab02292deea2af8c6e632b2cb698ac13867d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077682"
---
# <a name="overview-of-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>使用 Microsoft Graph API 预览版 (自定义) 

> [!IMPORTANT]
> 自定义安全属性功能当前处于预览阶段。 有关适用于 Beta 版、预览[版或](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)尚未正式发布的 Azure 功能的法律条款，请参阅 Microsoft Azure 预览版补充使用条款。

[Azure Active Directory (Azure AD) 中的](/azure/active-directory/fundamentals/custom-security-attributes-overview)自定义安全属性是特定于业务 (属性，) 定义和分配给 Azure AD 对象。 这些属性可用于存储信息、对对象进行分类或强制实施对特定 Azure 资源的精细访问控制。 自定义安全属性可以与 Azure ABAC (基于 Azure 属性的[访问控制) 。 ](/azure/role-based-access-control/conditions-overview)

本文概述了如何使用 Microsoft Graph API 以编程方式定义和分配自己的自定义安全属性。

## <a name="key-resource-types"></a>重要资源类型

以下是自定义安全属性的构建基块。

### <a name="attribute-sets"></a>属性集

属性 *集* 是一组相关的自定义安全属性。 以下是属性集的一般特征：

+ 名称不能包含空格或特殊字符。
+ 无法重命名或删除。
+ 可以委派给其他用户来定义和分配自定义安全属性。

若要配置属性集，请使用 [attributeSet 资源类型](attributeset.md)。
 
### <a name="custom-security-attribute-definitions"></a>自定义安全属性定义

自定义 *安全属性定义* 是自定义安全属性或键值对的架构。 例如，自定义安全属性名称、说明、数据类型和预定义值。 以下是自定义安全属性定义的一般特征：

+ 名称不能包含空格或特殊字符。
+ 无法重命名或删除，但可以停用。
+ 必须是属性集的一部分。

若要配置自定义安全属性定义，请使用 [customSecurityAttributeDefinition 资源类型](customsecurityattributedefinition.md)。

### <a name="allowed-values"></a>允许的值

*允许的值* 表示自定义安全属性的预定义值。 以下是允许值的一般特征：

+ 值可以包括空格，但不允许使用某些特殊字符。
+ 无法重命名或删除，但可以停用。
+ 稍后可以添加更多预定义值。
+ 可以是 Boolean、Integer 或 String 数据类型。

若要配置允许的值，请使用 [allowedValue 资源类型](allowedvalue.md)。

## <a name="which-directory-objects-support-custom-security-attributes"></a>哪些目录对象支持自定义安全属性？

可以使用 属性将自定义安全属性分配给以下 `customSecurityAttributes` 对象。 还可以为来自本地 Active Directory 的目录同步用户分配自定义安全属性。

+ [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
+ [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)

## <a name="limits-and-constraints"></a>限制和约束

下面是自定义安全属性的一些限制和约束。

| 资源 | 限制 | Notes |
| --- | :---: | --- |
| 每个租户的属性定义 | 500 | 仅适用于租户中的活动属性 |
| 每个租户的属性集 | 500 |  |
| 属性集名称长度 | 32 | Unicode 字符和大小写不区分大小写 |
| 属性集说明长度 | 128 | Unicode 字符 |
| 属性名称长度 | 32 | Unicode 字符和大小写不区分大小写 |
| 属性描述长度 | 128 | Unicode 字符 |
| 预定义值 |  | Unicode 字符和区分大小写 |
| 每个属性定义的预定义值 | 100 |  |
| 属性值长度 | 64 | Unicode 字符 |
| 按对象分配的属性值 | 50 | 值可以跨单值和多值属性分布。<br/>示例：5 个属性，每个属性具有 10 个值，或 50 个属性，每个属性有 1 个值 |
| 不允许用于：<br/>属性集名称<br/>属性名 | ``<space> ` ~ ! @ # $ % ^ & * ( ) _ - + = { [ } ] \| \ : ; " ' < , > . ? /`` |  |
| 不允许用于：<br/>属性值 | `# % & * + \ : " / < > ?` |  |

## <a name="permissions"></a>权限

若要管理自定义安全属性，必须为调用主体分配以下角色Azure AD之一。 默认情况下，全局管理员和其他管理员角色没有读取、定义或分配自定义安全属性的权限。

+ [属性定义读取器](/azure/active-directory/roles/permissions-reference#attribute-definition-reader)
+ [属性定义管理员](/azure/active-directory/roles/permissions-reference#attribute-definition-administrator)
+ [属性分配读取器](/azure/active-directory/roles/permissions-reference#attribute-assignment-reader)
+ [属性分配管理员](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

此外，还必须向调用主体授予相应的 [自定义安全属性权限](/graph/permissions-reference#custom-security-attributes-permissions)。

## <a name="license-requirements"></a>许可要求

使用自定义安全属性需要Azure AD Premium P1 P2 许可证。

## <a name="next-steps"></a>后续步骤

+ [customSecurityAttributeDefinition 资源类型](/graph/api/resources/customsecurityattributedefinition)
+ [使用 Microsoft Graph API 分配、更新或删除自定义安全属性](/graph/custom-security-attributes-examples)
+ [什么是自定义安全Azure AD？](/azure/active-directory/fundamentals/custom-security-attributes-overview)

