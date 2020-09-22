---
title: Microsoft Graph PowerShell SDK 入门
description: 使用 Microsoft Graph PowerShell SDK 开始使用它可执行一些基本任务。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: ab4a0c5a65dc752116d3622f71e024e039d90675
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193684"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Microsoft Graph PowerShell SDK 入门

在本指南中，你将使用 Microsoft Graph PowerShell SDK 执行一些基本任务。 如果尚未 [安装 SDK](installation.md)，请在遵循本指南之前执行此操作。

## <a name="api-version"></a>API 版本

默认情况下，SDK 使用 [Microsoft GRAPH REST API](/graph/api/overview?view=graph-rest-1.0)v1.0。 可以使用命令对此进行更改 `Select-MgProfile` 。

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>身份验证

PowerShell SDK 支持两种类型的身份验证：委派访问权限和仅限应用访问。 在本指南中，您将使用委派访问权限以用户身份登录，并同意 SDK 代表你进行操作，并调用 Microsoft Graph。

有关使用仅限应用访问的无人参与方案的详细信息，请参阅 [使用 Microsoft Graph POWERSHELL SDK 的仅应用程序身份验证](app-only.md)。

### <a name="determine-required-permission-scopes"></a>确定所需的权限范围

Microsoft Graph 中的每个 API 都由一个或多个权限范围保护。 登录用户必须同意您计划使用的 Api 所需的作用域之一。 在此示例中，我们将使用以下 Api。

- [列出用户](/graph/api/user-list?view=graph-rest-1.0) 以查找已登录用户的用户 ID
- [列出 joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) 以获取用户所属的团队。
- [列出通道](/graph/api/channel-list?view=graph-rest-1.0) 以获取团队中的频道。
- [发送邮件](/graph/api/channel-post-messages?view=graph-rest-1.0) 以将邮件发送到团队频道。

`User.Read.All`权限范围将启用前两个呼叫，并且 `Group.ReadWrite.All` 作用域将启用其余的。 这些权限需要管理员帐户。

### <a name="sign-in"></a>登录

使用 `Connect-Graph` 命令使用所需的作用域进行登录。 你需要使用管理员帐户登录才能同意所需的范围。

```powershell
Connect-Graph -Scopes "User.Read.All","Group.ReadWrite.All"
```

该命令将提示您转到要使用设备代码登录的网页。 完成此操作后，该命令将使用消息指示是否成功 `Welcome To Microsoft Graph!` 。 您只需对每个会话执行一次此操作。

> [!TIP]
> 您可以通过使用新的权限范围重复命令来添加其他权限 `Connect-Graph` 。

## <a name="call-microsoft-graph"></a>调用 Microsoft Graph

现在，你已登录，你可以开始调用 Microsoft Graph。

### <a name="get-the-signed-in-user"></a>获取已登录用户

在本节中，你将找到已登录用户并获取其用户 ID。 你将需要使用作为参数，以供稍后使用的其他命令使用。 首先，运行以下命令。

```powershell
Get-MgUser
```

这将输出 Microsoft 365 组织中的用户列表。

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

您可以使用 [OData 筛选器](../query-parameters.md#filter-parameter) 来帮助查找所需的特定用户。 运行以下命令，将替换 `Megan Bowen` 为您登录时使用的用户的显示名称。

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

通过输入以下命令验证是否正常工作。

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>列出用户加入的团队

现在，将用户的 ID 用作命令的参数 `Get-MgUserJoinedTeam` 。

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

就像 `Get-MgUser` 命令一样，这将提供一个团队列表。 选择用户加入的团队之一并使用其 `DisplayName` 筛选列表。

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a>列出团队频道

现在，将团队的 ID 用作命令的参数 `Get-MgTeamChannel` ，遵循列出所有通道的类似模式，然后筛选列表以获取所需的特定频道。

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>发送邮件

现在，你已拥有团队 ID 和通道 ID，你可以将消息发布到频道。 使用以下命令发送邮件。

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

此命令与以前使用的命令不同。 实际上，它只是创建一些内容，而不是只查询数据。 在 Microsoft Graph 中，这会转换为 HTTP `POST` ，它需要该文章的正文中的对象。 在这种情况下，对象为 [了 chatmessage](/graph/resources/chatmessage?view=graph-rest-1.0)。 请注意， `-Body` 命令的参数映射到上的 `body` 属性 `chatMessage` 。 其他属性以类似的方式进行映射，因此您可以更改发送的邮件。 例如，若要发送紧急邮件，请使用以下命令。

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

## <a name="next-steps"></a>后续步骤

- [了解如何导航 SDK](navigating.md)
- [对 Microsoft Graph PowerShell SDK 使用仅限应用的身份验证](app-only.md)
