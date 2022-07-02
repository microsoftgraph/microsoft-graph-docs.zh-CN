---
title: 跨租户访问设置 API 概述
description: 借助跨租户访问设置，可以管理组织的 B2B 协作和 B2B 直接连接。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 270f1b53428853c5ba539a94014bec532e10fced
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604576"
---
# <a name="cross-tenant-access-settings-api-overview"></a>跨租户访问设置 API 概述

命名空间：microsoft.graph

在传统的 Azure AD B2B 协作中，组织中的任何受邀用户都可以使用其标识访问外部组织中的资源。 管理员无法控制其租户中允许登录到外部组织的用户标识。 这些有限的控制使得很难阻止组织中的标识以未经授权的方式使用。

**使用跨租户访问设置** 可以控制和管理组织中用户与其他组织中的用户之间的协作。 该控件可用于 **出站访问** (用户如何与其他组织协作) 、 **入站访问** (其他组织如何与你) 协作，或者两者兼有。

通过精细控制，可以确定组织和外部组织中可以参与 Azure AD B2B 协作和 Azure AD B2B 直接连接的用户、组和应用。 这些控件通过以下方式实现：

+ 设置基线入站和出站 **访问设置的默认跨租户访问** 设置。
    + 在 Azure AD B2B 协作中，默认启用这两个访问设置。 这意味着可以邀请所有用户加入外部组织，并且所有用户都可以邀请外部用户。
    + 在 Azure AD B2B 直接连接中，默认禁用这两个访问设置。
    + 可以更新服务默认设置。
+ **合作伙伴特定的访问设置** ，可用于为单个组织配置自定义设置。 对于配置的组织，此配置优先于默认设置。 因此，虽然默认情况下可能会在整个组织中禁用 Azure AD B2B 协作和 Azure AD B2B 直接连接，但可以为特定外部组织启用这些功能。

> [!IMPORTANT]
> 
> 通过配置 B2B 直接连接出站设置，你同意允许已启用出站设置的外部组织访问有关用户的有限联系人数据。 Microsoft 与这些组织共享此数据，以帮助他们发送与用户连接的请求。 外部组织收集的数据（包括有限的联系人数据）受这些组织的隐私政策和做法的约束。

## <a name="default-cross-tenant-access-settings"></a>默认跨租户访问设置

默认的跨租户访问设置决定了你与所有其他 Azure AD 组织进行入站和出站协作的立场。 与未在跨租户访问设置中显式列出的组织进行的任何外部协作都将继承这些默认设置。 默认设置是使用 [crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md) 资源类型定义的。

默认情况下，Azure AD 为所有 Azure AD 租户分配跨租户访问设置的服务默认配置。 可以使用自己的配置替代这些服务默认值，以适合你的组织。 可以通过查看查询默认终结点时返回的 **isServiceDefault** 属性来确认是使用服务默认设置还是修改了默认设置。

## <a name="partner-cross-tenant-access-settings"></a>合作伙伴跨租户访问设置

特定于合作伙伴的跨租户访问设置决定了你与特定 Azure AD 组织进行入站和出站协作的立场。 与此组织的任何协作都将继承这些特定于合作伙伴的设置。 合作伙伴设置是使用 [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 资源类型定义的。

即使已将合作伙伴添加到跨租户访问设置，某些默认设置仍将适用。 例如，如果在跨租户访问设置中仅为合作伙伴配置 **b2bCollaborationInbound** ，则该合作伙伴配置的所有其他设置将从默认的跨租户访问设置继承。 查询合作伙伴终结点时，合作伙伴对象 `null` 上的任何属性都意味着，对于该属性，它将从默认策略继承设置。

## <a name="inbound-trust-settings-in-cross-tenant-access-settings"></a>跨租户访问设置中的入站信任设置

通过入站信任设置，可以信任 MFA 外部用户在其主目录中执行的操作。 这可防止外部用户在其主目录和目录中执行 MFA。 借助入站信任设置，可为外部用户启用无缝身份验证体验，并节省组织产生的 MFA 成本。  

例如，将信任设置配置为信任 MFA 时，你的 MFA 策略仍会应用于外部用户，但已在其主租户中完成 MFA 的用户无需在租户中再次完成 MFA。

通过入站信任设置，还可以信任符合标准或混合 Azure AD 加入其主目录的设备。 借助跨租户访问设置中的入站信任设置，现在可以通过要求外部用户使用合规或已加入混合 Azure AD 的设备来保护对应用和资源的访问。

## <a name="interpreting-the-api-response"></a>解释 API 响应

跨租户访问设置 API 可用于设置多个配置，以允许或阻止对组织的访问。 下表突出显示了方案，显示了 API 响应的示例，以及该响应的解释应是什么。 **b2bSetting 用作 b2b** 入站 (**b2bCollaborationInbound** 或 **b2bDirectConnectInbound**) 或出站 (**b2bCollaborationOutbound** 或 **b2bDirectConnectOutbound**) 配置的占位符。

<br/>

<table>
<tr>
<th> 应用场景 </th> <th> API 输出 </th> <th> 解释 </th>
</tr>
<tr>
<td> 阻止所有用户并阻止所有应用程序 </td>
<td>

``` json
"b2bsetting": {
    "usersAndGroups": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "AllUsers",
                "targetType": "user"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> - </td>
</tr>
<tr>
<td> 允许所有用户并允许所有应用程序 </td>
<td>

``` json
"b2bsetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllUsers",
                "targetType": "user"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> - </td>
</tr>
<tr>
<td> 允许组“g1”中的用户访问任何应用 </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 组“g1”中的用户可以访问任何应用。 组“g1”中未包含的所有其他用户将被阻止。 </td>
</tr>
<tr>
<td> 仅允许访问应用程序“a1” </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "AllUsers",
                "targetType": "user"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 仅允许所有用户访问应用程序“a1” </td>
</tr>
<tr>
<td> 允许组“g1”中的用户阻止对应用程序“a1”的访问 </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 组“g1”中的所有用户都可以访问除应用程序“a1” <b>以外的</b> 任何应用程序。 </td>
</tr>
<tr>
<td> 阻止组“g1”中的用户访问任何应用程序 </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": " blocked",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "AllApplications",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 组“g1”中的用户无法访问任何应用程序。 不在组“g1”中的其他用户有权访问所有应用程序。 </td>
</tr>
<tr>
<td> 阻止组“g1”中的用户，并仅允许访问应用程序“a1” </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 组“g1”中的用户无法访问任何应用程序。 组“g1”中的任何用户只能访问应用程序“a1”。 </td>
</tr>
<tr>
<td> 允许组“g1”中的用户仅访问应用程序“a1” </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "allowed",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 组“g1”中的用户只能访问应用程序“a1”。 阻止所有用户（包括组“g1”中的用户）访问任何其他应用程序。 </td>
</tr>
<tr>
<td> 阻止组“g1”中的用户访问应用程序“a1” </td>
<td>

``` json
"b2bSetting": {
    "usersAndGroups": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "g1",
                "targetType": "group"
            }
        ]
    },
    "applications": {
        "accessType": "blocked",
        "targets": [
            {
                "target": "a1",
                "targetType": "application"
            }
        ]
    }
}
```

</td>
<td> 组“g1”中的用户只能访问应用程序“a1”。 所有用户（包括组“g1”中的用户）都能够访问任何其他应用程序。 </td>
</tr>
</table>

## <a name="cross-tenant-access-settings-vs-tenant-restrictions"></a>跨租户访问设置与租户限制

跨租户访问设置出站控件用于控制 **组织帐户** 用于访问其他 Azure AD 组织中的资源的方式。 租户限制用于控制 **员工在网络或设备上使用其他 Azure AD 组织帐户** 的方式。 关键是，出站控件一直有效，因为它们与你的帐户相关联，而租户限制要求将其他信号注入身份验证请求以强制执行，因为租户限制的范围限于网络和设备，而不是帐户。 详细了解 [租户限制](/azure/active-directory/manage-apps/tenant-restrictions)。

## <a name="next-steps"></a>后续步骤

+ [跨租户访问设置文档](/azure/active-directory/external-identities/cross-tenant-access-overview)
+ [crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md) 资源类型
+ [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 资源类型
