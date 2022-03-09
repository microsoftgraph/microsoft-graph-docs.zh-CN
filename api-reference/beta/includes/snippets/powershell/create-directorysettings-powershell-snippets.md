---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46d9e929c02ab8bedb5cedc82ba5557b1f8b40ee
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395781"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    TemplateId = "62375ab9-6b52-47ed-826b-58e47e0e304b"
    Values = @(
        @{
            Name = "GuestUsageGuidelinesUrl"
            Value = "https://privacy.contoso.com/privacystatement"
        }
        @{
            Name = "EnableMSStandardBlockedWords"
            Value = "true"
        }
        @{
            Name = "EnableMIPLabels"
            Value = "true"
        }
        @{
            Name = "PrefixSuffixNamingRequirement"
            Value = "[Contoso-][GroupName]"
        }
    )
}

New-MgDirectorySetting -BodyParameter $params

```