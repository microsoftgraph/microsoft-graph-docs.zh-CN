---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae7101ba0d0f5d221f89f53af55d9688f1f38b4b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977721"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .resume()
    .buildRequest()
    .post();

```