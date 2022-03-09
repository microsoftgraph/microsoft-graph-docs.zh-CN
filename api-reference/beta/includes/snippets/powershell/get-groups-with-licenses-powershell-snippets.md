---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fc63f00230f0ad8f5bb7bbed1c79ae4891970a2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393380"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Property "id,assignedLicenses" -Filter "assignedLicenses/any()" 

```