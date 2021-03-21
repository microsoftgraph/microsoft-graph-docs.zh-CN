---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 377169db997ab038eaa7d4114a5375cbeb5b226b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967535"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("1a5f91a7-9bd1-4d5f-bb86-f43554cac51c").taskTriggers("25be207e-1154-491f-aa68-a9f7007d4bec")
    .buildRequest()
    .delete();

```