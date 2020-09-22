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
# <a name="install-the-microsoft-graph-powershell-sdk"></a>安装 Microsoft Graph PowerShell SDK

Microsoft Graph PowerShell SDK 发布在 [PowerShell 库](https://www.powershellgallery.com/packages/Microsoft.Graph)中。 您可以使用以下命令在 PowerShell Core 或 Windows PowerShell 中安装 SDK。

```powershell
Install-Module Microsoft.Graph
```

（可选）您可以使用参数更改安装的默认范围 `-Scope` 。 这需要管理员权限。

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> 在一个版本的 PowerShell 中安装 SDK 并不会为另一个版本安装 SDK。 请务必在您打算在其中使用安装命令的 PowerShell 版本中运行安装命令。

## <a name="verify-installation"></a>验证安装

安装完成后，您可以使用以下命令验证已安装的版本。

```powershell
Get-InstalledModule Microsoft.Graph
```

输出中的版本应与在 PowerShell 库上发布的最新版本相匹配。 现在，你已准备好使用 SDK。

> [!div class="nextstepaction"]
> [Microsoft Graph PowerShell SDK 入门](get-started.md)

## <a name="updating-the-sdk"></a>更新 SDK

您可以使用以下命令更新 SDK 及其所有依赖项。

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>卸载 SDK

首先，使用以下命令卸载主模块。

```powershell
Uninstall-Module Microsoft.Graph
```

然后，通过运行以下命令来删除所有依赖项模块。

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>提供反馈

我们欢迎你的反馈！ 请在 [SDK GitHub 存储库](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)中提供任何反馈或报告任何问题。
