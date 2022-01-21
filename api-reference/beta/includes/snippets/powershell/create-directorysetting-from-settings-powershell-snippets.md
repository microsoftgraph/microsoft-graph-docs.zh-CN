---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e9f87efd36fe9381ab779db09aa31db606b89de
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090587"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "Group.Unified"
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