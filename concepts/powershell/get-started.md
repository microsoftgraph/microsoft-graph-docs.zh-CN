---
title: Microsoft Graph PowerShell SDK 入门
description: 开始使用 Microsoft Graph PowerShell SDK 执行一些基本任务。
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: d92a6057b9c7df7df4f9a7014df20e7a21bfe923
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883393"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Microsoft Graph PowerShell SDK 入门

在本指南中，你将使用 Microsoft Graph PowerShell SDK 来执行一些基本任务。 如果尚未 [安装 SDK](installation.md)，请在遵循本指南之前执行此操作。

## <a name="api-version"></a>API 版本

默认情况下，SDK 使用 [Microsoft Graph REST API v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)。 可以使用命令更改此项 `Select-MgProfile` 。

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>身份验证

PowerShell SDK 支持两种类型的身份验证：委派访问和仅限应用的访问。 在本指南中，你将使用委派的访问权限以用户身份登录，向 SDK 授予代表你行事的许可，并调用 Microsoft Graph。

有关对无人参与的方案使用仅限应用的访问权限的详细信息，请参阅 [Microsoft Graph PowerShell SDK 使用仅限应用的身份验证](app-only.md)。

### <a name="determine-required-permission-scopes"></a>确定所需的权限范围

Microsoft Graph中的每个 API 都受一个或多个权限范围的保护。 用户登录必须同意你计划使用的 API 所需的范围之一。 在此示例中，我们将使用以下 API。

- [列出用户](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) 以查找登录用户的用户 ID
- [列出 joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) 以获取用户所属Teams。
- [列出](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) 频道以获取团队中的频道。
- [发送消息](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) 以将消息发送到团队频道。

权 `User.Read.All` 限范围将启用前两个调用，而该 `Group.ReadWrite.All` 范围将启用其余的调用。 这些权限需要管理员帐户。

### <a name="sign-in"></a>登录

使用该 `Connect-MgGraph` 命令使用所需的范围登录。 需要使用管理员帐户登录才能同意所需的范围。

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

该命令将提示你转到网页以使用设备代码登录。 完成此操作后，该命令将指示消息成功 `Welcome To Microsoft Graph!` 。 每个会话只需执行一次此操作。

> [!TIP]
> 可以通过使用新的权限范围重复 `Connect-MgGraph` 命令来添加其他权限。

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph

登录后，可以开始调用 Microsoft Graph。

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

### <a name="get-the-signed-in-user"></a>获取已登录用户

在本部分中，你将找到登录用户并获取她的用户 ID。 需要将该参数用作稍后将要使用的其他命令的参数。 首先运行以下命令。

```powershell
Get-MgUser
```

这会输出Microsoft 365组织中的用户列表。

```powershell
Id                                   DisplayName              Mail                                  UserPrincipalName
--                                   -----------              ----                                  -----------------
88d1ba68-8ff5-4de2-90ed-768c00abcfae Conf Room Adams          Adams@contoso.onmicrosoft.com         Adams@contoso.…
3103c7b9-cfe6-4cd3-a696-f88909b9a609 Adele Vance              AdeleV@contoso.OnMicrosoft.com        AdeleV@contoso…
da3a885e-2d97-41de-9347-5271ef321b58 MOD Administrator        admin@contoso.OnMicrosoft.com         admin@contoso.…
e0c6ee40-e105-476d-9597-acd061d21fcb Alex Wilber              AlexW@contoso.OnMicrosoft.com         AlexW@contoso.…
17c6bdee-8ed3-49af-a65e-71b64cca8382 Allan Deyoung            AllanD@contoso.OnMicrosoft.com        AllanD@contoso…
e5b78950-27cd-4f01-b083-eab4da97ca6a Conf Room Baker          Baker@contoso.onmicrosoft.com         Baker@contoso.…
40467725-1a58-495d-9e2f-5970c6306d8d Bianca Pisani                                                  BiancaP@contoso…
ce73bdb5-bf12-405e-ab85-40122fdd6eb7 Brian Johnson (TAILSPIN) BrianJ@contoso.onmicrosoft.com        BrianJ@contoso…
df1347a3-7ce7-4b4d-8aab-7c65b5c907b9 Cameron White                                                  CameronW@contoso…
```

可以使用 [OData 筛选器](../query-parameters.md#filter-parameter) 来帮助查找所需的特定用户。 运行以下命令，替换 `Megan Bowen` 为已登录用户的显示名称。

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

输入以下内容来验证是否有效。

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>列出用户加入的团队

现在，使用用户的 ID 作为命令的 `Get-MgUserJoinedTeam` 参数。

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

就像命令一样 `Get-MgUser` ，这提供了团队列表。 选择用户加入的团队之一并复制其 `Id`。

### <a name="list-team-channels"></a>列出团队频道

现在，使用团队的 ID 作为命令的参数 `Get-MgTeamChannel` ，遵循类似的模式列出所有通道，然后筛选列表以获取所需的特定通道。

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId ID_FROM_PREVIOUS_STEP -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>发送消息

现在，你已拥有团队 ID 和频道 ID，可以将消息发布到频道。 使用以下命令发送消息。

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

此命令与之前使用的命令不同。 它实际上不是只查询数据，而是在创建某些内容。 在 Microsoft Graph中，这会转换为 HTTP`POST`，并且需要该帖子正文中的对象。 在这种情况下，该对象是 [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true)。 请注意， `-Body` 该命令的参数映射到 `body` 属性上 `chatMessage`。 其他属性的映射方式类似，因此可以更改发送的消息。 例如，若要发送紧急消息，请使用以下命令。

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a>注销

使用命令 `Disconnect-MgGraph` 注销。

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a>后续步骤

- [了解如何导航 SDK](navigating.md)
- [在 Microsoft Graph PowerShell SDK 中使用仅限应用的身份验证](app-only.md)
