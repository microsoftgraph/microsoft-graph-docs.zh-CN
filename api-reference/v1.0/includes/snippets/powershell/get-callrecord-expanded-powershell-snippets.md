---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5515f0fc5a67098d37f6d4cf9298085791ff53d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130521"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationCallRecord -CallRecordId $callRecordId -ExpandProperty "sessions(`$expand=segments)" 

```