---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55006a0dd42ef57605adf75f8b4a0d5f17a70597053946f89ede46827c703244
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getUserArchivedPrintJobs = await graphClient.Print.Reports
    .GetUserArchivedPrintJobs("016b5565-3bbf-4067-b9ff-4d68167eb1a6","2021-05-24","2021-05-25")
    .Request()
    .GetAsync();

```