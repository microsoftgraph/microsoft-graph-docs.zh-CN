---
title: 跨租户访问设置 API 概述
description: 跨租户访问设置让你能够管理组织的 B2B 协作和 B2B 直接连接。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="cross-tenant-access-settings-api-overview"></a>跨租户访问设置 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在传统 Azure AD B2B 协作中，来自组织的任何受邀用户都可使用其身份访问外部组织的资源。 管理员无法控制允许其租户登录到外部组织的用户标识。 这些有限的控制使得难以阻止以未经授权的方式使用您组织的标识。

**跨租户访问设置** 使你可以控制和管理组织中用户与其他组织之间的协作。 该控件可以控制出站访问 (用户与其他组织的协作方式) 、入站访问 (组织如何与您进行协作) ，  或同时位于这两者。

粒度控件使你可以确定组织中和外部组织中可以参与 Azure AD B2B 协作和 Azure AD B2B 直接连接的用户、组和应用。 这些控件通过以下方式实现：

+ **设置基线入站和** 出站访问设置的默认跨租户访问设置。
    + 在Azure AD B2B 协作中，默认情况下启用这两个访问设置。 这意味着所有用户都可以受邀加入外部组织，并且你的所有用户都可以邀请外部用户。
    + 在Azure AD B2B 直接连接中，默认情况下禁用这两个访问设置。
    + 可能会更新服务默认设置。
+ **合作伙伴特定的访问设置** ，可让你为各个组织配置自定义设置。 对于已配置的组织，此配置优先于默认设置。 因此，Azure AD在Azure AD禁用 B2B 协作和 B2B 直接连接时，您可以为特定的外部组织启用这些功能。

> [!IMPORTANT]
> 
> 通过配置 B2B 直接连接出站设置，即表示你同意允许已启用出站设置的外部组织访问有关用户的有限联系人数据。 Microsoft 与这些组织共享此数据，以帮助他们发送与用户连接的请求。 外部组织收集的数据（包括有限的联系人数据）受这些组织的隐私策略和做法的约束。

## <a name="default-cross-tenant-access-settings"></a>默认跨租户访问设置

默认跨租户访问设置确定您与所有其他组织进行入站和出站Azure AD。 与未在跨租户访问设置中显式列出的组织的任何外部协作都将继承这些默认设置。 默认设置是使用 [crossTenantAccessPolicyConfigurationDefault 资源](../resources/crosstenantaccesspolicyconfigurationdefault.md) 类型定义的。

默认情况下，Azure AD为Azure AD租户分配跨租户访问设置的服务默认配置。 可以使用自己的配置覆盖这些服务默认值，以适合您的组织。 通过查看查询默认终结点时返回的 **isServiceDefault** 属性，可以确认使用的是服务默认设置还是修改了默认设置。

## <a name="partner-cross-tenant-access-settings"></a>合作伙伴跨租户访问设置

特定于合作伙伴的跨租户访问设置可确定您与特定组织进行入站和出站Azure AD关系。 与该组织的任何协作都将继承这些特定于合作伙伴的设置。 合作伙伴设置使用 [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 资源类型定义。

即使向跨租户访问设置添加了合作伙伴，某些默认设置仍将适用。 例如，如果在跨租户访问设置中仅为合作伙伴配置 **b2bCollaborationInbound** ，则此合作伙伴配置的所有其他设置都将继承自默认的跨租户访问设置。 查询合作伙伴终结点时 `null` ，合作伙伴对象上的任何属性都表示对于该属性，它从默认策略继承设置。

## <a name="inbound-trust-settings-in-cross-tenant-access-settings"></a>跨租户访问设置中的入站信任设置

入站信任设置使您能够信任 MFA 外部用户在主目录中执行。 这可以防止外部用户必须同时在主目录和目录中执行 MFA。 借助入站信任设置，您可以为外部用户启用无缝身份验证体验，并节省组织所产生的 MFA 成本。  

例如，将信任设置配置为信任 MFA 时，MFA 策略仍应用于外部用户，但已在主租户中完成 MFA 的用户无需在租户中再次完成 MFA。

入站信任设置还使您能够信任已加入其主目录中的兼容Azure AD混合设备。 借助跨租户访问设置中的入站信任设置，你现在可以通过要求外部用户使用兼容或混合访问已加入的设备来保护Azure AD访问。

## <a name="interpreting-the-api-response"></a>解释 API 响应

跨租户访问设置 API 可用于设置多个配置，以允许或阻止对组织的访问。 下表重点介绍了方案，显示了 API 响应的示例，以及该响应的解释内容。 **b2bSetting** 用作任何 B2B 入站 (**b2bCollaborationInbound** 或 **b2bDirectConnectInbound**) 或出站 (**b2bCollaborationOutbound** 或 **b2bDirectConnectOutbound**) 配置的占位符。

<table>
<tr>
<td> 应用场景 </td> <td> API 输出 </td> <td> 解释 </td>
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
<td> 允许组"g1"中的用户访问任何应用 </td>
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
<td> 组"g1"中的用户可以访问任何应用。 所有不在组"g1"中的其他用户将被阻止。 </td>
</tr>
<tr>
<td> 仅允许访问应用程序"a1" </td>
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
<td> 仅允许所有用户访问应用程序"a1" </td>
</tr>
<tr>
<td> 允许组"g1"中的用户并阻止访问应用程序"a1" </td>
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
<td> 允许组"g1"中的所有用户访问除应用程序"a1<b></b>"之外的任何应用程序。 </td>
</tr>
<tr>
<td> 阻止组"g1"中的用户访问任何应用程序 </td>
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
<td> 组"g1"中的用户无法访问任何应用程序。 不在组"g1"中的其他用户有权访问所有应用程序。 </td>
</tr>
<tr>
<td> 阻止组"g1"中的用户，并仅允许访问应用程序"a1" </td>
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
<td> 组"g1"中的用户无法访问任何应用程序。 任何不在组"g1"中的用户都只能访问应用程序"a1"。 </td>
</tr>
<tr>
<td> 允许组"g1"中的用户仅访问应用程序"a1" </td>
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
<td> 组"g1"中的用户只能访问应用程序"a1"。 将阻止所有用户（包括组"g1"中的用户）访问任何其他应用程序。 </td>
</tr>
<tr>
<td> 阻止组"g1"中的用户访问应用程序"a1" </td>
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
<td> 组"g1"中的用户仅被阻止访问应用程序"a1"。 所有用户（包括组"g1"中的用户）都能访问任何其他应用程序。 </td>
</tr>
</table>

## <a name="cross-tenant-access-settings-vs-tenant-restrictions"></a>跨租户访问设置与租户限制

跨租户访问设置出站控制用于控制组织帐户如何用于访问其他组织Azure AD资源。 租户限制用于控制员工在网络或Azure AD时如何使用组织的其他 **帐户**。 关键的一点，出站控件一段时间都运行，因为它们与帐户关联，而租户限制要求将其他信号注入身份验证请求以强制执行，因为租户限制的范围是网络和设备，而不是帐户。 详细了解租户 [限制](/azure/active-directory/manage-apps/tenant-restrictions)。

## <a name="next-steps"></a>后续步骤

+ [跨租户访问设置文档](/azure/active-directory/external-identities/cross-tenant-access-overview)
+ [crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md) 资源类型
+ [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 资源类型
