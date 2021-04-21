---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e28143276c5a88bc60c5bb51004b089fd5430bda
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921853"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var properties = new PrintDocumentUploadProperties
{
    DocumentName = "TestFile.pdf",
    ContentType = "application/pdf",
    Size = 4533322
};

await graphClient.Print.Shares["{printerShare-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"]
    .CreateUploadSession(properties)
    .Request()
    .PostAsync();

```