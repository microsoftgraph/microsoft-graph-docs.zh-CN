---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 091d00dbf7eb160fdcf34d0c10dc59c42e4861486208a554a9cb62bffdd99358
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplates = await graphClient.GroupSettingTemplates
    .Request()
    .GetAsync();

```