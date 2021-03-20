---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b99d4e6e7a56e2c960dacd4b0a82b063390ddbe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976458"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Case _case = graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .buildRequest()
    .get();

```