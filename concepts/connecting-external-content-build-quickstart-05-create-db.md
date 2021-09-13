---
ms.localizationpriority: medium
ms.openlocfilehash: e8f13a3fe886db688d12a997f0cddc38547a30f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289512"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

1. 在 PartsInventoryConnector.csproj 所在的 (CLI) 打开命令行接口。
2. 运行以下命令：

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> 如果 CSV 文件中架构发生更改，请运行以下命令，将这些更改反映到 SQLite 数据库中。

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
