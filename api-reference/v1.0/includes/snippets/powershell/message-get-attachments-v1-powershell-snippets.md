---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c900adf1380c95d1452df72eab2963c61d7f1b08
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100737"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessageAttachment -UserId $userId -MessageId $messageId

```