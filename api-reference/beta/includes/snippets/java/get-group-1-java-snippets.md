---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e57772265f60e762ccb4469c7b78ed375d9001
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961801"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4")
    .buildRequest()
    .get();

```