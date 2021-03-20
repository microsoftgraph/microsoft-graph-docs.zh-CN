---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0cb4afca56d9a4b235b0d014b804dfa87930346
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976835"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImage cloudPcDeviceImage = graphClient.deviceManagement().virtualEndpoint().deviceImages("{id}")
    .buildRequest()
    .get();

```