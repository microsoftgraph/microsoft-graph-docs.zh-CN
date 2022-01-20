---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d65c2d0ef5095c9592e2bd593b429159c6a117a6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105745"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationOnlineMeeting -Filter "VideoTeleconferenceId eq '123456789'" 

```