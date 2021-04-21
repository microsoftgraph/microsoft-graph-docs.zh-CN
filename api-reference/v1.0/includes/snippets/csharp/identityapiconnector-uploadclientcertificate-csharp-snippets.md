---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96e4be79ab0442ee1a192f1504c5810a59699243
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";

var password = "<password>";

await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .UploadClientCertificate(pkcs12Value,password)
    .Request()
    .PostAsync();

```