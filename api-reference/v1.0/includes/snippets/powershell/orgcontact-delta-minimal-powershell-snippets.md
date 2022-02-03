---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01a405fc0529ece03891659099ddce3b18e3ec64
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348954"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgContactDelta -Property "displayName,jobTitle,mail" 

```