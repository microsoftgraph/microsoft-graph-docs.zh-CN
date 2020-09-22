---
title: 安装 Microsoft Graph PowerShell SDK
description: 提供了有关安装 Microsoft Graph PowerShell SDK 的说明。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 245cf03c8edf04a43c563bd19832eb0a35cf7cff
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193659"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="ad004-103">安装 Microsoft Graph PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="ad004-103">Install the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="ad004-104">Microsoft Graph PowerShell SDK 发布在 [PowerShell 库](https://www.powershellgallery.com/packages/Microsoft.Graph)中。</span><span class="sxs-lookup"><span data-stu-id="ad004-104">The Microsoft Graph PowerShell SDK is published on the [PowerShell Gallery](https://www.powershellgallery.com/packages/Microsoft.Graph).</span></span> <span data-ttu-id="ad004-105">您可以使用以下命令在 PowerShell Core 或 Windows PowerShell 中安装 SDK。</span><span class="sxs-lookup"><span data-stu-id="ad004-105">You can install the SDK in PowerShell Core or Windows PowerShell using the following command.</span></span>

```powershell
Install-Module Microsoft.Graph
```

<span data-ttu-id="ad004-106">（可选）您可以使用参数更改安装的默认范围 `-Scope` 。</span><span class="sxs-lookup"><span data-stu-id="ad004-106">Optionally, you can change the default scope of the installation using the `-Scope` parameter.</span></span> <span data-ttu-id="ad004-107">这需要管理员权限。</span><span class="sxs-lookup"><span data-stu-id="ad004-107">This requires admin permissions.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> <span data-ttu-id="ad004-108">在一个版本的 PowerShell 中安装 SDK 并不会为另一个版本安装 SDK。</span><span class="sxs-lookup"><span data-stu-id="ad004-108">Installing the SDK in one version of PowerShell does not install it for the other.</span></span> <span data-ttu-id="ad004-109">请务必在您打算在其中使用安装命令的 PowerShell 版本中运行安装命令。</span><span class="sxs-lookup"><span data-stu-id="ad004-109">Be sure to run the installation command inside the version of PowerShell you intend to use it in.</span></span>

## <a name="verify-installation"></a><span data-ttu-id="ad004-110">验证安装</span><span class="sxs-lookup"><span data-stu-id="ad004-110">Verify installation</span></span>

<span data-ttu-id="ad004-111">安装完成后，您可以使用以下命令验证已安装的版本。</span><span class="sxs-lookup"><span data-stu-id="ad004-111">After the installation completes, you can verify the installed version with the following command.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph
```

<span data-ttu-id="ad004-112">输出中的版本应与在 PowerShell 库上发布的最新版本相匹配。</span><span class="sxs-lookup"><span data-stu-id="ad004-112">The version in the output should match the latest version published on the PowerShell Gallery.</span></span> <span data-ttu-id="ad004-113">现在，你已准备好使用 SDK。</span><span class="sxs-lookup"><span data-stu-id="ad004-113">Now you're ready to use the SDK.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ad004-114">Microsoft Graph PowerShell SDK 入门</span><span class="sxs-lookup"><span data-stu-id="ad004-114">Get started with the Microsoft Graph PowerShell SDK</span></span>](get-started.md)

## <a name="updating-the-sdk"></a><span data-ttu-id="ad004-115">更新 SDK</span><span class="sxs-lookup"><span data-stu-id="ad004-115">Updating the SDK</span></span>

<span data-ttu-id="ad004-116">您可以使用以下命令更新 SDK 及其所有依赖项。</span><span class="sxs-lookup"><span data-stu-id="ad004-116">You can update the SDK and all of its dependencies using the following command.</span></span>

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a><span data-ttu-id="ad004-117">卸载 SDK</span><span class="sxs-lookup"><span data-stu-id="ad004-117">Uninstalling the SDK</span></span>

<span data-ttu-id="ad004-118">首先，使用以下命令卸载主模块。</span><span class="sxs-lookup"><span data-stu-id="ad004-118">First, use the following command to uninstall the main module.</span></span>

```powershell
Uninstall-Module Microsoft.Graph
```

<span data-ttu-id="ad004-119">然后，通过运行以下命令来删除所有依赖项模块。</span><span class="sxs-lookup"><span data-stu-id="ad004-119">Then, remove all of the dependency modules by running the following commands.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a><span data-ttu-id="ad004-120">提供反馈</span><span class="sxs-lookup"><span data-stu-id="ad004-120">Provide feedback</span></span>

<span data-ttu-id="ad004-121">我们欢迎你的反馈！</span><span class="sxs-lookup"><span data-stu-id="ad004-121">We welcome feedback!</span></span> <span data-ttu-id="ad004-122">请在 [SDK GitHub 存储库](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)中提供任何反馈或报告任何问题。</span><span class="sxs-lookup"><span data-stu-id="ad004-122">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span></span>
