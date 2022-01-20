---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42efa159c6f6704b0408618353771c8c85031071
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116135"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId

```