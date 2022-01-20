---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3da338c6b023235b24c0fc8f2bbc66ded53301d8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099506"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -Property "subject,body,bodyPreview,uniqueBody" 

```