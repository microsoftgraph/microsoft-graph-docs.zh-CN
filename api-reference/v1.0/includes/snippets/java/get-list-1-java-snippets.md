---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e956c4673b682bfa57ba7c60ffa24d27f5566454
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956443"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest()
    .get();

```