---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3ffa578307dda51eada6c676242076ac16b5774
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394262"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgApplicationExtensionProperty -ApplicationId $applicationId -ExtensionPropertyId $extensionPropertyId

```