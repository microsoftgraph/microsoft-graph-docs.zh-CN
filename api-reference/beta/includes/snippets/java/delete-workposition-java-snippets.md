---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a3ad11100ab378652706bbe21167a9df74abd48
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977360"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().positions("{id}")
    .buildRequest()
    .delete();

```