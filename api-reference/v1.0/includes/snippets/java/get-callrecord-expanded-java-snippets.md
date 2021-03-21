---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4e9988e79f3668f797d22cb5e79ca06f7801079
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("{id}")
    .buildRequest()
    .expand("sessions($expand=segments)")
    .get();

```