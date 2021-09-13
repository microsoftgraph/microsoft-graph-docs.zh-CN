---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f36589a831dc8b3505872c6ef6d3c4e10f39fbaecdbbaa7e9883c4f0496b969
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333737"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("db5e04be-daa2-4a35-beb1-5e73cc381599").installedApps("NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=")
    .upgrade()
    .buildRequest()
    .post();

```