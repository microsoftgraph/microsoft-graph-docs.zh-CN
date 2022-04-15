---
title: 安装 Microsoft Graph PowerShell SDK
description: 提供有关安装 Microsoft Graph PowerShell SDK 的说明。
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 80086e4879ce9acb547e060c45891bd58dc602bf
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883386"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>安装 Microsoft Graph PowerShell SDK

> [!NOTE]
> 安装 SDK 的主模块将安装所有 38 个子模块。 请考虑仅安装必要的模块，包括 `Microsoft.Graph.Authentication`。 有关可用 Microsoft Graph 模块的列表，请使用以下命令。
>
> ```powershell
> Find-Module Microsoft.Graph*
> ```

Microsoft Graph PowerShell SDK 在[PowerShell 库](https://www.powershellgallery.com/packages/Microsoft.Graph)上发布。 可以在 PowerShell Core 中安装 SDK，也可以使用以下命令Windows PowerShell。

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

（可选）可以使用 `-Scope` 参数更改安装范围。 这需要管理员权限。

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> 在一个版本的 PowerShell 中安装 SDK 不会为另一个版本安装它。 请务必在要在其中使用的 PowerShell 版本内运行安装命令。

## <a name="supported-powershell-versions"></a>支持的 PowerShell 版本

建议使用 PowerShell 7 及更高版本，以便在所有平台上与 Microsoft Graph PowerShell SDK 配合使用。 将 SDK 与 PowerShell 7 或更高版本配合使用没有其他先决条件。

必须满足以下先决条件才能将 Microsoft Graph PowerShell SDK 与Windows PowerShell配合使用。

- 升级到 [PowerShell 5.1 或更高版本](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell)
- 安装[.NET Framework 4.7.2 或更高版本](/dotnet/framework/install/)
- Update **PowerShellGet** to the latest version using `Install-Module PowerShellGet -Force`

## <a name="verify-installation"></a>验证安装

安装完成后，可以使用以下命令验证已安装的版本。

```powershell
Get-InstalledModule Microsoft.Graph
```

输出中的版本应与PowerShell 库上发布的最新版本匹配。 现在可以使用 SDK 了。

> [!div class="nextstepaction"]
> [Microsoft Graph PowerShell SDK 入门](get-started.md)

## <a name="updating-the-sdk"></a>更新 SDK

可以使用以下命令更新 SDK 及其所有依赖项。

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>卸载 SDK

首先，使用以下命令卸载主模块。

```powershell
Uninstall-Module Microsoft.Graph
```

然后，通过运行以下命令删除所有依赖项模块。

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>提供反馈

我们欢迎反馈！ 请提供任何反馈或报告 [SDK GitHub存储库](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)上的任何问题。
