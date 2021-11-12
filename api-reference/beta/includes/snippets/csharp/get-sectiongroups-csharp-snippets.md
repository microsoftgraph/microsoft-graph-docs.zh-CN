---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d04091eb309afde8976bd5104680cfc5ecde246d4fde995bd5d0e6daa3298a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"].SectionGroups
    .Request()
    .GetAsync();

```