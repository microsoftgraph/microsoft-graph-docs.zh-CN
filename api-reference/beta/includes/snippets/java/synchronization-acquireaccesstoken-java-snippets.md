---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afbd3065b1ba1a654bb14c8acb7dcd317d991167
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975874"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SynchronizationSecretKeyStringValuePair> credentialsList = new LinkedList<SynchronizationSecretKeyStringValuePair>();
SynchronizationSecretKeyStringValuePair credentials = new SynchronizationSecretKeyStringValuePair();

credentialsList.add(credentials);

graphClient.applications("{applicationsId}").synchronization()
    .acquireAccessToken(credentialsList)
    .buildRequest()
    .post();

```