---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd832b2892bfa84b2a856fd2531c85d29a33e68ae4722a4dd5626d27b391fb0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var properties = new PrintDocumentUploadProperties
{
    DocumentName = "TestFile.pdf",
    ContentType = "application/pdf",
    Size = 4533322
};

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"]
    .CreateUploadSession(properties)
    .Request()
    .PostAsync();

```