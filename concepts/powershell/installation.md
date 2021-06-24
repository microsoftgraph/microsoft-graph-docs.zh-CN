---
title: 安装 Microsoft Graph PowerShell SDK
description: 提供有关安装 Microsoft Graph PowerShell SDK 的说明。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 58e967d7acedbbfe4f8c3781a7ec796e697a44c8
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107674"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="6207c-103">安装 Microsoft Graph PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="6207c-103">Install the Microsoft Graph PowerShell SDK</span></span>

> [!NOTE]
> <span data-ttu-id="6207c-104">安装 SDK 的主模块将安装所有 38 个子模块。</span><span class="sxs-lookup"><span data-stu-id="6207c-104">Installing the main module of the SDK will install all 38 sub modules.</span></span> <span data-ttu-id="6207c-105">考虑仅安装必要的模块，包括 `Microsoft.Graph.Authentication` 。</span><span class="sxs-lookup"><span data-stu-id="6207c-105">Consider only installing the neccessary modules, including `Microsoft.Graph.Authentication`.</span></span>

<span data-ttu-id="6207c-106">Microsoft Graph PowerShell SDK 发布在[PowerShell 库上](https://www.powershellgallery.com/packages/Microsoft.Graph)。</span><span class="sxs-lookup"><span data-stu-id="6207c-106">The Microsoft Graph PowerShell SDK is published on the [PowerShell Gallery](https://www.powershellgallery.com/packages/Microsoft.Graph).</span></span> <span data-ttu-id="6207c-107">可以使用以下命令在 PowerShell 核心或 Windows PowerShell安装 SDK。</span><span class="sxs-lookup"><span data-stu-id="6207c-107">You can install the SDK in PowerShell Core or Windows PowerShell using the following command.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

<span data-ttu-id="6207c-108">（可选）可以使用 参数更改安装 `-Scope` 范围。</span><span class="sxs-lookup"><span data-stu-id="6207c-108">Optionally, you can change the scope of the installation using the `-Scope` parameter.</span></span> <span data-ttu-id="6207c-109">这需要管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6207c-109">This requires admin permissions.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> <span data-ttu-id="6207c-110">在 PowerShell 的一个版本中安装 SDK 不会为另一个版本安装它。</span><span class="sxs-lookup"><span data-stu-id="6207c-110">Installing the SDK in one version of PowerShell does not install it for the other.</span></span> <span data-ttu-id="6207c-111">请务必在要用于它的 PowerShell 版本中运行安装命令。</span><span class="sxs-lookup"><span data-stu-id="6207c-111">Be sure to run the installation command inside the version of PowerShell you intend to use it in.</span></span>

## <a name="verify-installation"></a><span data-ttu-id="6207c-112">验证安装</span><span class="sxs-lookup"><span data-stu-id="6207c-112">Verify installation</span></span>

<span data-ttu-id="6207c-113">安装完成后，可以使用以下命令验证已安装的版本。</span><span class="sxs-lookup"><span data-stu-id="6207c-113">After the installation completes, you can verify the installed version with the following command.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph
```

<span data-ttu-id="6207c-114">输出中的版本应匹配在 PowerShell 库上发布的最新版本。</span><span class="sxs-lookup"><span data-stu-id="6207c-114">The version in the output should match the latest version published on the PowerShell Gallery.</span></span> <span data-ttu-id="6207c-115">现在，你已准备好使用 SDK。</span><span class="sxs-lookup"><span data-stu-id="6207c-115">Now you're ready to use the SDK.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6207c-116">Microsoft Graph PowerShell SDK 入门</span><span class="sxs-lookup"><span data-stu-id="6207c-116">Get started with the Microsoft Graph PowerShell SDK</span></span>](get-started.md)

## <a name="updating-the-sdk"></a><span data-ttu-id="6207c-117">更新 SDK</span><span class="sxs-lookup"><span data-stu-id="6207c-117">Updating the SDK</span></span>

<span data-ttu-id="6207c-118">可以使用以下命令更新 SDK 及其所有依赖项。</span><span class="sxs-lookup"><span data-stu-id="6207c-118">You can update the SDK and all of its dependencies using the following command.</span></span>

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a><span data-ttu-id="6207c-119">卸载 SDK</span><span class="sxs-lookup"><span data-stu-id="6207c-119">Uninstalling the SDK</span></span>

<span data-ttu-id="6207c-120">首先，使用以下命令卸载主模块。</span><span class="sxs-lookup"><span data-stu-id="6207c-120">First, use the following command to uninstall the main module.</span></span>

```powershell
Uninstall-Module Microsoft.Graph
```

<span data-ttu-id="6207c-121">然后，通过运行以下命令删除所有依赖关系模块。</span><span class="sxs-lookup"><span data-stu-id="6207c-121">Then, remove all of the dependency modules by running the following commands.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a><span data-ttu-id="6207c-122">提供反馈</span><span class="sxs-lookup"><span data-stu-id="6207c-122">Provide feedback</span></span>

<span data-ttu-id="6207c-123">我们欢迎您提供反馈！</span><span class="sxs-lookup"><span data-stu-id="6207c-123">We welcome feedback!</span></span> <span data-ttu-id="6207c-124">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="6207c-124">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span></span>
