---
title: Microsoft Graph PowerShell SDK 入门
description: 使用 Microsoft Graph PowerShell SDK 执行一些基本任务，开始使用它。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 6f5ee22960f9bf33156807f9f55f49e6e4aa17b5
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777573"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="cf5d7-103">Microsoft Graph PowerShell SDK 入门</span><span class="sxs-lookup"><span data-stu-id="cf5d7-103">Get started with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="cf5d7-104">在本指南中，你将使用 Microsoft Graph PowerShell SDK 执行一些基本任务。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-104">In this guide you'll use the Microsoft Graph PowerShell SDK to perform some basic tasks.</span></span> <span data-ttu-id="cf5d7-105">如果尚未安装 [SDK，](installation.md)请在遵循本指南之前进行安装。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-105">If you haven't already [installed the SDK](installation.md), please do so before following this guide.</span></span>

## <a name="api-version"></a><span data-ttu-id="cf5d7-106">API 版本</span><span class="sxs-lookup"><span data-stu-id="cf5d7-106">API version</span></span>

<span data-ttu-id="cf5d7-107">默认情况下，SDK 使用[Microsoft Graph REST API v1.0。](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="cf5d7-107">By default, the SDK uses the [Microsoft Graph REST API v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=true).</span></span> <span data-ttu-id="cf5d7-108">可以使用命令更改 `Select-MgProfile` 此参数。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-108">You can change this by using the `Select-MgProfile` command.</span></span>

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a><span data-ttu-id="cf5d7-109">身份验证</span><span class="sxs-lookup"><span data-stu-id="cf5d7-109">Authentication</span></span>

<span data-ttu-id="cf5d7-110">PowerShell SDK 支持两种类型的身份验证：委派访问和仅应用访问。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-110">The PowerShell SDK supports two types of authentication: delegated access, and app-only access.</span></span> <span data-ttu-id="cf5d7-111">在本指南中，你将使用委派访问权限以用户的名义登录，同意 SDK 代表你操作，并调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-111">In this guide, you will use delegated access to login as a user, grant consent to the SDK to act on your behalf, and call the Microsoft Graph.</span></span>

<span data-ttu-id="cf5d7-112">有关将仅应用访问用于无人参与方案的详细信息，请参阅将仅应用身份验证与 [Microsoft Graph PowerShell SDK 一同使用](app-only.md)。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-112">For details on using app-only access for unattended scenarios, see [Use app-only authentication with the Microsoft Graph PowerShell SDK](app-only.md).</span></span>

### <a name="determine-required-permission-scopes"></a><span data-ttu-id="cf5d7-113">确定所需的权限范围</span><span class="sxs-lookup"><span data-stu-id="cf5d7-113">Determine required permission scopes</span></span>

<span data-ttu-id="cf5d7-114">Microsoft Graph 中的每个 API 都受一个或多个权限范围保护。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-114">Each API in the Microsoft Graph is protected by one or more permission scopes.</span></span> <span data-ttu-id="cf5d7-115">用户登录必须同意计划使用的 API 所需的范围之一。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-115">The user logging in must consent to one of the required scopes for the APIs you plan to use.</span></span> <span data-ttu-id="cf5d7-116">此示例中，我们将使用以下 API。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-116">In this example, we'll use the following APIs.</span></span>

- <span data-ttu-id="cf5d7-117">[列出](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) 要查找登录用户的用户 ID 的用户</span><span class="sxs-lookup"><span data-stu-id="cf5d7-117">[List users](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) to find the user ID of the logged-in user</span></span>
- <span data-ttu-id="cf5d7-118">[列出 joinedTeams，](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) 获取用户是其中一个成员的 Teams。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-118">[List joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) to get the Teams the user is a member of.</span></span>
- <span data-ttu-id="cf5d7-119">[列出频道](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) ，获取团队中的频道。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-119">[List channels](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) to get the channels in a Team.</span></span>
- <span data-ttu-id="cf5d7-120">[发送消息](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) 以向团队频道发送邮件。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-120">[Send message](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) to send a message to a Team channel.</span></span>

<span data-ttu-id="cf5d7-121">权限 `User.Read.All` 范围将启用前两个调用， `Group.ReadWrite.All` 该范围将启用其余调用。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-121">The `User.Read.All` permission scope will enable the first two calls, and the `Group.ReadWrite.All` scope will enable the rest.</span></span> <span data-ttu-id="cf5d7-122">这些权限需要管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-122">These permissions require an admin account.</span></span>

### <a name="sign-in"></a><span data-ttu-id="cf5d7-123">登录</span><span class="sxs-lookup"><span data-stu-id="cf5d7-123">Sign in</span></span>

<span data-ttu-id="cf5d7-124">使用 `Connect-MgGraph` 此命令使用所需范围登录。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-124">Use the `Connect-MgGraph` command to sign in with the required scopes.</span></span> <span data-ttu-id="cf5d7-125">你将需要使用管理员帐户登录，以同意所需的作用域。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-125">You'll need to sign in with an admin account to consent to the required scopes.</span></span>

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

<span data-ttu-id="cf5d7-126">该命令将提示您转到网页以使用设备代码登录。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-126">The command prompts you to go to a web page to sign in using a device code.</span></span> <span data-ttu-id="cf5d7-127">完成后，该命令会通过一条消息指示 `Welcome To Microsoft Graph!` 是否成功。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-127">Once you've done that, the command indicates success with a `Welcome To Microsoft Graph!` message.</span></span> <span data-ttu-id="cf5d7-128">每个会话只需执行一次此操作。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-128">You only need to do this once per session.</span></span>

> [!TIP]
> <span data-ttu-id="cf5d7-129">您可以通过使用新的权限范围重复该命令 `Connect-MgGraph` 来添加其他权限。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-129">You can add additional permissions by repeating the `Connect-MgGraph` command with the new permission scopes.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="cf5d7-130">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cf5d7-130">Call Microsoft Graph</span></span>

<span data-ttu-id="cf5d7-131">现在，你已登录，可以开始调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-131">Now that you're signed in, you can start making calls to Microsoft Graph.</span></span>

### <a name="get-the-signed-in-user"></a><span data-ttu-id="cf5d7-132">获取登录用户</span><span class="sxs-lookup"><span data-stu-id="cf5d7-132">Get the signed-in user</span></span>

<span data-ttu-id="cf5d7-133">在此部分中，你将找到登录用户并获取其用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-133">In this section you'll locate the signed-in user and get her user ID.</span></span> <span data-ttu-id="cf5d7-134">你将需要该参数用作以后将使用的其他命令的参数。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-134">You'll need that to use as a parameter to the other commands you'll use later.</span></span> <span data-ttu-id="cf5d7-135">首先运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-135">Start by running the following command.</span></span>

```powershell
Get-MgUser
```

<span data-ttu-id="cf5d7-136">这将输出 Microsoft 365 组织中用户列表。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-136">This outputs a listing of users in your Microsoft 365 organization.</span></span>

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

<span data-ttu-id="cf5d7-137">可以使用 [OData 筛选器来帮助](../query-parameters.md#filter-parameter) 找到您想要的特定用户。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-137">You can use an [OData filter](../query-parameters.md#filter-parameter) to help locate the specific user you want.</span></span> <span data-ttu-id="cf5d7-138">运行以下命令，替换为 `Megan Bowen` 显示名称登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-138">Run the following command, replacing `Megan Bowen` with the display name of the user you signed in with.</span></span>

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

<span data-ttu-id="cf5d7-139">通过输入以下内容验证是否有效。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-139">Verify that worked by entering the following.</span></span>

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a><span data-ttu-id="cf5d7-140">列出用户加入的 Teams</span><span class="sxs-lookup"><span data-stu-id="cf5d7-140">List the user's joined Teams</span></span>

<span data-ttu-id="cf5d7-141">现在，使用用户的 ID 作为命令 `Get-MgUserJoinedTeam` 的参数。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-141">Now use the user's ID as a parameter to the `Get-MgUserJoinedTeam` command.</span></span>

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

<span data-ttu-id="cf5d7-142">与命令 `Get-MgUser` 一样，这会提供 Teams 列表。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-142">Just like the `Get-MgUser` command, this gives a list of Teams.</span></span> <span data-ttu-id="cf5d7-143">选择用户加入的 Teams 之一，并使用其 `DisplayName` 筛选列表。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-143">Select one of the user's joined Teams and use its `DisplayName` to filter the list.</span></span>

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a><span data-ttu-id="cf5d7-144">列出团队频道</span><span class="sxs-lookup"><span data-stu-id="cf5d7-144">List Team channels</span></span>

<span data-ttu-id="cf5d7-145">现在，使用团队 ID 作为命令的参数，遵循列出所有频道的类似模式，然后筛选列表，获取 `Get-MgTeamChannel` 您想要的特定频道。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-145">Now use the Team's ID as a parameter to the `Get-MgTeamChannel` command, following a similar pattern of listing all channels, then filtering the list to get the specific channel you want.</span></span>

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a><span data-ttu-id="cf5d7-146">发送邮件</span><span class="sxs-lookup"><span data-stu-id="cf5d7-146">Send a message</span></span>

<span data-ttu-id="cf5d7-147">现在，你同时拥有团队 ID 和频道 ID，你可以向频道发布消息。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-147">Now that you have both the Team ID and the channel ID, you can post a message to the channel.</span></span> <span data-ttu-id="cf5d7-148">使用以下命令发送邮件。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-148">Use the following command to send the message.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

<span data-ttu-id="cf5d7-149">此命令与之前使用的命令不同。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-149">This command differs from the previous commands you used.</span></span> <span data-ttu-id="cf5d7-150">它实际上正在创建一些内容，而不只是查询数据。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-150">Instead of just querying data, it's actually creating something.</span></span> <span data-ttu-id="cf5d7-151">在 Microsoft Graph 中，这会转换为 HTTP，并且它需要该文章正文 `POST` 中的对象。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-151">In Microsoft Graph, this translates to an HTTP `POST`, and it requires an object in the body of that post.</span></span> <span data-ttu-id="cf5d7-152">在这种情况下，对象是 [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-152">In this case, the object is a [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true).</span></span> <span data-ttu-id="cf5d7-153">请注意， `-Body` 该命令的参数映射到 `body` 上的属性 `chatMessage` 。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-153">Note that the `-Body` parameter to the command maps to the `body` property on `chatMessage`.</span></span> <span data-ttu-id="cf5d7-154">其他属性的映射方式类似，因此可以更改发送的邮件。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-154">Other properties are mapped in a similar way, so you can change the message you send.</span></span> <span data-ttu-id="cf5d7-155">例如，若要发送紧急邮件，请使用以下命令。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-155">For example, to send an urgent message use the following command.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a><span data-ttu-id="cf5d7-156">注销</span><span class="sxs-lookup"><span data-stu-id="cf5d7-156">Sign out</span></span>

<span data-ttu-id="cf5d7-157">使用 `Disconnect-MgGraph` 命令注销。</span><span class="sxs-lookup"><span data-stu-id="cf5d7-157">Use the `Disconnect-MgGraph` command to sign out.</span></span>

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a><span data-ttu-id="cf5d7-158">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cf5d7-158">Next steps</span></span>

- [<span data-ttu-id="cf5d7-159">了解如何导航 SDK</span><span class="sxs-lookup"><span data-stu-id="cf5d7-159">Learn how to navigate the SDK</span></span>](navigating.md)
- [<span data-ttu-id="cf5d7-160">将仅应用身份验证与 Microsoft Graph PowerShell SDK 一同使用</span><span class="sxs-lookup"><span data-stu-id="cf5d7-160">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>](app-only.md)
