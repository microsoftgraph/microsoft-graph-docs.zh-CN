---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a97fbad323da0edd8fc964372cfd0ba9e2672e54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967077"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().me().assignments("{id}").rubric().reference()
    .buildRequest()
    .delete();

```