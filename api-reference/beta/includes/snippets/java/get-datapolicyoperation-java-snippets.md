---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51a0113ff5448eda348315e7f40119889544638d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968364"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataPolicyOperation dataPolicyOperation = graphClient.dataPolicyOperations("{id}")
    .buildRequest()
    .get();

```