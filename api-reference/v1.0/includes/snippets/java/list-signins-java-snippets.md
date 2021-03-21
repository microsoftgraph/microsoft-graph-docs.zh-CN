---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 692d0b659f588ca51c58a95807c8c2fc89c19a65
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975535"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .get();

```