---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec787bfe34ce69b3342835ea34b1b7b7395eb16f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971016"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("{domain-name}")
    .verify()
    .buildRequest()
    .post();

```