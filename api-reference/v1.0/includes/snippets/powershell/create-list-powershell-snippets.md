---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 759fa408256adacb82932739c33e76b83932c9db
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132507"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    DisplayName = "Books"
    Columns = @(
        @{
            Name = "Author"
            Text = @{
            }
        }
        @{
            Name = "PageCount"
            Number = @{
            }
        }
    )
    List = @{
        Template = "genericList"
    }
}

New-MgSiteList -SiteId $siteId -BodyParameter $params

```