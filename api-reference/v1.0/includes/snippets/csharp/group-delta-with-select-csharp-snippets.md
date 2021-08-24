---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6c555f2fde6ebe7fc20f677ec9917b057cae3c63b3aaf4a4f335112480bc43f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups
    .Delta()
    .Request()
    .Select("displayName,description,mailNickname")
    .GetAsync();

```