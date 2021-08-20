---
title: 使用 Microsoft Graph 创建团队和管理成员
description: '创建包含团队的组涉及以下步骤： '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: e8175cf44c97609a24227881f22866c0bb1aeea2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260784"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a>使用 Microsoft Graph 创建团队和管理成员

可使用 Microsoft Graph 中的 Microsoft Teams API 以多种方式创建团队。 本文介绍了为获得最佳效果而推荐的方法。


## <a name="initial-team-creation"></a>初始团队创建

所有团队都有 Microsoft 365 组的支持。在通过 Microsoft Graph 创建新团队时，建立并运营团队的最快方法是设置新的 Microsoft 365 组、所有者和成员，然后将其转换为团队。

1. 使用“[创建组](/graph/api/group-post-groups?view=graph-rest-1.0)”操作来创建 [Microsoft 365 组](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)。 你可以指定所有者和成员。 确保新创建的组拥有正确的所有者，如步骤 2 所述。

    为了为此组创建团队，需要设置以下属性值，如下所示：

    - **groupTypes** = { "Unified" } 
    - **mailEnabled** = true
    - **securityEnabled** = false

    ```http
    POST /groups
    {
        "displayName":"Flight 157",
        "mailNickname":"flight157",
        "description":"Everything about flight 157",
        "visibility":"Private",
        "groupTypes":["Unified"],
        "mailEnabled":true,
        "securityEnabled":false,
        "members@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
            "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
        ],
        "owners@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
        ]
    }
    ```

    以下示例显示了相应的响应。 

    >**请注意:** 为了提高可读性，可能缩短了显示的响应对象。所有属性都将通过实际调用返回。

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. 确保组有两个或多个所有者。 可通过“[添加所有者](/graph/api/group-post-owners?view=graph-rest-1.0)”操作来实现这一点。 这些应为真实的用户帐户，而不是服务帐户。 拥有两个所有者有助于处理以下情况：一个所有者离开公司或无法执行团队管理操作。

3. 使用“[添加成员](/graph/api/group-post-members?view=graph-rest-1.0)”操作将所有成员（以及来宾，如有必要）添加到组中（如果在步骤 1 中未执行此操作）。 若要添加多个成员，请在每个添加操作后添加 1 秒延迟。 

4. 成功创建组（完成步骤 1 后最长需要 15 分钟）后，使用“[从组创建团队](/graph/api/team-post?view=graph-rest-1.0#example-4-create-a-team-from-group)”操作来创建 Microsoft Teams 团队。 如果遇到错误，则可能无法完成组创建过程；请尝试稍等几分钟。 

    ```http
    POST https://graph.microsoft.com/v1.0/teams
    Content-Type: application/json
    {
      "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
      "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
    }
    ```

    以下示例显示了相应的响应。 

    >**请注意:** 为了提高可读性，可能缩短了显示的响应对象。所有属性都将通过实际调用返回。

    ```http
    HTTP/1.1 202 Accepted
    Content-Type: application/json
    Location: /teams/{teamId}/operations/{operationId}
    Content-Location: /teams/{teamId}
    {
    }
    ```

    已创建团队的 ID 与组相同。

5. 完成此过程后，所有的所有者和成员都应能够在其 Teams 客户端中查看新创建的团队。

## <a name="adding-or-managing-members"></a>添加或管理成员

若要在创建团队后添加成员，请使用“[添加成员](/graph/api/group-post-members?view=graph-rest-1.0)”操作。 建议在添加操作之间添加 1 秒延迟。 请注意以下与成员身份更改有关的事项：

1. 对 Microsoft 365 组进行的成员身份更改通过后台同步机制同步到 Teams，此过程通常需要 24 小时（在某些情况下需要更长时间）。

2. 仅当团队中的一个或多个用户（所有者或成员）在 Teams 桌面客户端中处于活动状态时，才会触发后台进程。 启动 Teams 应用程序和/或使其运行即构成活动 — 用户无需访问专门修改的团队。

    >**注意：** Teams 移动客户端不会触发成员身份同步。应至少有一个用户位于桌面客户端上，以确保此后台进程顺利运行。

## <a name="checklist-for-validation"></a>验证清单

创建团队后，可使用以下清单验证是否已成功创建该团队。

### <a name="validate-team-creation"></a>验证团队创建

1. 验证为团队提供支持的 Microsoft 365 组是通过 Azure AD 还是 Microsoft 365 管理中心创建的。

2. 通过 Teams 管理门户验证团队创建是否成功。

3. 验证团队是否拥有通过 Teams 管理门户列出的正确所有者和成员。

4. 验证团队所有者登录 Teams 桌面或 Web 客户端后是否可以看到该团队。

5. 验证成员登录 Teams 桌面或 Web 客户端后是否可以看到该团队。

### <a name="validate-addition-of-members"></a>验证成员的添加

1. 验证新成员是否通过 Azure AD 或 Microsoft 365 管理中心显示在组中。

2. 验证新添加的成员登录 Teams 桌面或 Web 客户端后是否可以看到该团队。
