---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00e584ecf64a1ab2ed82c050d24950bc5f445286
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980931"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("db5e04be-daa2-4a35-beb1-5e73cc381599").installedApps("NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=")
    .upgrade()
    .buildRequest()
    .post();

```