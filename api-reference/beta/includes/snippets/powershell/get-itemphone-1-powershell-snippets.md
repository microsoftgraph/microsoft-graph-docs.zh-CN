---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d4a976dddb70a72603154a933d1cd669e2efc4c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129770"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfilePhone -UserId $userId -ItemPhoneId $itemPhoneId

```