---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 991c70b2f681c24aa0d68b811a205357f4d20e5f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111459"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgInformationProtectionBitlockerRecoveryKey -BitlockerRecoveryKeyId $bitlockerRecoveryKeyId -Property "key" 

```