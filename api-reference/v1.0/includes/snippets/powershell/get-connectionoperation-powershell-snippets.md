---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25655c517e47f14c89d3d9747b1ef2b6091eb29b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441377"
---
```powershell

Import-Module Microsoft.Graph.Search

Get-MgExternalConnectionOperation -ExternalConnectionId $externalConnectionId -ConnectionOperationId $connectionOperationId

```