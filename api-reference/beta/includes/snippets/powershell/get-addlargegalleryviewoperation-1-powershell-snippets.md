---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49f04a6ca8892ad35f6a8f71d7a43c9f7181d926
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204148"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationCallOperation -CallId $callId -CommsOperationId $commsOperationId

```