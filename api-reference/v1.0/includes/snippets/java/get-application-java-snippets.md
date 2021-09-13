---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33c9bfa58d5edd3b83ecedbf6ac06fd0acd7184a2a7888f1ea7d865c20960805
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = graphClient.applications("{id}")
    .buildRequest()
    .get();

```