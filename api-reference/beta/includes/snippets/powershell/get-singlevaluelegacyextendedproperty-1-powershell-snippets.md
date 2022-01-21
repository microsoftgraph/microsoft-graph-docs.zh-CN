---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7110632b3e08bd529f9d0497dfa1e68a8fd808a1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122980"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "singleValueExtendedProperties(`$filter=id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color')" 

```