---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ada7ecbebd4c7fdd2bcca8255116747b4d5b9293
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101858"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgApplicationExtensionProperty -ApplicationId $applicationId -ExtensionPropertyId $extensionPropertyId

```