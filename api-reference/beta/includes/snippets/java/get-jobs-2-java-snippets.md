---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8298c8430624c29fa7d445fca2c056b1c85c8e9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209140"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().shares("{id}").jobs()
    .buildRequest()
    .get();

```