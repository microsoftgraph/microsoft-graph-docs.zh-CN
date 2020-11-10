---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e64e9092d7ce6407e7202e4b3cc6cda47962e11
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971458"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/onenote/resources/{id}/content", InputStream.class)
    .buildRequest()
    .get();

```