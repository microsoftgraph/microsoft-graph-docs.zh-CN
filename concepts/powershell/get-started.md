---
title: Microsoft Graph PowerShell SDK 入门
description: 使用 Microsoft Graph PowerShell SDK 开始使用它可执行一些基本任务。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: eeeaee7bf45e3b8d17f866425556102eef2c1cae
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782884"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="37e60-103">Microsoft Graph PowerShell SDK 入门</span><span class="sxs-lookup"><span data-stu-id="37e60-103">Get started with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="37e60-104">在本指南中，你将使用 Microsoft Graph PowerShell SDK 执行一些基本任务。</span><span class="sxs-lookup"><span data-stu-id="37e60-104">In this guide you'll use the Microsoft Graph PowerShell SDK to perform some basic tasks.</span></span> <span data-ttu-id="37e60-105">如果尚未 [安装 SDK](installation.md)，请在遵循本指南之前执行此操作。</span><span class="sxs-lookup"><span data-stu-id="37e60-105">If you haven't already [installed the SDK](installation.md), please do so before following this guide.</span></span>

## <a name="api-version"></a><span data-ttu-id="37e60-106">API 版本</span><span class="sxs-lookup"><span data-stu-id="37e60-106">API version</span></span>

<span data-ttu-id="37e60-107">默认情况下，SDK 使用 [Microsoft GRAPH REST API](/graph/api/overview?view=graph-rest-1.0)v1.0。</span><span class="sxs-lookup"><span data-stu-id="37e60-107">By default, the SDK uses the [Microsoft Graph REST API v1.0](/graph/api/overview?view=graph-rest-1.0).</span></span> <span data-ttu-id="37e60-108">可以使用命令对此进行更改 `Select-MgProfile` 。</span><span class="sxs-lookup"><span data-stu-id="37e60-108">You can change this by using the `Select-MgProfile` command.</span></span>

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a><span data-ttu-id="37e60-109">身份验证</span><span class="sxs-lookup"><span data-stu-id="37e60-109">Authentication</span></span>

<span data-ttu-id="37e60-110">PowerShell SDK 支持两种类型的身份验证：委派访问权限和仅限应用访问。</span><span class="sxs-lookup"><span data-stu-id="37e60-110">The PowerShell SDK supports two types of authentication: delegated access, and app-only access.</span></span> <span data-ttu-id="37e60-111">在本指南中，您将使用委派访问权限以用户身份登录，并同意 SDK 代表你进行操作，并调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="37e60-111">In this guide, you will use delegated access to login as a user, grant consent to the SDK to act on your behalf, and call the Microsoft Graph.</span></span>

<span data-ttu-id="37e60-112">有关使用仅限应用访问的无人参与方案的详细信息，请参阅 [使用 Microsoft Graph POWERSHELL SDK 的仅应用程序身份验证](app-only.md)。</span><span class="sxs-lookup"><span data-stu-id="37e60-112">For details on using app-only access for unattended scenarios, see [Use app-only authentication with the Microsoft Graph PowerShell SDK](app-only.md).</span></span>

### <a name="determine-required-permission-scopes"></a><span data-ttu-id="37e60-113">确定所需的权限范围</span><span class="sxs-lookup"><span data-stu-id="37e60-113">Determine required permission scopes</span></span>

<span data-ttu-id="37e60-114">Microsoft Graph 中的每个 API 都由一个或多个权限范围保护。</span><span class="sxs-lookup"><span data-stu-id="37e60-114">Each API in the Microsoft Graph is protected by one or more permission scopes.</span></span> <span data-ttu-id="37e60-115">登录用户必须同意您计划使用的 Api 所需的作用域之一。</span><span class="sxs-lookup"><span data-stu-id="37e60-115">The user logging in must consent to one of the required scopes for the APIs you plan to use.</span></span> <span data-ttu-id="37e60-116">在此示例中，我们将使用以下 Api。</span><span class="sxs-lookup"><span data-stu-id="37e60-116">In this example, we'll use the following APIs.</span></span>

- <span data-ttu-id="37e60-117">[列出用户](/graph/api/user-list?view=graph-rest-1.0) 以查找已登录用户的用户 ID</span><span class="sxs-lookup"><span data-stu-id="37e60-117">[List users](/graph/api/user-list?view=graph-rest-1.0) to find the user ID of the logged-in user</span></span>
- <span data-ttu-id="37e60-118">[列出 joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) 以获取用户所属的团队。</span><span class="sxs-lookup"><span data-stu-id="37e60-118">[List joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get the Teams the user is a member of.</span></span>
- <span data-ttu-id="37e60-119">[列出通道](/graph/api/channel-list?view=graph-rest-1.0) 以获取团队中的频道。</span><span class="sxs-lookup"><span data-stu-id="37e60-119">[List channels](/graph/api/channel-list?view=graph-rest-1.0) to get the channels in a Team.</span></span>
- <span data-ttu-id="37e60-120">[发送邮件](/graph/api/channel-post-messages?view=graph-rest-1.0) 以将邮件发送到团队频道。</span><span class="sxs-lookup"><span data-stu-id="37e60-120">[Send message](/graph/api/channel-post-messages?view=graph-rest-1.0) to send a message to a Team channel.</span></span>

<span data-ttu-id="37e60-121">`User.Read.All`权限范围将启用前两个呼叫，并且 `Group.ReadWrite.All` 作用域将启用其余的。</span><span class="sxs-lookup"><span data-stu-id="37e60-121">The `User.Read.All` permission scope will enable the first two calls, and the `Group.ReadWrite.All` scope will enable the rest.</span></span> <span data-ttu-id="37e60-122">这些权限需要管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="37e60-122">These permissions require an admin account.</span></span>

### <a name="sign-in"></a><span data-ttu-id="37e60-123">登录</span><span class="sxs-lookup"><span data-stu-id="37e60-123">Sign in</span></span>

<span data-ttu-id="37e60-124">使用 `Connect-MgGraph` 命令使用所需的作用域进行登录。</span><span class="sxs-lookup"><span data-stu-id="37e60-124">Use the `Connect-MgGraph` command to sign in with the required scopes.</span></span> <span data-ttu-id="37e60-125">你需要使用管理员帐户登录才能同意所需的范围。</span><span class="sxs-lookup"><span data-stu-id="37e60-125">You'll need to sign in with an admin account to consent to the required scopes.</span></span>

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

<span data-ttu-id="37e60-126">该命令将提示您转到要使用设备代码登录的网页。</span><span class="sxs-lookup"><span data-stu-id="37e60-126">The command prompts you to go to a web page to sign in using a device code.</span></span> <span data-ttu-id="37e60-127">完成此操作后，该命令将使用消息指示是否成功 `Welcome To Microsoft Graph!` 。</span><span class="sxs-lookup"><span data-stu-id="37e60-127">Once you've done that, the command indicates success with a `Welcome To Microsoft Graph!` message.</span></span> <span data-ttu-id="37e60-128">您只需对每个会话执行一次此操作。</span><span class="sxs-lookup"><span data-stu-id="37e60-128">You only need to do this once per session.</span></span>

> [!TIP]
> <span data-ttu-id="37e60-129">您可以通过使用新的权限范围重复命令来添加其他权限 `Connect-MgGraph` 。</span><span class="sxs-lookup"><span data-stu-id="37e60-129">You can add additional permissions by repeating the `Connect-MgGraph` command with the new permission scopes.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="37e60-130">调用 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="37e60-130">Call Microsoft Graph</span></span>

<span data-ttu-id="37e60-131">现在，你已登录，你可以开始调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="37e60-131">Now that you're signed in, you can start making calls to Microsoft Graph.</span></span>

### <a name="get-the-signed-in-user"></a><span data-ttu-id="37e60-132">获取已登录用户</span><span class="sxs-lookup"><span data-stu-id="37e60-132">Get the signed-in user</span></span>

<span data-ttu-id="37e60-133">在本节中，你将找到已登录用户并获取其用户 ID。</span><span class="sxs-lookup"><span data-stu-id="37e60-133">In this section you'll locate the signed-in user and get her user ID.</span></span> <span data-ttu-id="37e60-134">你将需要使用作为参数，以供稍后使用的其他命令使用。</span><span class="sxs-lookup"><span data-stu-id="37e60-134">You'll need that to use as a parameter to the other commands you'll use later.</span></span> <span data-ttu-id="37e60-135">首先，运行以下命令。</span><span class="sxs-lookup"><span data-stu-id="37e60-135">Start by running the following command.</span></span>

```powershell
Get-MgUser
```

<span data-ttu-id="37e60-136">这将输出 Microsoft 365 组织中的用户列表。</span><span class="sxs-lookup"><span data-stu-id="37e60-136">This outputs a listing of users in your Microsoft 365 organization.</span></span>

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

<span data-ttu-id="37e60-137">您可以使用 [OData 筛选器](../query-parameters.md#filter-parameter) 来帮助查找所需的特定用户。</span><span class="sxs-lookup"><span data-stu-id="37e60-137">You can use an [OData filter](../query-parameters.md#filter-parameter) to help locate the specific user you want.</span></span> <span data-ttu-id="37e60-138">运行以下命令，将替换 `Megan Bowen` 为您登录时使用的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="37e60-138">Run the following command, replacing `Megan Bowen` with the display name of the user you signed in with.</span></span>

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

<span data-ttu-id="37e60-139">通过输入以下命令验证是否正常工作。</span><span class="sxs-lookup"><span data-stu-id="37e60-139">Verify that worked by entering the following.</span></span>

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a><span data-ttu-id="37e60-140">列出用户加入的团队</span><span class="sxs-lookup"><span data-stu-id="37e60-140">List the user's joined Teams</span></span>

<span data-ttu-id="37e60-141">现在，将用户的 ID 用作命令的参数 `Get-MgUserJoinedTeam` 。</span><span class="sxs-lookup"><span data-stu-id="37e60-141">Now use the user's ID as a parameter to the `Get-MgUserJoinedTeam` command.</span></span>

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

<span data-ttu-id="37e60-142">就像 `Get-MgUser` 命令一样，这将提供一个团队列表。</span><span class="sxs-lookup"><span data-stu-id="37e60-142">Just like the `Get-MgUser` command, this gives a list of Teams.</span></span> <span data-ttu-id="37e60-143">选择用户加入的团队之一并使用其 `DisplayName` 筛选列表。</span><span class="sxs-lookup"><span data-stu-id="37e60-143">Select one of the user's joined Teams and use its `DisplayName` to filter the list.</span></span>

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a><span data-ttu-id="37e60-144">列出团队频道</span><span class="sxs-lookup"><span data-stu-id="37e60-144">List Team channels</span></span>

<span data-ttu-id="37e60-145">现在，将团队的 ID 用作命令的参数 `Get-MgTeamChannel` ，遵循列出所有通道的类似模式，然后筛选列表以获取所需的特定频道。</span><span class="sxs-lookup"><span data-stu-id="37e60-145">Now use the Team's ID as a parameter to the `Get-MgTeamChannel` command, following a similar pattern of listing all channels, then filtering the list to get the specific channel you want.</span></span>

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a><span data-ttu-id="37e60-146">发送邮件</span><span class="sxs-lookup"><span data-stu-id="37e60-146">Send a message</span></span>

<span data-ttu-id="37e60-147">现在，你已拥有团队 ID 和通道 ID，你可以将消息发布到频道。</span><span class="sxs-lookup"><span data-stu-id="37e60-147">Now that you have both the Team ID and the channel ID, you can post a message to the channel.</span></span> <span data-ttu-id="37e60-148">使用以下命令发送邮件。</span><span class="sxs-lookup"><span data-stu-id="37e60-148">Use the following command to send the message.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

<span data-ttu-id="37e60-149">此命令与以前使用的命令不同。</span><span class="sxs-lookup"><span data-stu-id="37e60-149">This command differs from the previous commands you used.</span></span> <span data-ttu-id="37e60-150">实际上，它只是创建一些内容，而不是只查询数据。</span><span class="sxs-lookup"><span data-stu-id="37e60-150">Instead of just querying data, it's actually creating something.</span></span> <span data-ttu-id="37e60-151">在 Microsoft Graph 中，这会转换为 HTTP `POST` ，它需要该文章的正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="37e60-151">In Microsoft Graph, this translates to an HTTP `POST`, and it requires an object in the body of that post.</span></span> <span data-ttu-id="37e60-152">在这种情况下，对象为 [了 chatmessage](/graph/resources/chatmessage?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="37e60-152">In this case, the object is a [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0).</span></span> <span data-ttu-id="37e60-153">请注意， `-Body` 命令的参数映射到上的 `body` 属性 `chatMessage` 。</span><span class="sxs-lookup"><span data-stu-id="37e60-153">Note that the `-Body` parameter to the command maps to the `body` property on `chatMessage`.</span></span> <span data-ttu-id="37e60-154">其他属性以类似的方式进行映射，因此您可以更改发送的邮件。</span><span class="sxs-lookup"><span data-stu-id="37e60-154">Other properties are mapped in a similar way, so you can change the message you send.</span></span> <span data-ttu-id="37e60-155">例如，若要发送紧急邮件，请使用以下命令。</span><span class="sxs-lookup"><span data-stu-id="37e60-155">For example, to send an urgent message use the following command.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

## <a name="next-steps"></a><span data-ttu-id="37e60-156">后续步骤</span><span class="sxs-lookup"><span data-stu-id="37e60-156">Next steps</span></span>

- [<span data-ttu-id="37e60-157">了解如何导航 SDK</span><span class="sxs-lookup"><span data-stu-id="37e60-157">Learn how to navigate the SDK</span></span>](navigating.md)
- [<span data-ttu-id="37e60-158">对 Microsoft Graph PowerShell SDK 使用仅限应用的身份验证</span><span class="sxs-lookup"><span data-stu-id="37e60-158">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>](app-only.md)
