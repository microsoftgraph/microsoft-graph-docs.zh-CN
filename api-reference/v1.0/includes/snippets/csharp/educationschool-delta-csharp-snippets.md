---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84a92cddc2a03eb988b68e4a9b48979936afcabfcd289ddcbc35ab4a4fc9f4c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Schools
    .Delta()
    .Request()
    .GetAsync();

```