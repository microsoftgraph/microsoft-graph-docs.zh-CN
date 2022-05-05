---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d92e3f2216ead3c6fe98d80f0ff0a3ceb4f980
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210365"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationCallContentSharingSession -CallId $callId -ContentSharingSessionId $contentSharingSessionId

```