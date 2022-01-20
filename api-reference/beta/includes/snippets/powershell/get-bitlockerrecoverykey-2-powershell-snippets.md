---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef95ae783307a9f7b2934916259858015d55cbe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130080"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgInformationProtectionBitlockerRecoveryKey -Filter "deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'" 

```