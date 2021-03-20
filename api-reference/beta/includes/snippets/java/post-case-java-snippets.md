---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5617b50d717b58cba17c813d70a73a1fe75a44eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966660"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Case _case = new Case();
_case.displayName = "My Case 1";

graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .post(_case);

```