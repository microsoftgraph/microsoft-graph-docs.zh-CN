---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7c9e029c28294556234e339682be86b022d70d7
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb"].Jobs["5182"]
    .Request()
    .GetAsync();

```