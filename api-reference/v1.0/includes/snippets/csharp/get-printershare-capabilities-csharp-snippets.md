---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 438f2843c51bdf88cc4505acf84a8e036d8aac01414a849bac106aa1f17556ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .Select("id,displayName,capabilities")
    .GetAsync();

```