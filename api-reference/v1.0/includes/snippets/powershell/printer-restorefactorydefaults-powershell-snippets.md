---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41ca1d7db946456a6e04904b45de3e34a2cf15cc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346206"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Restore-MgPrintPrinterFactoryDefault -PrinterId $printerId

```