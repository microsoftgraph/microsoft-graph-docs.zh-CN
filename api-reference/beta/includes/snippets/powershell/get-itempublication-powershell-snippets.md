---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2464c5b4f87d8325295b6d0f38c69fcbe5541189
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089957"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId

```