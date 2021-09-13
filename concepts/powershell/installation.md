---
title: 安装 Microsoft Graph PowerShell SDK
description: 提供有关安装 Microsoft Graph PowerShell SDK 的说明。
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 0e4a7f9269aef1700431921aead6014a15afd8dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139042"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>安装 Microsoft Graph PowerShell SDK

> [!NOTE]
> 安装 SDK 的主模块将安装所有 38 个子模块。 考虑仅安装必要的模块，包括 `Microsoft.Graph.Authentication` 。

Microsoft Graph PowerShell SDK 发布在[PowerShell 库上](https://www.powershellgallery.com/packages/Microsoft.Graph)。 可以使用以下命令在 PowerShell 核心或 Windows PowerShell安装 SDK。

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

（可选）可以使用 参数更改安装 `-Scope` 范围。 这需要管理员权限。

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> 在 PowerShell 的一个版本中安装 SDK 不会为另一个版本安装它。 请务必在要用于它的 PowerShell 版本中运行安装命令。

## <a name="supported-powershell-versions"></a>支持的 PowerShell 版本

PowerShell 7 及更高版本是建议在所有平台上与 Microsoft Graph PowerShell SDK 一Graph PowerShell 版本。 将 SDK 与 PowerShell 7 或更高版本一同使用没有任何其他先决条件。

若要将 Microsoft Graph PowerShell SDK 与 Windows PowerShell 一Windows PowerShell。

- 升级到 [PowerShell 5.1 或更高版本](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell)
- 安装[.NET Framework 4.7.2 或更高版本](/dotnet/framework/install/)
- 使用 **将 PowerShellGet** 更新到最新版本 `Install-Module PowerShellGet -Force`

## <a name="verify-installation"></a>验证安装

安装完成后，可以使用以下命令验证已安装的版本。

```powershell
Get-InstalledModule Microsoft.Graph
```

输出中的版本应匹配在 PowerShell 库上发布的最新版本。 现在，你已准备好使用 SDK。

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

然后，通过运行以下命令删除所有依赖关系模块。

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>提供反馈

我们欢迎您提供反馈！ Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).
