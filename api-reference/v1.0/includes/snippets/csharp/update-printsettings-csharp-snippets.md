---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68663bcd255386da1424a86d8bcc3e67d75be8d2ee6a6839c888b4cfc9625f79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printSettings = new PrintSettings
{
    DocumentConversionEnabled = true
};

var print = new Print();
print.Settings = printSettings;

await graphClient.Print
    .Request()
    .UpdateAsync(print);

```