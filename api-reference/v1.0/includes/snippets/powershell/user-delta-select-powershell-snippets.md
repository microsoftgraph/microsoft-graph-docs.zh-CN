---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18254455eadca90e3309aa624c734dd83d40b7ff
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344687"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

Get-MgUserDelta -Property "displayName,jobTitle,mobilePhone" 

```