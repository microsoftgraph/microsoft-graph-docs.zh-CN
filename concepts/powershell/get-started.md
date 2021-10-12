---
title: Microsoft Graph PowerShell SDK 入门
description: 通过使用 Microsoft Graph PowerShell SDK 执行一些基本任务，开始使用它。
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 623c034622054150ff6b58b97e063f3e833489de
ms.sourcegitcommit: f7956d25472a55af03be83b6ab986a7149a7ac88
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/12/2021
ms.locfileid: "60270311"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Microsoft Graph PowerShell SDK 入门

在本指南中，你将使用 Microsoft Graph PowerShell SDK 来执行一些基本任务。 如果尚未安装 [SDK，](installation.md)请在遵循本指南之前进行安装。

## <a name="api-version"></a>API 版本

默认情况下，SDK 使用[Microsoft Graph REST API v1.0。](/graph/api/overview?view=graph-rest-1.0&preserve-view=true) 可以使用 命令更改 `Select-MgProfile` 这一点。

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>身份验证

PowerShell SDK 支持两种类型的身份验证：委派访问和仅应用访问。 在本指南中，你将使用委派访问权限以用户登录，同意 SDK 代表你操作，并调用 Microsoft Graph。

有关对无人参与方案使用仅应用访问的详细信息，请参阅使用 Microsoft Graph [PowerShell SDK 进行仅应用身份验证](app-only.md)。

### <a name="determine-required-permission-scopes"></a>确定所需的权限范围

Microsoft 管理中心Graph API 都受一个或多个权限范围保护。 用户登录必须同意计划使用的 API 的所需范围之一。 本示例中，我们将使用以下 API。

- [列出](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) 用户以查找登录用户的用户 ID
- [列出 joinedTeams，Teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true)用户是成员的列表。
- [列出频道](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) ，获取团队中的频道。
- [发送消息](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) 以将消息发送到团队频道。

权限 `User.Read.All` 范围将启用前两个调用， `Group.ReadWrite.All` 而该范围将启用其余调用。 这些权限需要管理员帐户。

### <a name="sign-in"></a>登录

使用 `Connect-MgGraph` 命令以所需范围登录。 你将需要使用管理员帐户登录，以同意所需的作用域。

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

该命令会提示你转到网页，以使用设备代码登录。 完成后，该命令会通过一条消息指示是否 `Welcome To Microsoft Graph!` 成功。 每个会话只需执行一次此操作。

> [!TIP]
> 您可以通过使用新的权限范围重复该命令 `Connect-MgGraph` 来添加其他权限。

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph

现在，你已登录，你可以开始调用 Microsoft Graph。

### <a name="get-the-signed-in-user"></a>获取登录用户

在此部分中，你将找到登录用户并获取其用户 ID。 你将需要该参数用作以后将使用的其他命令的参数。 首先运行以下命令。

```powershell
Get-MgUser
```

这会输出组织中用户Microsoft 365列表。

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

可以使用 [OData 筛选器来帮助](../query-parameters.md#filter-parameter) 找到您需要的特定用户。 运行以下命令，将 `Megan Bowen` 替换为显示名称登录的用户的用户名。

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

通过输入以下内容验证是否有效。

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>列出用户加入的团队

现在，使用用户的 ID 作为命令 `Get-MgUserJoinedTeam` 的参数。

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

与命令 `Get-MgUser` 一样，这会提供团队列表。 选择用户的加入团队之一并复制其 `Id` 。

### <a name="list-team-channels"></a>列出团队频道

现在，使用团队 ID 作为命令的参数，遵循列出所有频道的类似模式，然后筛选列表，获取 `Get-MgTeamChannel` 您想要的特定频道。

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId ID_FROM_PREVIOUS_STEP -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>发送消息

现在，你同时拥有团队 ID 和频道 ID，你可以向频道发布消息。 使用以下命令发送邮件。

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

此命令与之前使用的命令不同。 它实际上正在创建一些内容，而不只是查询数据。 在 Microsoft Graph 中，这会转换为 HTTP ，并且它需要该文章 `POST` 正文中的 对象。 在这种情况下，对象是 [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true)。 请注意， `-Body` 命令的参数映射到 `body` 上的 属性 `chatMessage` 。 其他属性以类似方式映射，因此可以更改发送的邮件。 例如，若要发送紧急邮件，请使用以下命令。

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a>注销

使用 `Disconnect-MgGraph` 命令注销。

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a>后续步骤

- [了解如何导航 SDK](navigating.md)
- [通过 Microsoft Graph PowerShell SDK 使用仅应用程序身份验证](app-only.md)
