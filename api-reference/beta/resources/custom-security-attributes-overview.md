---
title: '使用 Microsoft 图形 API (Preview 属性的自定义) '
description: 了解如何使用 Microsoft Azure AD以编程方式定义自己的自定义安全图形 API。
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: conceptualPageType
ms.openlocfilehash: 609e92333195f883ed8387320f925255654fa5ad
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607755"
---
# <a name="overview-of-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>使用 Microsoft 图形 API (Preview 属性的自定义) 

> [!IMPORTANT]
> 自定义安全属性功能当前处于预览阶段。 有关适用于 Beta 版、预览[版](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)或尚未正式发布的 Azure 功能的法律条款，请参阅 Microsoft Azure 预览版补充使用条款。

[Azure Active Directory (Azure AD) 中的](/azure/active-directory/fundamentals/custom-security-attributes-overview)自定义安全属性是特定于业务 (属性，) 定义和分配给 Azure AD 对象。 这些属性可用于存储信息、对对象进行分类或强制实施对特定 Azure 资源的精细访问控制。 自定义安全属性可以与 [Azure ABAC (基于 Azure 属性的访问控制) ](/azure/role-based-access-control/conditions-overview)。

本文概述了如何使用 Microsoft 图形 API以编程方式定义和分配自己的自定义安全属性。

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

可以使用 属性将自定义安全属性分配给以下 `customSecurityAttributes` 对象。 还可以为目录中的已同步本地 Active Directory分配自定义安全属性。

+ [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
+ [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)

## <a name="limits-and-constraints"></a>限制和约束

有关自定义安全属性的限制和约束的列表，请参阅 [限制和约束](/azure/active-directory/fundamentals/custom-security-attributes-overview#limits-and-constraints)。

## <a name="permissions"></a>Permissions

若要管理自定义安全属性，必须为调用主体分配以下角色Azure AD之一。 默认情况下，全局管理员和其他管理员角色没有读取、定义或分配自定义安全属性的权限。

+ [属性定义读取器](/azure/active-directory/roles/permissions-reference#attribute-definition-reader)
+ [属性定义管理员](/azure/active-directory/roles/permissions-reference#attribute-definition-administrator)
+ [属性分配读取器](/azure/active-directory/roles/permissions-reference#attribute-assignment-reader)
+ [属性分配管理员](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

此外，还必须向调用主体授予相应的 [自定义安全属性权限](/graph/permissions-reference#custom-security-attributes-permissions)。

## <a name="license-requirements"></a>许可要求

使用自定义安全属性需要Azure AD Premium P1或 P2 许可证。

## <a name="next-steps"></a>后续步骤

+ [customSecurityAttributeDefinition 资源类型](/graph/api/resources/customsecurityattributedefinition)
+ [使用 Microsoft 策略分配、更新或删除自定义安全图形 API](/graph/custom-security-attributes-examples)
+ [什么是自定义安全Azure AD？](/azure/active-directory/fundamentals/custom-security-attributes-overview)

