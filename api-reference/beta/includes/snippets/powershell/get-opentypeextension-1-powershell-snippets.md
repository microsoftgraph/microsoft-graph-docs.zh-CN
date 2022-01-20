---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1524f5b7c010f27d6e2eb3303b7eb050f225a298
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112867"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessageExtension -UserId $userId -MessageId $messageId -ExtensionId $extensionId

```